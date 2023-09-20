<script>
    import Padding from "../sd-pad-top.svelte";

    export let left = false;
    export let right = false;
</script>

<div class="container {right ? 'right' : ''}">
    <div class="time-grid">
        <div>2022-2023</div>
        <div class="name"><strong>Dogshit</strong></div>
    </div>
    <Padding pad="0.25" />
    <div class="{left ? 'left' : ''}">
        <div class="resp">研究锂离子电池负极集流体结构性能及电化学性能测试方法及规范。</div>
        <div class="contribs">
            <ul>
                <li>负责对集流体进行微观结构表征。</li>
                <li>测试集流体纵向和横向拉伸长度及极片材料剥离强度。</li>
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
