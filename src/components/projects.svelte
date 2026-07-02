<div id="projects" class="sections">
    <div id="projects-front">
        <h1>Projects</h1>
        <div class="projects-container">
            <div id="nethack" class="projects-entry">Nethack</div>
            <div class="projects-entry"></div>
            <div class="projects-entry"></div>
            <div class="projects-entry"></div>
            <div class="projects-entry"></div>
  
        </div>
    </div>
</div>

<style>
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
        height: 20vh;

        max-width: 384px;
        max-height: 216px;

        border: 3px solid rgb(0, 255, 242);
        
        display: flex;
        align-items: center;
        justify-content: center;
        
    }

    .projects-entry:hover {
        scale: 1.1;
    }

    #nethack {
        background: url("../lib/images/nethack.webp");
        background-size: cover;
    }

    h1 {
        text-align: center;
    }
</style>

