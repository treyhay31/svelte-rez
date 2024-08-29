<script>
  import CopyClipboard from "./CopyClipboard.svelte";
  export let phoneNumber = "1234567890"; // Replace with the actual phone number
  export let displayName = "Trey"; // Optional: Name to display in the link text

  // Construct the tel link
  $: telLink = `tel:${phoneNumber}`;

  const copy = (thing) => {
    console.log("copy", thing);
    const app = new CopyClipboard({
      target: document.getElementById("clipboard"),
      props: { name: thing },
    });
    app.$destroy();
  };
</script>

<div class="phone">
  <a class="font-header" href={telLink}>Call me? ({displayName})</a>
  <button on:click={() => copy(`${phoneNumber}`)}> 📋 </button>
  <div id="clipboard"></div>
</div>

<style>
  .phone {
    display: grid;
    grid-template-columns: 1fr 1fr;
    place-items: center;
    place-content: center;
  }
  a {
    font-size: 2rem;
  }
  #clipboard {
    display: none;
  }
</style>
