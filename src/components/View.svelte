<script>
	import { counter } from '../store';
	import Button from './Button.svelte';
    const up = () => {
        $counter++;
    };
    const down = () => {
        $counter--;
    }
</script>

<h1>{$counter}</h1>
<Button value={'+'} on:click={up}/>
<Button value={'-'} on:click={down}/>
