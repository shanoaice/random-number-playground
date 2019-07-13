<script>
  let maxValue = 1;
  let minValue = 0;
  import RandomNum from "./RandomNum";
</script>

<style>
  main {
    font-family: sans-serif;
    text-align: center;
  }
  #maxValue {
    height: 2em;
  }
  #minValue {
    height: 2em;
  }
</style>

<main>
  <h1>Random Number Playground</h1>
</main>

<label for="minValue">Min Random Value</label>
<input type=number bind:value={minValue} id="minValue">

<br>
<br>

<label for="maxValue">Max Random Value:</label>
<input type=number bind:value={maxValue} id="maxValue" />

<br>
<br>

<RandomNum maxValue={maxValue} minValue={minValue} />
