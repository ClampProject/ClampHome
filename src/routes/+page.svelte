<script>
    import LinkButton from "$lib/LinkButton/Button.svelte";
</script>

<div class="main">
    <div style="margin-top: 16px;" />
    <div class="branding">
        <img src="/icon.png" alt="Clamp Logo" class="logo" />
        <div class="line" style="height:64px;margin:8px" />
        <h1 class="brandname">Clamp</h1>
    </div>

    <p class="colorful welcome">Hello there! Welcome to Clamp!</p>
    <p>
        We are a very (very (very)) small team making cool stuff for you to try
        out!
    </p>
    <div class="line" style="width:80%;" />
    <h2>Tools for people (or robots if you tried hard enough)</h2>

    <LinkButton icon="/icons/coding.png" url="https://clamp-coding.vercel.app/">
        Clamp Coding
    </LinkButton>
    <p>nah bruh fr only one tol?</p>

    <div class="line" style="width:80%;" />
    <div style="margin-top: 16px;" />
    <a href="https://github.com/ClampProject" target="_blank">
        GitHub Organization
    </a>
</div>

<style>
    @keyframes rainbowTextColor {
        0% {
            color: rgb(255, 117, 117);
        }
        25% {
            color: rgb(255, 253, 117);
        }
        50% {
            color: rgb(117, 255, 124);
        }
        75% {
            color: rgb(117, 172, 255);
        }
        100% {
            color: rgb(211, 117, 255);
        }
    }

    .main {
        display: flex;
        flex-direction: column;
        align-items: center;
        width: 100%;
    }
    .logo {
        width: 96px;
    }
    .line {
        width: 1px;
        height: 1px;
        background: rgba(255, 255, 255, 0.25);
        margin: 4px;
    }
    .branding {
        display: flex;
        flex-direction: row;
        align-items: center;
    }
    .brandname {
        /* this class name makes it sound proffesional */
        /* we are not  */
        margin-block: 0px;
        font-size: 64px;
    }

    .colorful {
        color: aqua;
        animation: rainbowTextColor 2s linear 0s infinite normal;
        margin-block-end: 4px;
    }
    .welcome {
        font-size: 24px;
    }
</style>
