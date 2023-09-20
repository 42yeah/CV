<script>
    import Padding from "../sd-pad-top.svelte";

    export let left = false;
</script>

<div class="container">
    <div class="time-grid">
        <div>2022.06 - 至今</div>
        <div class="name"><strong>科研助理</strong>，广州理文科技有限公司</div>
    </div>
    <Padding pad="0.25" />
    <div class="{left ? 'left' : ''}">
        <div class="resp">独立承担整个项目工作，负责锂离子电池的商业硅碳负极，主要对首效与循环问题进行改性。</div>
        <div class="contribs">
            <ul>
                <li>探究不同商业硅碳负极的合成条件、合成手段、碳源、硅源种类对硅碳负极性能的影响。</li>
                <li>研发应用于锂离子电池的商业硅碳负极。 </li>
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
