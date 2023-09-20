<script>
    import qrImg from "$lib/res/wenqr.jpg";
</script>

<div class="qr-container">
    <img src={qrImg}>
</div>

<style>
    .qr-container {
        position: absolute;
        right: 4.2cm;
        top: 1cm;
    }

    .qr-container img {
        width: 2cm;
        height: 2cm;
    }
</style>
