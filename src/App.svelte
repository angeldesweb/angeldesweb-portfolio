<script>
    import github from './images/github.svg';
    import twitter from './images/twitter.svg';
    import instagram from './images/instagram.svg';
    import facebook from './images/facebook.svg';
    import linkedin from './images/linkedin.svg';
</script>

<div class="app">
    <div class="container">
        <header>
            <h1>Angel Zamora</h1>
        </header>
        <div class="content">
            <p>Disculpe la molestia.</p>
            <hr>
            <span>Este sitio se encuentra actualmente en mantenimiento.</span>
            <a class="button" href="https://www.dropbox.com/s/gr2u0amwu3we8dn/CURRICULUM_ANGEL.pdf?dl=1" target="blank">Descargar CV de Ángel Zamora</a>
        </div>
        <div class="media">
            <a href="https://github.com/angeldesweb" target="blank" class="social github">
                <img src={github} alt="">
            </a>
            <a href="https://www.facebook.com/angeldesweb" target="blank" class="social facebook">
                <img src={facebook} alt="">
            </a>
            <a href="https://www.instagram.com/angeldesweb/" target="blank" class="social instagram">
                <img src={instagram} alt="">
            </a>
            <a href="https://twitter.com/angeldesweb1" target="blank" class="social twitter">
                <img src={twitter} alt="">
            </a>
            <a href="https://www.linkedin.com/in/%C3%A1ngel-zamora-b42982133" target="blank" class="social linkedin">
                <img src={linkedin} alt="">
            </a>
        </div>
    </div>
</div>

<style>
    @media screen and (orientation:landscape) {
        h1 {
            font-size:8vw;        
        }
        header {
            height:25%;
        }
    }

    @media screen and (orientation:portrait) {
        h1 {
            font-size:8vh;
            margin-top:1em;        
        }
        header {
            height:15%;
        }
    }

    .app {
        width:100vw;
        height:100vh;
        background-image: url('./images/background.jpg');
        background-size: cover;
        background-position: top center;
    }
    .container {
        background-color: rgba(0, 0, 0, 0.596);
        width:100%;
        height: 100%;
        position:relative;
        padding:0 .5em;
    }
    header {
        background-color: rgba(0, 0, 0, 0.25);        
        display:flex;
        justify-content: center;
        backdrop-filter: blur(4px);
        -webkit-backdrop-filter: blur( 4px );
        border: 1px solid rgba( 255, 255, 255, 0.18 );
    }

    header > h1 {
        font-family: 'gogh';
        font-size: 8vw;
        width:100%;
        text-align:center;
        background-image: url('./images/background.jpg');
        background-size: cover;
        background-position-y:top;
        color:transparent;
        background-clip: text;
        -webkit-background-clip: text;
    }

    .content {
        width:min(30rem,100%);
        background: rgba( 0, 0, 0, 0.25 );
        box-shadow: 0 8px 32px 0 rgba( 31, 38, 135, 0.37 );
        backdrop-filter: blur( 4px );
        -webkit-backdrop-filter: blur( 4px );
        border-radius: 10px;
        border: 1px solid rgba( 255, 255, 255, 0.18 );
        margin: 3em auto;
        color:#fff;
        display:grid;
        place-content:center;
        padding:1em;
        font-family: Arial, Helvetica, sans-serif;
    }

    .content > p {
        text-align: center;
        font-weight: lighter;
        font-size: 1.5em;
        margin-bottom:.5em;
    }
    .content > span {
        margin-top:.5em;
        font-size:1em;
    }
    .button {
        text-align:center;
        text-decoration: none;
        background: rgba( 255, 255, 255, 0.25 );
        box-shadow: 0 8px 32px 0 rgba( 31, 38, 135, 0.37 );
        backdrop-filter: blur( 4px );
        -webkit-backdrop-filter: blur( 4px );
        border-radius: 10px;
        border: 1px solid rgba( 255, 255, 255, 0.18 );
        margin-top:1em;
        padding:.5em;
        color:rgb(174, 174, 174);
    }

    .button:hover {
        backdrop-filter: blur( 10px );
        -webkit-backdrop-filter: blur( 10px );
        color:#fff;
        font-weight: bolder;
    }
    .social {
        backdrop-filter: blur(5px);
        border: 1px solid rgba( 255, 255, 255, 0.18 );
        border-radius: 10px;
        padding:.5em;
        cursor:pointer;
        height:4rem;
        width:4rem;
        display:grid;
        place-content: center;
    }

    .social:hover {
        backdrop-filter: blur(3px);
        box-shadow: 3px 3px 2px 0px rgba(111, 111, 111, 0.75);
        -webkit-box-shadow: 3px 3px 2px 0px rgba(111, 111, 111, 0.75);
        -moz-box-shadow: 3px 3px 2px 0px rgba(111, 111, 111, 0.75);
    }

    img {
        height: 3rem;
        width: 3rem;
        background-color: transparent;
        filter: saturate(0%) opacity(29%) contrast(0%);
        -webkit-filter: saturate(0%) opacity(29%) contrast(0%);
        -moz-filter: saturate(0%) opacity(29%) contrast(0%);
    }

    .media {
        background-color: rgba(0, 0, 0, 0.25);
        display:flex;
        justify-content: space-around;
        gap:1em;
        flex-wrap:wrap;
        backdrop-filter: blur(4px);
        border: 1px solid rgba( 255, 255, 255, 0.18 );
        margin-bottom:0;
        position:absolute;
        left:.5em;
        right:.5em;
        bottom:0;
        padding:1em;
    }
</style>
