<div class="three-sep-container">
    <div class="three-sep">
        <slot />
    </div>
</div>

<style>
    .three-sep {
        display: grid;
        grid-template-columns: 33% 33% 33%;
    }
</style>
