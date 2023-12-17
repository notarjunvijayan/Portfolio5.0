<script>
    let entered = true
</script>

<div class="loader" class:active = {entered === true}>
    <div class="loader-text">
        <h1>ARJUN VIJAYAN</h1>
        <p>Portfolio Webpage</p>
        <button 
        on:click={()=>{
            entered = true
            }}
        >Enter
        </button>
    </div>
    <div class="loader-lines">
        <hr/>
        <hr/>
        <hr/>
        <div class="background loader-bg">
            <div class="noise"></div>
        </div>
    </div>
</div>
<div class="container">
    <div class="hero">
        <div class="hero-text">
            <h1><span class="orange">WEB</span></h1>
            <h1>DEVELOPER</h1>
        </div>
    </div>
    <div class="bottom">
        <div class="home-text">
            <p>Hi :)</p>
            <p>Welcome to my portfolio webpage, where I talk about me and showcase my projects</p>
            <p>Start now by navigating from the links given</p>
        </div>
        <div class="links">
            <a href="/about">About</a>
            <a href="/projects">Projects</a>
            <a href="/contact">Contact</a>
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
    .active{
        transform: translateY(-100vh);
        transition: 1.5s ease-in-out;
    }
    .loader{
        position: absolute;
        width: 100dvw;
        height: 100dvh;
        display: flex;
        align-items: center;
        justify-content: center;
        background: transparent;
    }
    .loader-text{
        z-index:2;
    }
    .loader-lines{
        position: absolute;
        background-color: #FF6F00;
        width: 100vw;
        height: 100vh;
        top: 0;
        left: 0;
        z-index: 1;
        display: flex;
    }
    .loader-lines hr{
        position: relative;
        width:1px;
        border: none;
        background-color:rgba(0, 0, 0);
        opacity: 0.3;
        
    }
    .loader h1{
        font-size: 8rem;
    }
    .loader p{
        font-size: 2rem;
    }
    .loader-text{
        text-align: center;
    }
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
    .orange{
        color: #FF6F00;
    }
    .hero{
        height: 60dvh;
        display: flex;
        align-items: center;
        justify-content: center;
    }
    .hero-text{
        text-align: center;
    }
    .home-text{
        display: flex;
        flex-direction: column;
        justify-content: center;
        height: 30dvh;
    }
    h1{
        font-family: mono;
        font-size: 10rem;
        margin: 0;
        line-height: 11rem;
        font-weight: 500;
    } 
    p{
        font-family: aeonik;
        line-height: 0.5rem;
        font-size: 1.2rem;
    }
    .bottom{
        display: flex;
        align-items: center;
        justify-content: space-between;
        padding: 0 3dvw;
        height: 30dvh;
    }
    .links{
        display: flex;
        flex-direction: column;
        align-items: end;
    }
    .links a{
        text-decoration: none;
        color: white;
        font-family: mono;
        font-size: 1.5rem;
        line-height: 3rem;
    }
    a:hover{
        color:#FF6F00;
    }
    .container{
        inset: 4;
        color:white;
        padding-top: 10vh;
        height: 90dvh;
        z-index: 0;
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