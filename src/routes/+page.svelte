<script>
    import Abduzido from './Abduzido.svelte';


    let vary = 0;
    let paragraph = 'Visite <a href="https://kit.svelte.dev">este link</a> para fazer sei la o que';

    function aumentar(){
        vary += 1;
    }

</script>

<div class="container">
    <h1>Teste de svelte do fliperin</h1>
    <p>{@html paragraph}</p>
    <button on:click={aumentar}> clicou {vary} {vary === 1 ? 'vez' : 'vezes'}</button>
</div>

<div class="container2">
    <Abduzido/>
    <Abduzido/>
    <Abduzido/>
    <Abduzido/>
    <Abduzido/>
    <Abduzido/>
    <Abduzido/>
    <Abduzido/>
    <Abduzido/>
    <Abduzido/>
</div>

<style>
    :global(body){
        margin: 0 auto;
    }

    .container{
        width:100%;
        height:300px;
        background-color:aquamarine;
        display: flex;
        flex-flow: column nowrap;
        align-content: center;
        align-items: center;
        justify-content: center;
        justify-self: center;
    }

    .container2{
        width:100%;
        height:300px;
        display: flex;
        flex-flow: row wrap;
    }


    h1, p{
        font-family: 'Segoe UI';
        color: #333;
    }

    button{
        padding:10px;
        border-radius: 5px;
        width:10%;
        border-style: none;
        background-color: #333;
        color: white;
        font-size: 16px;
        cursor:pointer;
        transition: 0.2s linear;
    }

    button:hover{
        filter: brightness(40%);
    }
</style>

