

<div class="main">
    <div class="nav">
        <button class="Tab01"  on:click={() =>onClick("0")}> Tab 01</button>
        <button class="Tab02"  on:click={() =>onClick("1")}> Tab 02</button>
        <button class="Tab03"  on:click={() =>onClick("2")}> Tab 03</button>
        <button class="Tab04"  on:click={() =>onClick("3")}> Tab 04</button>
    </div>
    <div class="outlet">
        <Content state={aux}></Content>
    </div>
</div>


<script>
    import Content from "./content.svelte";
    
        let aux = 0
        
        function onClick(id) {
            aux = id
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
  
</style>