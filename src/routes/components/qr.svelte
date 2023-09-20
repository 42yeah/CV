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
        top: 5.2cm;
    }

    .qr-container img {
        width: 3cm;
        height: 3cm;
    }
</style>
