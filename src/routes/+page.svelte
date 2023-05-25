<script>

    export let characters = [];

    import Card from '$lib/Card.svelte'
    const BASE_URL = "https://rickandmortyapi.com/api";
  
    fetch(`${BASE_URL}/character`)
      .then(res => res.json())
      .then(data => {
        characters = data.results;
        console.log(characters);
      });
  </script>
  
  <div class = "characters">
    {#each characters as character}
        <div>{character.name +" "+ character.species+ " " + character.status}</div>
        
    {/each}

</div>
  
<Card />


