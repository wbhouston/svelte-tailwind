<script>
  let count = 0
  const increment = () => {
    count += 1
  }
</script>

<button style='border-1 px-2 py-1 font-bold' on:click={increment}>
  count is {count}
</button>