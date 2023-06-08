<script>
    export let icon = "/icon.png";
    export let url = "https://clamp-project.vercel.app/";
</script>

<a href={url}>
    <button>
        <img src={icon} alt="LinkIcon" />
        <slot />
    </button>
</a>

<style>
    a {
        text-decoration: none;
    }
    button {
        padding: 12px;
        background: transparent;
        color: white;
        font-size: 30px;
        cursor: pointer;

        display: flex;
        flex-direction: row;
        align-items: center;
    }
    img {
        height: 60px;
        margin-right: 8px;
    }
</style>
