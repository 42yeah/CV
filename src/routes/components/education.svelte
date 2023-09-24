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
                2021 至今
            </div>
            <div class="edu-cell">
                <strong>广州大学</strong> 化学工程
            </div>
            <div class="edu-cell">
                2017-2021
            </div>
            <div class="edu-cell">
                <strong>广州大学</strong> 化学工程与工艺
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

    .edu-cell {
        padding: 3px 5px;
        border-left: 1px solid #ccc;
        border-top: 1px solid #ccc;
    }
</style>

