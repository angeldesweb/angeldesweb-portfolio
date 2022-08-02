
<div class="app">
    <a href="http://www.thismanslife.co.uk" target="_blank">AZ</a>
</div>

<style>


    .app {
        font-family: 'agero';
        height:100vh;
        background-color: rgb(47, 38, 38);
    }

    a {
        color: #c1da6e;
        text-shadow: 0 20px 25px #efeffa, 0 40px 60px #ffffff;
        font-family:'agero';
        font-size: 80px;
        font-weight: bold;
        text-decoration: none;
        letter-spacing: -3px;
        margin: 0;
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translateX(-50%) translateY(-50%);
    }

    a:before,a:after {
        content: '';
        padding: .9em .4em;
        position: absolute;
        left: 50%;
        width: 100%;
        top: 50%;
        display: block;
        border:10px solid red;
        /* border-top: 0;
        border-right:0; */
        border-radius:0 0 0 0;
        transform: translateX(-50%) translateY(-50%) rotate(0deg);
        animation: 10s infinite alternate ease-in-out tipsy;
    }

    a:before {
        border-color: #c1da6e #c1da6e rgba(0, 0, 0, 0) rgba(0, 0, 0, 0);
        z-index: -1;
    }

    a:after {
        border-color: rgba(0, 0, 0, 0) rgba(0, 0, 0, 0) #c1da6e #c1da6e;
        box-shadow: 25px 25px 25px rgba(243, 243, 243, 0.8);
    }  
    
    @keyframes tipsy {
        0% {
            transform: translateX(-50%) translateY(-50%) rotate(0deg);
        }
        100% {
            transform: translateX(-50%) translateY(-50%) rotate(360deg);
        }
    }
</style>