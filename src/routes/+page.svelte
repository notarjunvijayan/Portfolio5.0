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
        width:0.5px;
        border: 1px solid rgba(255, 255, 255, 0.125);
    }
    .orange{
        color: #FF6F00;
    }
    .hero{
        height: 50dvh;
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
        height: 40dvh;
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
        height: 40dvh;
    }
    .links{
        display: flex;
        flex-direction: column;
        align-items: end;
        height: 2dvh;
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
        background: transparent;
        color:white;
        padding-top: 10vh;
        height: 90dvh;
        z-index: 0;
    }
</style>