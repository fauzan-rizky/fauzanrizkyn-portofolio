<div id="projects" class="sections">
    <div id="projects-front">
        <h1>Projects</h1>
        <div class="projects-container">
        <a target="_blank" href="https://github.com/fauzan-rizky/nethack">
        <div class="projects-entry">
                <div id="nethack" class="projects-bg"></div>
                <div class="projects-desc">
                    <p class="projects-desc-text projects-title">Nethack</p>
                    <p class="projects-desc-text">Network diagnostic tool</p>
                    <p class="projects-desc-text">Tech Stack: Python, Nuitka</p>
                    <p class="projects-desc-text">Status: Finished</p>
                </div>
            </div>
        </a>
        <a target="_blank" href="https://scefco.pages.dev">
        <div class="projects-entry">
                <div id="scefco" class="projects-bg"></div>
                <div class="projects-desc">
                    <p class="projects-desc-text projects-title">Scefco</p>
                    <p class="projects-desc-text">School competition website</p>
                    <p class="projects-desc-text">Tech Stack: AstroJS</p>
                    <p class="projects-desc-text">Status: Finished</p>
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
    a, a:link, a:visited, a:hover, a:active {
  color: inherit;
  text-decoration: none;
}
    #projects-front {
        width: 75%;
        height: 100%;

        max-width: 1440px;
    }

    .projects-container {
        display: grid;
        align-items: center;
        justify-content: space-between;
        grid-template-columns: repeat(3, auto);
        height: 75%;
    }

    .projects-entry {
        width: 20vw;
        height: 30vh;

        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        transition: all 0.5s ease-out;
        padding: 5px;
        border: 2px solid var(--secondaryColor);
    }

    .projects-bg {
        width: 100%;
        height: 60%;
    }

    .projects-desc {
        width: 100%;
        height: 40%;
        background-color: black;
    }

    .projects-desc-text {
        font-size: 20px;
        font-weight: 500;
    }

    .projects-title {
        font-weight: 700;
        color: var(--secondaryColor);
    }

    .projects-entry:hover {
        scale: 1.1;
    }

    .empty-projects {
        opacity: 0;
    }

    #nethack {
        background: url("../lib/images/nethack.webp");
        background-size: cover;
    }

    #scefco {
        background: url("../lib/images/scefco.webp");
        background-size: cover;
    }

    h1 {
        text-align: center;
    }
</style>
