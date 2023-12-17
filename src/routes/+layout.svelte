<script>
    let opened = false
</script>

<nav>
    <h2><a href="/">AV</a></h2>
    <button on:click={()=>{opened = true}}>Menu</button>
</nav>
<div class="menu" class:open = {opened === true}>
    <button on:click={()=>{opened = false}}>Close</button>
    <a href="/">Home</a>
    <a href="/about">About</a>
    <a href="/projects">Projects</a>
    <a href="/contact">Contact</a>
</div>

<style>
    @import './fonts.css';
    .menu{
        position: absolute;
        background-color: #FF6F00;
        width: 20vw;
        height: 100vh;
        right: 0;
        transform: translateX(30vw);
        transition: 1s;
        display: flex;
        flex-direction: column;
        justify-content: space-around;
        padding: 0 5vw;
        align-items: end;
    }
    .menu a{
        font-family: mono;
        color: #101010;
        font-size: 4rem;
    }
    .menu a:hover{
        color: black;
    }
    .open{
        transform: translateX(0vw);
        transition: 1s;
    }
    nav{
        display: flex;
        border-bottom: 1px solid white;
        background: rgba( 255, 255, 255, 0.25 );
        backdrop-filter: blur(11px) saturate(122%);
        -webkit-backdrop-filter: blur(8px) saturate(122%);
        background-color: rgba(16, 16, 16, 0.62);
        border-bottom: 1px solid rgba(255, 255, 255, 0.125);
        color:white;
        position: fixed;
        width: 94dvw;
        height: 10dvh;
        align-items: center;
        padding: 0 3dvw;
        justify-content: space-between;
    }
    h2{
        font-family: mono;
        font-size: 2rem;
    }
    a{
        text-decoration: none;
        color: white;
        margin: 0;
        padding: 0;
    }
    a:hover{
        color: #FF6F00;
    }
</style>

<slot></slot>