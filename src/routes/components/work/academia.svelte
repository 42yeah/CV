<script>
    import Padding from "../sd-pad-top.svelte";

    export let left = false;
</script>

<div class="container">
    <div class="time-grid">
        <div>2021 - 至今</div>
        <div class="name"><strong>钠离子电池层状氧化物正极材料的制备及改性研究</strong>，广州大学能源催化研究所</div>
    </div>
    <div class="{left ? 'left' : ''}">
        <div class="contribs">
            <ul>
                <li>查阅相关文献，设计P2型和O3型层状氧化物合成方法及改性方案，并独立完成专利与实验研究性论文的撰写。</li>
                <li>负责分析电化学性能数据与结构表征，探究电池正极材料储能机理，失效原因等。</li>
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
