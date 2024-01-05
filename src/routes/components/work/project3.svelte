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
        <div class="resp">探究单晶高镍三元正极材料的制备过程对于设计和开发高性能锂离子正极材料的影响。</div>
        <div class="contribs">
            <ul>
                <li>利用水热、共沉淀和溶胶凝胶法合成单晶高镍三元正极材料，探究其形貌与电化学性能。</li>
                <li>通过烧结过程后对单晶高镍三元正极材料进行晶体形貌表征，深入研究其晶体成型条件。</li>
            </ul>
        </div>
    </div>
</div>

<style>
    .time-grid {
        display: grid;
        grid-template-columns: 15% auto;
        padding-bottom: 0.5em;
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
