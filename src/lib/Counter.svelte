<script>
  let count = 0
  const increment = () => {
    count += 1
  }
</script>

<button class='border border-gray-800 rounded-sm px-2 py-1 font-semibold' on:click={increment}>
  count is {count}
</button>