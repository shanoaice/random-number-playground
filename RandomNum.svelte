<script>
  export let maxValue;
  export let minValue;
  let result = 0;

  function genRand() {
    result = Math.random() * (maxValue - minValue) + minValue;
  }

  function genRandInt() {
    const min = Math.ceil(minValue);
    const max = Math.floor(maxValue);
    result = Math.floor(Math.random() * (max - min)) + min;
  }

  function reset() {
    result = 0;
  }
</script>

<style>
  button {
    padding: 1em 2em
  }
</style>

<p>{result}</p>

<button on:click={genRand}>Generate Random Number</button>
<button on:click={genRandInt}>Generate Random Integer</button>
<button on:click={reset}>Reset</button>