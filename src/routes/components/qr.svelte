<script>
    import qrImg from "$lib/res/peneqr.png";
</script>

<div class="qr-container">
    <img src={qrImg}>
</div>

<style>
    .qr-container {
        position: absolute;
        right: 1cm;
        top: 1cm;
    }

    .qr-container img {
        width: 2cm;
        height: 2cm;
    }
</style>
