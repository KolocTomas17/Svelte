<script>
	let count = 1;

	// the `$:` means 're-run whenever these values change'
	$: one = count * 1;
	$: oned = doubled * 1;

	$: doubled = count * 2;
	$: quadrupled = doubled * 2;

	$: three = count * 3;
	$: threed = doubled * 3;

	$: four = count * 4;
	$: foured = doubled * 4;

	$: five = count * 5;
	$: fived = doubled * 5;

	$: six = count * 6;
	$: sixed = doubled * 6;

	$: seven = count * 7;
	$: sevened = doubled * 7;

	$: eight = count * 8;
	$: eighted = doubled * 8;


	$: nine = count * 9;
	$: nined = doubled * 9;

	$: ten = count * 10;
	$: tened = doubled * 10;

	function handleClick() {
		count += 1;
	}
</script>

<button on:click={handleClick}>
	Count: {count}
</button>

<box>
	<p>{count}  *  1 = {one}</p>
	<p>{doubled}  *  1 = {oned}</p>

	<p>{count}  *  2 = {doubled}</p>
	<p>{doubled}   * 2 = {quadrupled}</p>
	
	<p>{count}  *  3 = {three}</p>
	<p>{doubled}  *  3 = {threed}</p>
	
	<p>{count}  *  4 = {four}</p>
	<p>{doubled} * 4 = {foured}</p>
	
	<p>{count}  *  5 = {five}</p>
	<p>{doubled}  *  5 = {fived}</p>
</box>


<box>
	<p>{count}  *  6 = {six}</p>
	<p>{doubled}  *  6 = {sixed}</p>

	<p>{count}  *  7 = {seven}</p>
	<p>{doubled}  *  7 = {sevened}</p>

	<p>{count}  *  8 = {eight}</p>
	<p>{doubled}  *  8 = {eighted}</p>

	<p>{count}  *  9 = {nine}</p>
	<p>{doubled}  *  9 = {nined}</p>

	<p>{count}  *  10 = {ten}</p>
	<p>{doubled}  *  10 = {tened}</p>
</box>


