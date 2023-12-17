<nav>
    <h2><a href="/">AV</a></h2>
    <button>Menu</button>
</nav>

<style>
    @import './fonts.css';
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