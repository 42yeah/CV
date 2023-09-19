<div class="two-sep-container">
    <div class="two-sep">
        <slot />
    </div>
</div>

<style>
    .two-sep {
        display: grid;
        grid-template-columns: 50% 50%;
    }
</style>
