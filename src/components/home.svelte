<script>
    import "../global.css";
    import "../fonts.css";
    import svelteLogo from "../lib/images/svelte.webp";
    import linuxLogo from "../lib/images/Tux.svg";
    import pythonLogo from "../lib/images/python.webp";
    import gitLogo from "../lib/images/gitlogo.webp";

    import azuma from "../lib/images/azuma.webp";
    import fauzan from "../lib/images/ojanhacker.webp";

    import Slider from "./slider.svelte";
</script>

<div id="home" class="sections">
    <div id="Home">
        <div id="Identity" class="halfLR">
            <div id="profile-mobile-container">
                <div id="profile-mobile" class="mobile">
                    <img id="azuma" src={azuma} alt="" />
                    <img id="fauzan" src={fauzan} alt="" />
                </div>
            </div>

            <div class="halfUD name">
                <h1 class="slideLRYellow mainShadow">FAUZAN RIZKY NAUFAL</h1>
                <h6 id="barcode" class="slideLRYellow">FAUZAN RIZKY NAUFAL</h6>
                <p id="aka">A.K.A.</p>
                <div class="badge-container">
                    <span class="badge-items">Ojan</span>
                    <span class="badge-items">福田 直人 (Fukuda Naoto)</span>
                    <span class="badge-items">刘发谅 (Liu Fa Liang)</span>
                </div>
            </div>

            <div id="job" class="halfUD job">
                <h5 id="jobTitle" class="slideLRYellow mainShadow">
                    Informatics Engineering student at Politeknik Negeri Jakarta
                </h5>
                <div id="jobTitle-mobile">
                    <h5 class="jobpart slideLRYellow mainShadow">
                        Informatics Engineering student
                    </h5>
                    <h5 class="jobpart slideLRYellow mainShadow">at</h5>
                    <h5 class="jobpart slideLRYellow mainShadow">
                        Politeknik Negeri Jakarta
                    </h5>
                </div>
                <p>Specializations</p>
                <div class="badge-container">
                    <span id="ds-badge" class="badge-items">Data Science</span>
                    <span id="ml-badge" class="badge-items"
                        >Machine Learning</span
                    >
                    <span id="frontend-badge" class="badge-items">Frontend</span
                    >
                </div>
                <p>Skills</p>
                <div id="techs-container">
                    <img class="techs-logo" src={svelteLogo} alt="" />
                    <img class="techs-logo" src={pythonLogo} alt="" />
                    <img class="techs-logo" src={linuxLogo} alt="" />
                    <img class="techs-logo" src={gitLogo} alt="" />
                </div>
            </div>
        </div>
        <div id="profile-container" class="halfLR">
            <div id="profile" class="">
                <img id="azuma" src={azuma} alt="" />
                <img id="fauzan" src={fauzan} alt="" />
            </div>
        </div>
    </div>
</div>
<div class="slider">
    <p class="sliderText">
        PORTOFOLIO_PORTOFOLIO_PORTOFOLIO_PORTOFOLIO_PORTOFOLIO_PORTOFOLIO_PORTOFOLIO_PORTOFOLIO_PORTOFOLIO_PORTOFOLIO_
    </p>
    <p class="sliderText">
        PORTOFOLIO_PORTOFOLIO_PORTOFOLIO_PORTOFOLIO_PORTOFOLIO_PORTOFOLIO_PORTOFOLIO_PORTOFOLIO_PORTOFOLIO_PORTOFOLIO_
    </p>
</div>

<style>
    h1,
    h5,
    h6,
    p {
        width: fit-content;
    }

    #home {
        height: 95%;
    }

    .slider {
        display: flex;
        align-items: center;
        height: 5%;
        /* border-top: 1px solid var(--secondaryColor);
        border-bottom: 1px solid var(--secondaryColor); */
        padding: 1% 0 1% 0;
        color: var(--mainColor);
        width: fit-content;

        animation: slider 12.5s linear infinite;
    }

    .sliderText {
        font-weight: 600;
        animation: sliderText 2.5s ease-in infinite;
    }

    @keyframes slider {
        0% {
            transform: translateX(0);
        }

        100% {
            transform: translateX(-50%);
        }
    }

    @keyframes sliderText {
        0% {
            text-shadow: 0px 0px 0px var(--mainColor);
        }

        50% {
            text-shadow: 0px 0px 30px var(--mainColor);
        }

        100% {
            text-shadow: 0px 0px 0px var(--mainColor);
        }
    }

    #Home {
        display: flex;
        width: 75%;
        height: 75%;

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

    #jobTitle {
        font-weight: 600;
    }

    #jobTitle-mobile {
        display: none;
    }

    #profile-mobile-container {
        display: none;
    }

    #profile-container {
        display: flex;
        justify-content: end;
        width: 50%;
    }

    #profile {
        width: 25vw;
        height: 25vw;
        max-width: 480px;
        max-height: 480px;

        position: relative;
        display: flex;
        align-items: center;
        justify-content: center;
        transition: all 0.1s linear;
    }

    #profile:after {
        content: "";
        position: absolute;
        top: 10px;
        left: 10px;

        width: 100%;
        height: 100%;

        background-color: var(--mainColor);
    }

    #profile:hover {
        scale: 1.1;
    }

    img {
        width: 100%;
    }

    #fauzan,
    #azuma {
        position: absolute;
        width: 100%;
        height: 100%;
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
        background-color: black;
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

    @media only screen and (max-width: 720px) {
        .halfUD {
            text-align: center;
        }

        .name {
            height: 17.5%;
        }

        .job {
            height: 32.5%;
        }

        #barcode,
        #aka {
            display: none;
        }
        #azuma {
            display: none;
        }
        #profile-container {
            display: none;
        }

        .halfLR {
            width: 100%;
        }

        .badge-container {
            display: none;
        }

        #techs-container {
            justify-content: center;
        }

        p {
            text-align: center;
            width: 100%;
        }

        .slideLRYellow {
            height: 100%;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        #jobTitle-mobile {
            display: flex;
            flex-direction: column;
            align-items: center;
        }

        #jobTitle {
            display: none;
        }

        #profile-mobile-container {
            height: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        #profile-mobile {
            width: 50vw;
            height: 50vw;
            max-width: 480px;
            max-height: 480px;

            position: relative;
            display: flex;
            align-items: center;
            justify-content: center;
            transition: all 0.1s linear;
        }

        #profile-mobile:after {
            content: "";
            position: absolute;
            top: 10px;
            left: 10px;

            width: 100%;
            height: 100%;

            background-color: var(--mainColor);
        }

        #profile-mobile:hover {
            scale: 1.1;
        }

        img {
            width: 100%;
        }

        .jobpart {
            height: fit-content;
        }
    }
</style>
