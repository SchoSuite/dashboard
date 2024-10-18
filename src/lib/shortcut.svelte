<script>
    export let text;
</script>

<button id="main">
    <div id="img"></div>
    <p id="txt">{text}</p>
</button>

<style>
    @import "/theme.css";

    #main {
        border: none;
        background-color: var(--bg2);
        text-align: center;
        transition: all, 0.5s;
        border-radius: 10px;
        aspect-ratio: 1 / 1;
        min-width: 50px;
        max-width: 50px;
        overflow: hidden;
        display: block;
        position: relative;
    }

    #main:hover {
        background-color: var(--bg1);
    }

    #main::before {
        content: "";
        position: absolute;
        left: 0;
        top: 50%;
        transform: translateY(-50%);
        width: 4px;
        height: 0%;
        background-color: var(--orange);
        border-radius: 2px;
        transition: all, 0.2s;
    }

    #main:hover::before {
        content: "";
        position: absolute;
        left: 0;
        top: 50%;
        transform: translateY(-50%);
        width: 4px;
        height: 60%;
        background-color: var(--orange);
        border-radius: 2px;
    }

    #main:active {
        transform: scale(0.8);
    }

    #img {
        width: 25px;
        height: 25px;
        background-color: var(--cyan);
        margin-left: auto;
        margin-right: auto;
        margin-bottom: -15px;
        margin-top: 5px;
        border-radius: 5px;
    }

    p {
        color: var(--fg2);
    }
</style>
