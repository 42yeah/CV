<script>
    import Padding from "./sd-pad-top.svelte";
    import Title from "./title.svelte";
</script>

<div>
    <Title>教育经历</Title>
    <Padding pad="0.25" />

    <div class="left">
        <div class="edu-table">
            <div class="edu-cell">
                2021
            </div>
            <div class="edu-cell">
                <strong>广州大学</strong> 计算机技术
            </div>
            <div class="edu-cell">
                2017-2021
            </div>
            <div class="edu-cell">
                <strong>东莞理工学院</strong> 计算机科学与技术
            </div>
        </div>
    </div>
</div>

<style>
    .edu-table {
        display: grid;
        grid-template-columns: 30% auto;
        border-right: 1px solid #ccc;
        border-bottom: 1px solid #ccc;
        width: 300px;
    }

    .left {
        border-right: 1px solid #aaa;
    }

    .edu-cell {
        padding: 3px 5px;
        border-left: 1px solid #ccc;
        border-top: 1px solid #ccc;
    }
</style>

