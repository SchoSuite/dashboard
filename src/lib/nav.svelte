<div id="top">
    <div id="left">
        <button>Home</button>
        <button>About</button>
        <div id="separator"></div>
        <p>we can put a motivation quote here</p>
    </div>

    <div id="right">
        <button>Account</button>
    </div>
</div>

<style>
    @import "/theme.css";

    #top {
        display: flex;
        background-color: var(--bg2);
        position: fixed;
        width: 100%;
        left: 0px;
        top: 0px;
        border-top: 4px solid var(--green);
        box-shadow: 0px 0px 5px var(--black);
    }

    #left {
        flex: 50%;
        padding-left: 20px;
        align-items: center;
        display: flex;
    }

    #separator {
        display: inline-block;
        height: 20px;
        width: 1.5px;
        background-color: var(--fg2);
        margin-right: -5px;
    }

    #right {
        flex: 50%;
        text-align: right;
        padding-right: 20px;
    }

    #left,
    #right {
        padding-top: 10px;
        padding-bottom: 10px;
        gap: 10px;
    }

    p {
        display: inline;
        font-style: italic;
        font-size: 12px;
        color: var(--fg2);
    }

    button {
        margin: 0px;
        border: none;
        border-radius: 20px;
        padding: 10px;
        color: var(--fg1);
        background-color: var(--bg2);
        transition: all, 0.5s;
    }

    button:hover {
        background-color: var(--bg1);
    }

    button:active {
        transform: scale(0.8);
    }
</style>
