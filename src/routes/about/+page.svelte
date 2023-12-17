<div class="container">
    <div class="content">
        <div class="url">
            \ about
        </div>
    </div>
    <div class="lines">
        <hr/>
        <hr/>
        <hr/>
        <div class="background">
            <div class="noise"></div>
        </div>
    </div>
</div>

<style>
    .lines{
        position:absolute;
        width: 100dvw;
        height: 100dvh;
        display:flex;
        z-index: -1;
        top: 0;
        background-color: #101010;;
    }
    .lines hr{
        position: relative;
        width:1px;
        border: none;
        background-color: rgba(255, 255, 255);
        opacity: 0.2;
    }
    .url{
        font-family: mono;
        font-size: 1.2rem;
    }
    .container{
        background-color: transparent;
        color:white;
        height: 100vh;
    }
    .content{
        padding:15dvh 3rem;
    }
    .noise{
        background: url(/background.png);
        position: absolute;
        width: 100dvw;
        height: 100dvh;
        z-index: -1;
        top: 0;
        left: 0;
        opacity: 0.05;
    }
</style>