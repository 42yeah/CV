<script>
    export let name;
    export let thumbnail;
    export let last;

    import Padding from "./sd-pad-top.svelte";
</script>

<div class="project-container {last ? 'last' : ''}">
    <div class="thumbnail">
        <img src={thumbnail}>
    </div>
    <h3 class="title">{name}</h3>
    <Padding pad="0.25" />
    <div class="desc">
        <slot />
    </div>
</div>

<style>
    .project-container {
        width: 100%;
    }

    .title {
        text-align: center;
    }

    .thumbnail {
        padding: 10px;
        display: flex;
        justify-content: center;
    }

    .thumbnail > img {
        border-radius: 5px;
        height: 3.2cm;
    }

    .desc {
        display: flex;
        padding: 10px;
    }
</style>
