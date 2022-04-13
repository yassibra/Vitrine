<button class="btn">Hello daisyui</button>
<script lang="ts">
  let count=0;
  const cars = ["Saab", "Volvo", "BMW"];
  cars.push("BMM")
  function addOne(){
    count += 1;
  }
</script>
<button class="btn" on:click={addOne}>
 Clicked {count} oui times
</button>
{#each cars as car}
  <button class="btn">{car} t</button>

{/each}