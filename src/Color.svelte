<script>
    export let colors = [];
    let order = ['black', 'blue', 'green', 'cyan', 'red', 'DarkViolet', 'brown', 'gray',
                 'gray', 'lightblue', 'lightgreen', 'lightcyan', 'orange', 'violet', 'SandyBrown', 'lightgray'];
    let comb = [];
    colors.forEach(col => {
        let nr = parseInt(col, 10);
        comb.push(order[nr >> 4]);
        comb.push(order[nr & 0x0F]);
    });
    console.log(comb);
</script>

    {#each colors as color, i}
        <span style="font-family: monospace; color: {comb[2*i+1]}; background: {comb[2*i]}">{color}</span><br>
    {/each}

<style>

</style>