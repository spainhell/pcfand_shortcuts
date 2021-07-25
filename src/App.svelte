<script lang="ts">
	import Keyb from './Keyb.svelte';
</script>

<h2>Datový editor</h2>
<table>
    <tr><td><Keyb labels={["&larr;"]}/></td><td>předchozí údaj</td></tr>
    <tr><td><Keyb labels={["&rarr;"]}/></td><td>následující údaj</td></tr>
    <tr><td><Keyb labels={["Enter"]}/></td><td>další editovaný údaj</td></tr>
    <tr><td><Keyb labels={["Home"]}/></td><td>první údaj ve větě</td></tr>
    <tr><td><Keyb labels={["End"]}/></td><td>poslední pořízený údaj ve větě</td></tr>
    <tr><td><Keyb labels={["Ctrl", "&bsol;"]} delims={["+"]}/></td><td>na začátek další věty</td></tr>
</table>

<h2>Pohyb po větách</h2>
<table>
    <tr><td><Keyb labels={["Page Up"]}/></td><td>o obrazovku vzad</td></tr>
    <tr><td><Keyb labels={["Page Down"]}/></td><td>o obrazovku vpřed</td></tr>
    <tr><td><Keyb labels={["&uarr;", "Ctrl", "Home"]} delims={[", ", "+"]}/></td><td>předchozí věta</td></tr>
    <tr><td><Keyb labels={["&darr;", "Ctrl", "End"]} delims={[", ", "+"]}/></td><td>následující věta</td></tr>
    <tr><td><Keyb labels={["Ctrl", "Page Up"]} delims={["+"]}/></td><td>první věta</td></tr>
    <tr><td><Keyb labels={["Ctrl", "Page Down"]} delims={["+"]}/></td><td>poslední věta</td></tr>
    <tr><td><Keyb labels={["F3"]}/></td><td>najdi větu (podle klíč. údaje)</td></tr>
    <tr><td><Keyb labels={["Ctrl", "F3"]} delims={["+"]}/></td><td>najdi větu (podle jejího čísla)</td></tr>
</table>


<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>