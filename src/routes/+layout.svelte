<script>
    let opened = false
</script>

<nav>
    <h2><a href="/">AV</a></h2>
    <button on:click={()=>{
        opened = true
        sessionStorage.setItem(opened,true)
        }}>Menu</button>
</nav>
<div class="menu" class:open = {opened === true}>
    <div class="menu-head">
        <div class="menu-text">
            Menu
        </div>
        <button on:click={()=>{opened = false}}>X</button>
    </div>
    <div class="menu-links">
        <a href="/" class="menu-link"><span>01</span><span>Home</span></a>
        <a href="/about" class="menu-link"><span>02</span><span>About</span></a>
        <a href="/projects" class="menu-link"><span>03</span><span>Projects</span></a>
        <a href="/contact" class="menu-link"><span>04</span><span>Contact</span></a>
    </div>
    <div class="qr-code">
        <img src="/qr-code.svg" alt="qr-code"/>
    </div>
    <div class="qr-text">
        <p>Do not scan this QR Code</p>
    </div>
</div>

<style>
    @import './fonts.css';
    .menu{
        position: absolute;
        background-color: #FF6F00;
        width: 20vw;
        height: 100dvh;
        right: 0;
        transform: translateX(30vw);
        transition: 1s;
        display: flex;
        flex-direction: column;
        padding: 0 5dvw;
        align-items: center;
    }
    .menu button{
        border-radius: 50px;
        width: 2.5rem;
        height: 2.5rem;
        background-color: #FF6F00;
        border: 1px solid #101010;
        font-family: Aeonik;
    }
    .menu button:hover{
        background-color: #101010;
        color: #FF6F00;
        cursor: pointer;
    }
    .menu-links{
        display: flex;
        flex-direction: column;
        justify-content: space-around;
        height: 30dvh;
    }
    .menu-head{
        display: flex;
        width: 30dvw;
        justify-content: space-between;
        margin: 3dvh 0;
        font-family: mono;
    }
    .menu-head button{
        margin-right:2dvw;
    }
    .menu-text{
        padding: 0 2vw;
        font-size: 2rem;
    }
    .menu-link{
        border: 1px solid black;
        width: 26dvw;
        display: flex;
        align-items: center;
        justify-content: space-between;
        padding: 2dvh 2dvw;
    }
    .menu-link span{
        padding: 0 3dvw;
    }
    .menu a{
        font-family: mono;
        color: #101010;
        font-size: 1rem;
    }
    .menu a:hover{
        color: white;
        background-color: #101010;
    }
    .qr-code{
        margin-top: 5rem;
    }
    .qr-code img{
        width: 20dvw;
    }
    .qr-text{
        font-family: mono;
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
    nav button{
        background-color: #101010;
        color: white;
        font-family: mono;
        border: 1px solid white;
        display: flex;
        align-items: center;
        justify-content: center;
        width: 6rem;
        height: 2.5rem;
        font-size: 1.2rem;
    }
    nav button:hover{
        background-color: white;
        color: black;
        cursor:pointer;
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

    @media screen and (max-width:768px){
        .menu{
            width: 90dvw;
            transform: translateX(100vw);
        }
        .menu-head{
            width: 90dvw;
        }
        .open{
        transform: translateX(0vw);
        transition: 1s;
        }
        .menu-links{
            width:100dvw;
        }
        .menu-link{
            width: 95dvw;
        }
        .qr-code img{
            width:50dvw;
        }
    }
</style>

<slot></slot>