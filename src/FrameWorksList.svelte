<script>
  let frameworks = [
    { id: 1, name: "Svelte" },
    { id: 2, name: "Angular" },
    { id: 3, name: "React" },
    { id: 4, name: "Vue" }
  ];
</script>

<ul>
  {#each frameworks as { id, name }}
    <li>{id} : {name}</li>
  {/each}
</ul>
