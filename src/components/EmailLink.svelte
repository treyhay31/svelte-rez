<script>
  export let email = "treyhay@gmail.com";
  export let subject = "Opportunity to collaborate";
  export let body = "Hi Trey, Can you bring some awesome to our project?...";

  $: encodedSubject = encodeURIComponent(subject);
  $: encodedBody = encodeURIComponent(body);
  $: mailtoLink = `mailto:${email}?subject=${encodedSubject}&body=${encodedBody}`;

  const copy = (thing) => {
    console.log("copy", thing);
    const app = new CopyClipboard({
      target: document.getElementById("clipboard"),
      props: { name: thing },
    });
    app.$destroy();
  };
</script>

<div class="email">
  <a class="font-header" href={mailtoLink}>Email me?</a>
  <button on:click={() => copy(`${email}`)}> 📋 </button>
  <div id="clipboard"></div>
</div>

<style>
  button {
    background-color: transparent;
    cursor: pointer;
  }
  .email {
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
