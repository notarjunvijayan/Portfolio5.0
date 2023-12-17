<div class="container">
    <div class="hero">
        <div class="hero-text">
            <p>I'm a</p>
            <h1><span class="orange">WEB</span></h1>
            <h1>DEVELOPER</h1>
        </div>
    </div>
    <div class="links">
        <a href="/about">About</a>
        <a href="/projects">Projects</a>
        <a href="/contact">Contact</a>
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
        height: 70dvh;
        display: flex;
        align-items: center;
        justify-content: center;
    }
    .hero-text{
        text-align: center;
    }
    h1{
        font-family: mono;
        font-size: 7rem;
        margin: 0;
        line-height: 9rem;
        font-weight: 500;
    }
    .links{
        display: flex;
        flex-direction: column;
        align-items: end;
        padding: 0 3dvw;
        height: 2dvh;
    }
    .links a{
        text-decoration: none;
        color: white;
        font-family: mono;
        font-size: 1.5rem;
    }
    .container{
        background: transparent;
        color:white;
        padding-top: 10vh;
        height: 100vh;
        z-index: 0;
    }
</style>