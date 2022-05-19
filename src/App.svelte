<div class="main">
    <div class="App">
        <Tabs ids={ids} contents={contents}></Tabs>
    </div>
</div>

<script>
import './assets/base.css';

import Tabs from "./components/Tabs.svelte";

    const contents = [
        'Esse é o texto da Primeira Tab',
        'Esse é o texto da Segunda Tab',
        'Esse é o texto da Terceira Tab',
        'Esse é o texto da Quarta Tab'
    ]

    const ids = [
          "Tab-01",
          "Tab-02",
          "Tab-03",
          "Tab-04"
        ]

</script>

<style>
    .main {
    box-sizing: border-box;
    padding: 0;
    margin: 0;
  }
  
  .App {
    width: 100vw;
    height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
    overflow: hidden;
  }

  
</style>