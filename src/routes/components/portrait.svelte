<script>
    import portrait from "$lib/res/portrait.jpg";
</script>

<div class="portrait-container">
    <div style="background-image: url({portrait})"></div>
</div>

<style>
    .portrait-container {
        position: absolute;
        right: 1cm;
        top: 1cm;
    }

    .portrait-container div {
        width: 3cm;
        height: 4cm;
        background-size: cover;
    }
</style>
