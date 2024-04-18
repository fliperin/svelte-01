<script>
    import Abduzido from './Abduzido.svelte';


    let vary = 0;

    function aumentar(){
        vary = vary + 2;
    }

</script>

<div class="container">
    <h1>Teste de svelte do fliperin</h1>
    <p>Visite <a href="https://kit.svelte.dev">este link</a> para fazer sei la o que</p>
    <button on:click={aumentar}> teste {vary} </button>
</div>

<Abduzido/>

<style>
    *{
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
        font-size: 20px;
        cursor:pointer;
        transition: 0.2s linear;
    }

    button:hover{
        filter: brightness(40%);
    }
</style>

