<script>
    import portrait from "$lib/res/portrait.jpeg";
</script>

<div class="portrait-container">
    <img src={portrait}>
</div>

<style>
    .portrait-container {
        position: absolute;
        right: 1cm;
        top: 1cm;
    }

    .portrait-container img {
        width: 3cm;
        height: 4cm;
    }
</style>
