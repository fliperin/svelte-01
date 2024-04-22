<script>
    let src = '200w.gif';
</script>

<div class="quadradinho">
    <img {src} alt="test" class="img">
</div>


<style>
    .quadradinho{
        width:20%;
        height:200px;
        background-color: purple;
        display: flex;
        flex-direction: row nowrap;
        justify-content: center;
        align-items: center;
        color: white;
        font-family: Segoe UI;
        font-size: 20px;
    }

    .img{
        width:80%;
        height: 80%;
    }
</style>
