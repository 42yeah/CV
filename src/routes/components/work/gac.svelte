<script>
    import Padding from "../sd-pad-top.svelte";

    export let left = false;
</script>

<div class="container">
    <div class="time-grid">
        <div>2023 至今</div>
        <div class="name"><strong>电池参数获取方法研究，广汽研究院</strong></div>
    </div>
    <Padding pad="0.25" />
    <div class="{left ? 'left' : ''}">
        <div class="resp">负责废旧动力电池镍钴锰三元正极材料再生利用方法的设计研发。</div>
        <div class="contribs">
            <ul>
                <li>对废旧三元正极材料进行预处理条件探究。</li>
                <li>负责废旧三元正极材料再生工艺的条件设计及优化。</li>
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

</style>
