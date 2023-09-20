<script>
    import Padding from "../sd-pad-top.svelte";

    export let left = false;
    export let right = false;
</script>

<div class="container {right ? 'right' : ''}">
    <div class="time-grid">
        <div>2022 至今</div>
        <div class="name"><strong>单晶高镍三元正极材料的制备及其电化学性能研究</strong></div>
    </div>
    <Padding pad="0.25" />
    <div class="{left ? 'left' : ''}">
        <div class="resp">探究单晶高镍三元正极材料的晶体性质对于设计和开发高性能锂离子正极材料的影响。</div>
        <div class="contribs">
            <ul>
                <li>通过水热法、共沉淀法、溶胶凝胶法等合成单晶高镍三元正极材料。</li>
                <li>对比多种工艺下制备出的单晶高镍三元正极材料的形貌与电化学性能。</li>
            </ul>
        </div>
    </div>
</div>

<style>
    .time-grid {
        display: grid;
        grid-template-columns: 15% auto;
    }

    ul {
        list-style: square;
        padding-left: 13px;
    }

    li {
        padding-top: 0.5em;
    }

    .left {
        border-right: 1px solid #aaa;
        padding-right: 0.5cm;
    }

    .right {
        padding-left: 0.5cm;
    }
</style>
