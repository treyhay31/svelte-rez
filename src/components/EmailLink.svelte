<script>
  export let email = "treyhay@gmail.com";
  export let subject = "Opportunity to collaborate";
  export let body = "Hi Trey, Can you bring some awesome to our project?...";
  let svgElement;
  let emailDiv;
  let isEmailVisible = false;

  function toggleEmailVisibility() {
    isEmailVisible = !isEmailVisible;
    emailDiv.style.display = isEmailVisible ? "block" : "none";
  }
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

<div class="email-component">
  <svg
    bind:this={svgElement}
    on:click={toggleEmailVisibility}
    on:keydown={toggleEmailVisibility}
    fill="#1C2033"
    width="52"
    height="52"
    version="1.1"
    id="lni_lni-postcard"
    xmlns="http://www.w3.org/2000/svg"
    xmlns:xlink="http://www.w3.org/1999/xlink"
    x="0px"
    y="0px"
    viewBox="0 0 64 64"
    style="enable-background:new 0 0 64 64;"
    xml:space="preserve"
  >
    <g>
      <path
        d="M56,11.9H8c-3.4,0-6.2,2.8-6.2,6.2v27.7c0,3.4,2.8,6.2,6.2,6.2h48c3.4,0,6.2-2.8,6.2-6.2V18.2C62.2,14.7,59.4,11.9,56,11.9
            z M57.8,45.8c0,1-0.8,1.8-1.8,1.8H8c-1,0-1.8-0.8-1.8-1.8V18.2c0-1,0.8-1.8,1.8-1.8h48c1,0,1.8,0.8,1.8,1.8V45.8z"
      />
      <path
        d="M32,20.9c-1.2,0-2.2,1-2.2,2.2v15.3c0,1.2,1,2.2,2.2,2.2c1.2,0,2.2-1,2.2-2.2V23.1C34.2,21.9,33.2,20.9,32,20.9z"
      />
      <path
        d="M11.6,33h8.9c1.2,0,2.2-1,2.2-2.2s-1-2.2-2.2-2.2h-8.9c-1.2,0-2.2,1-2.2,2.2S10.4,33,11.6,33z"
      />
      <path
        d="M52,20.9h-9.4c-1.5,0-2.6,1.2-2.6,2.6v9.4c0,1.4,1.2,2.6,2.6,2.6H52c1.4,0,2.6-1.2,2.6-2.6v-9.4C54.6,22,53.4,20.9,52,20.9
            z M50.1,31h-5.7v-5.7h5.7V31z"
      />
      <path
        d="M23,36.1H11.6c-1.2,0-2.2,1-2.2,2.2s1,2.2,2.2,2.2H23c1.2,0,2.2-1,2.2-2.2S24.3,36.1,23,36.1z"
      />
    </g>
  </svg>

  <div class="email" bind:this={emailDiv} style="display: none;">
    <a class="font-header" href={mailtoLink}>Email me?</a>
    <button on:click={() => copy(`${email}`)}> 📋 </button>
    <div id="clipboard"></div>
  </div>
</div>

<style>
  .email-component {
    position: relative;
    z-index: 100;
  }
  svg {
    cursor: pointer;
  }
  button {
    background-color: transparent;
    cursor: pointer;
    outline: none;
    border: none;
    font-size: 2rem;
  }
  .email {
    position: absolute;
    top: -6rem;
    right: -19rem;
    display: grid;
    grid-template-columns: 1fr 1fr;
    place-items: center;
    place-content: center;

    border-radius: 2rem;
    border-bottom-left-radius: 3px;

    background: var(--robin-egg-blue);
    padding-top: 0.7rem;
    padding-left: 1.5rem;
    padding-right: 1rem;
    line-height: 3rem;
  }
  a {
    font-size: 2rem;
  }
  #clipboard {
    display: none;
  }
</style>
