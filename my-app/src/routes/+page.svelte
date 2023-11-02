<script>
  let count = 1;

  // the `$:` means 're-run whenever these values change'
  $: one = count * 1;

  $: doubled = count * 2;

  $: three = count * 3;

  $: four = count * 4;

  $: five = count * 5;

  $: six = count * 6;

  $: seven = count * 7;

  $: eight = count * 8;

  $: nine = count * 9;

  $: ten = count * 10;

  function handleClick() {
    count += 1;
  }

  function delClick() {
    count = 1;
  }
</script>

<button on:click={handleClick}>
  Add number {count}
</button>
<button on:click={delClick}>
  Reset
</button>


<box>
  <p>{count} * 1 = {one}</p>

  <p>{count} * 2 = {doubled}</p>

  <p>{count} * 3 = {three}</p>

  <p>{count} * 4 = {four}</p>

  <p>{count} * 5 = {five}</p>
</box>

<box>
  <p>{count} * 6 = {six}</p>

  <p>{count} * 7 = {seven}</p>

  <p>{count} * 8 = {eight}</p>

  <p>{count} * 9 = {nine}</p>

  <p>{count} * 10 = {ten}</p>
</box>
