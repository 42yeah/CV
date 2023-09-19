<script>
    import GamerTag from "./gamertag.svelte";
</script>

<div class="tag-container">
    <GamerTag name="C++" prof="熟练" />
    <GamerTag name="OpenGL" prof="熟练" />
    <GamerTag name="Python" prof="熟练" />
    <GamerTag name="JavaScript" prof="熟练" />
    <GamerTag name="CUDA" prof="熟悉" />
    <GamerTag name="Vulkan" prof="熟悉" />
    <GamerTag name="Eigen" prof="熟悉" />
    <GamerTag name="Lua" prof="熟悉" />
    <GamerTag name="Metal" prof="了解" />
    <GamerTag name="DirectX" prof="了解" />
    <GamerTag name="雅思" prof="8 分" />
</div>

<style>
    .tag-container {
        display: flex;
        row-gap: 0.1cm;
        flex-wrap: wrap;
        column-gap: 0.1cm;
    }
</style>
