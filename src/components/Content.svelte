
<div class="outlet">
    <p>{contents[state]}</p>
</div>

<script>

    export let state = 0;

    const contents = [
        'Esse é o texto da Primeira Tab',
        'Esse é o texto da Segunda Tab',
        'Esse é o texto da Terceira Tab',
        'Esse é o texto da Quarta Tab'
    ]

</script>

<style>
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