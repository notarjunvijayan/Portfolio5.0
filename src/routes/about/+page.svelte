<div class="container">
    <div class="content">
        <div class="url">
            \ about
        </div>
        <div class="about">
            <div class="about-text">
                <p>I'm Arjun Vijayan, a passionate Full Stack Web Developer who thrives on turning ideas into digital realities.</p>
                <p>When I am not making websites, I play competitive online fps shooters.</p>   
                <p>Wanna Get in Touch? Click the buttons below to get my resume or Contact me</p>
                <button>Get Resume</button>
                <button>Contact</button>
            </div>
            <div class="about-image">
            </div>
        </div>
        <div class="education">
            <h2>EDUCATION</h2>
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
    .about{
        height: 75dvh;
        display: flex;
        padding: 3rem 0;
        align-items: center;
    }
    .about-text{
        font-family: Aeonik;
        font-size: 1.5rem;
        width:45rem;
        line-height: 2rem;
    }
    .education{
        width: 90dvw;
        height: 75dvh;
        background-color: #FF6F00;
        margin-top:3rem;
        padding: 3rem;
    }
    .education h2{
        font-family: mono;
        color: #101010;
        font-size: 4rem;
    }
    .lines{
        position:absolute;
        width: 100dvw;
        height: 250dvh;
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