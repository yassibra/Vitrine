
<script lang="ts">
  let count=0;
  const cars = ["Saab", "Volvo", "BMW"];
  cars.push("BMM")
  function addOne(){
    count += 1;
  }
  import Nav from './Nav.svelte';
</script>
<Nav/>
<button class="btn">Hello daisyui</button>
<button class="btn btn-accent btn-outline">Button</button>
<button class="btn" on:click={addOne}>
 Clicked {count} oui times
</button>
{#each cars as car}
  <button class="btn">{car} t</button>

{/each}