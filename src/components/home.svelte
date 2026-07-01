<script>
    import "../global.css";
    import Sections from "./sections.svelte";
</script>

<Sections>
    <div id="Home">
        <div id="Identity" class="halfLR">
            <div class="halfUD">
                <h1>FAUZAN RIZKY NAUFAL</h1>
                <p>A.K.A.</p>
                <div class="badge-container">
                    <span class="badge-items">Ojan</span>
                    <span class="badge-items">福田 直人 (Fukuda Naoto)</span>
                    <span class="badge-items">刘发谅 (Liu Fa Liang)</span>
                </div>
            </div>
            <div class="halfUD">
                <h3>(Future) Data Scientist</h3>
                <p>Specializations</p>
                <div class="badge-container">
                    <span id="ds-badge" class="badge-items">Data Science</span>
                    <span id="ml-badge" class="badge-items">Machine Learning</span>
                    <span id="frontend-badge" class="badge-items">Frontend</span>
                </div>
            </div>
        </div>
        <div class="halfLR"></div>
    </div>
</Sections>

<style>
    #Home {
        display: flex;
        width: 75%;
        height: 75%;
    }

    #Identity {
        display: flex;
        flex-direction: column;
    }
   

</style>
