<script>
  let good = ""
  let count = 0
</script>

Le compte est à {count}
<button
  on:click={() => {
    good = "good"
  }}
>
  Hey
</button>

<button
  on:click={() => {
    count += 1
  }}
>
  +
</button>

<button
  on:click={() => {
    good = ""
  }}
>
  Cancel
</button>

<div class={good}>Make me look good</div>

<style>
  .good {
    padding: 8px;
    background-color: bisque;
    border-radius: 10px;
    /* make it spin */
    animation: spin 1s linear infinite;
  }

  @keyframes spin {
    from {
      transform: rotate(0deg);
    }
    to {
      transform: rotate(360deg);
    }
  }
</style>
