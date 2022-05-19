

<div class="main">
    <div class="nav">
      {#each ids as id, index}
        <button class={id}  on:click={() =>onClick(index)}> {id}</button>
      {/each}
    </div>
    <div class="outlet">
        <p>{contents[state]}</p>
    </div>
</div>


<script>
    let state = 0;
    export let contents = []

    export let ids = []
    
        
    function onClick(id) {
        state = id
    }
    
</script>


<style>
  
  /* Tab Navigation */
  div.nav {
    width: 100%;
    margin: 0 auto 1rem;
    display: flex;
    justify-content: space-between;
  
  }
  
  div.nav button {
    width: 150px;
    height: 50px;
    padding: 1rem;
    margin: 0.5px 10px;
    list-style: none;
    text-align: center;
    cursor: pointer;
    transition: all 0.7s;
    border-radius: 0.5rem;
    font-size: 15px;
    background-color: rgba(219, 209, 209, 0.993);
  }
  
  
  div.nav button:hover {
    background-color: rgba(219, 209, 209, 0.299);
  }

  .outlet {
    width: 100%;
    height: 180px;
    padding: 1rem 1rem;
    list-style: none;
    cursor: pointer;
    transition: all 0.7s;
    border-radius: 0.5rem;
    border: 1px solid black;
    background: #e1e8ec;
    font-size: 25px;
  }
  
</style>