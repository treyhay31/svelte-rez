<script>
  export let email = "treyhay@gmail.com";
  export let subject = "Opportunity to collaborate";
  export let body = "Hi Trey, Can you bring some awesome to our project?...";

  $: encodedSubject = encodeURIComponent(subject);
  $: encodedBody = encodeURIComponent(body);
  $: mailtoLink = `mailto:${email}?subject=${encodedSubject}&body=${encodedBody}`;
</script>

<a href={mailtoLink}>Email me?</a>
