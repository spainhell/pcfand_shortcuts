<script>
    export let labels = [];
    export let delims = [];
    let result = "";

    if (delims.length > labels.length) {
        result = "bad delimiters count";
    } else {
        for (let i = 0; i < labels.length; i++) {
            result += "<span style=\"border: solid black 1px\">" + labels[i] + "</span>";
            if (i < delims.length) {
                result += delims[i];
            }
        }
    }
</script>

<div>
    { @html result }
</div>

<style>
</style>

