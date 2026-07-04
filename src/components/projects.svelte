<div id="projects" class="sections">
    <div id="projects-front">
        <h1>Projects</h1>
        <div class="projects-container">
            <a target="_blank" href="https://github.com/fauzan-rizky/nethack">
                <div class="projects-entry">
                    <div id="nethack" class="projects-bg"></div>
                    <div class="projects-desc">
                        <p class="projects-desc-text projects-title">Nethack</p>
                        <span class="badge-techs">Python</span>
                        <p class="projects-desc-text">
                            just for fun "plug and get info" hacking tool I made,
                            utilizes windows basic network commands and python to get wifi
                            passwords, locating IP, and ARP scraping with scapy
                        </p>
                    </div>
                </div>
            </a>
            <a target="_blank" href="https://scefco.pages.dev">
                <div class="projects-entry">
                    <div id="scefco" class="projects-bg"></div>
                    <div class="projects-desc">
                        <p class="projects-desc-text projects-title">Scefco</p>
                        <span class="badge-techs">AstroJS</span>
                        <p class="projects-desc-text">
                            A school competition landing page website I made voluntarily for viewing
                            the events, competitions aswell as the guidebooks, contacts and more
                        </p>
                    </div>
                </div>
            </a>
            <a target="_blank" href="https://nusantarapathway.id">
                <div class="projects-entry">
                    <div id="nusantarapathway" class="projects-bg"></div>
                    <div class="projects-desc">
                        <p class="projects-desc-text projects-title">
                            Nusantara Pathway
                        </p>
                        <span class="badge-techs">SvelteJS</span>
                        <p class="projects-desc-text">
                            An academic tutoring landing page website I'm currently working on 
                        </p>
                    </div>
                </div>
            </a>

            <div class="empty-projects projects-entry"></div>
            <div class="empty-projects projects-entry"></div>
            <div class="empty-projects projects-entry"></div>
        </div>
    </div>
</div>

<style>
    a,
    a:link,
    a:visited,
    a:hover,
    a:active {
        color: inherit;
        text-decoration: none;
    }

    h1 {
        padding: 10px 0 10px 0;
    }

    #projects {
        height: fit-content;
    }
    #projects-front {
        width: 75%;
        height: 100%;

        max-width: 1440px;
        padding: 50px 0 50px 0;
    }

    .projects-container {
        display: grid;
        align-items: center;
        justify-content:space-around;
        align-content: space-between;
        row-gap: 50px;
        grid-template-columns: repeat(3, auto);
        height: fit-content;
    }

    .projects-entry {
        width: 20vw;
        height: 40vh;

        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        transition: all 0.5s ease-out;
        padding: 5px;
        border: 2px solid var(--secondaryColor);

        z-index: 2;
    }

    .projects-bg {
        width: 100%;
        height: 45%;
    }

    .projects-desc {
        width: 100%;
        height: 55%;
        background-color: black;
    }

    .projects-desc-text {
        font-size: 20px;
        font-weight: 500;
        text-align: justify;
        padding: 3px;
    }

    .badge-techs {
        display: inline-block;
        padding: 3px 6px;
        margin: 3px 0px 3px 0px;
        border: 3px solid var(--secondaryColor);
        font-size: 1rem;
        font-weight: 700;
        color: var(--secondaryColor);
        white-space: nowrap;
    }

    .projects-title {
        font-weight: 700;
        color: var(--secondaryColor);
    }

    .projects-entry:hover {
        scale: 1.1;
    }

    .empty-projects {
        display: none;
    }

    #nethack {
        background: url("../lib/images/nethack.webp");
        background-size: cover;
    }

    #scefco {
        background: url("../lib/images/scefco.webp");
        background-size: cover;
    }

    #nusantarapathway {
        background: url("../lib/images/nusantarapathway.png");
        background-size: cover;
    }

    h1 {
        text-align: center;
    }
</style>
