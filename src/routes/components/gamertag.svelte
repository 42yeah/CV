<script>
    export let name;
    export let prof;
</script>

<div class="tag">
    <div class="name">
        {name}
    </div>
</div>

<style>
    .tag {
        border: 1px solid #aaa;
        display: flex;
    }

    .name {
        padding: 1px 10px;
    }

    .prof {
        background-color: #eaeaea;
        border-left: 1px solid #aaa;
        padding: 1px 10px;
    }
</style>
