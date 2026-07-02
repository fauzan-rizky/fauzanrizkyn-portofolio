<script>
    import "../global.css";
    import svelteLogo from "../lib/images/svelte.webp"
    import linuxLogo from "../lib/images/Tux.svg"
    import pythonLogo from "../lib/images/python.webp"
    import gitLogo from "../lib/images/gitlogo.webp"

    import azuma from "../lib/images/azuma.webp"
    import fauzan from "../lib/images/ojanhacker.webp"
</script>

<div class="sections">
<div id="Home">
        <div id="Identity" class="halfLR">
            <div class="halfUD">
                <h1 class="slideLRYellow">FAUZAN RIZKY NAUFAL</h1>
                <h6 id="barcode" class="slideLRYellow">FAUZAN RIZKY NAUFAL</h6>
                <p>A.K.A.</p>
                <div class="badge-container">
                    <span class="badge-items">Ojan</span>
                    <span class="badge-items">福田 直人 (Fukuda Naoto)</span>
                    <span class="badge-items">刘发谅 (Liu Fa Liang)</span>
                </div>
            </div>
            <div id="job" class="halfUD">
                <h3 class="slideLRYellow">(future) Data Scientist</h3>
                <p>Specializations</p>
                <div class="badge-container">
                    <span id="ds-badge" class="badge-items">Data Science</span>
                    <span id="ml-badge" class="badge-items">Machine Learning</span>
                    <span id="frontend-badge" class="badge-items">Frontend</span>
                </div>
                <p>Skills</p>
                <div id="techs-container">
                    <img class="techs-logo" src={svelteLogo} alt="">
                <img class="techs-logo" src={pythonLogo} alt="">
                <img class="techs-logo" src={linuxLogo} alt="">
                <img class="techs-logo" src={gitLogo} alt="">
                </div>
                
            </div>
        </div>
        <div id="profile-container" class="halfLR">
            <div id="profile">
                <img id="azuma" src={azuma} alt="">
                <img id="fauzan" src={fauzan} alt="">
            </div>
        </div>
    </div>
</div>
    

<style>
    h1, h3, h6, p {
        width: fit-content;
    }
    #Home {
        display: flex;
        width: 75%;
        height: 65%;

        max-width: 1440px;
        max-height: 810px;
    }

    #barcode {
        font-family: "Libre Barcode 128", system-ui;
        font-weight: 500;
    }

    #Identity {
        display: flex;
        flex-direction: column;
    }
    
    #job {
        display: flex;
        flex-direction: column;
    }
   
    #profile-container {
        display: flex;
        justify-content: end;
        width: 50%;
    }

    #profile {
        width: 25vw;
        height: 25vw;
        position: relative;
        display: flex;
        align-items: center;
        justify-content: center;
        transition: all 0.1s linear;
        
    }

    #profile:hover {
        scale: 1.1
    }

    img {
        width: 100%;
    }

    #fauzan, #azuma {
        position: absolute;
        border: 3px solid rgb(255, 230, 0);
        border-radius: 15px;
    }

    #fauzan {
        z-index: 1;
    }

    #azuma {
        transition: all 0.2s ease-in;
        z-index: 2;
    }

    #azuma:hover {
        opacity: 0;
    }

    #techs-container {
        display: flex;
    }
    
    .techs-logo {
        width: 10%;
    }

    .slideLRYellow {
        background-color: black;
        position: relative;
    }

    .slideLRYellow::before {
        content: "";
        position: absolute;
        right: 0;
        top: 0;
        width: 100%;
        height: 90%;
        background-color: yellow;
        z-index: 2;

        animation: slideYellow 0.5s ease-out;
        animation-delay: 0.15s;
        animation-fill-mode: forwards;
    }

    @keyframes slideYellow {
        0% {
            width: 100%;
        }

        100% {
            width: 0%;
        }
    }

</style>
