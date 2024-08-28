<script>
  export let phoneNumber = "1234567890"; // Replace with the actual phone number
  export let displayName = "Trey"; // Optional: Name to display in the link text

  // Construct the tel link
  $: telLink = `tel:${phoneNumber}`;
</script>

<a href={telLink}>Call me? ({displayName})</a>
