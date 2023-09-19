<script>
    import testImg from "$lib/res/Test.svg";
    import callImg from "$lib/res/Call.svg";
    import emailImg from "$lib/res/EmailAddressViewer.svg";
    import webImg from "$lib/res/Web.svg";
</script>

<div class="flex-table">
    <div class="flex-cell">
        <img src={testImg}>
        <div class="flex-text">广州大学</div>
    </div>
    <div class="flex-cell">
        <img src={emailImg}>
        <div class="flex-text">hey@42yeah.is</div>
    </div>
    <div class="flex-cell">
        <img src={callImg}>
        <div class="flex-text">(+86) 13423211159</div>
    </div>
    <div class="flex-cell">
        <img src={webImg}>
        <div class="flex-text">blog.42yeah.is</div>
    </div>
</div>

<style>
    * {
        font-family: "Source Hans Sans";

    }

    img {
        height: 20px;
        padding-right: 0.2cm;
    }

    .flex-table {
        display: grid;
        grid-template-columns: 7cm auto;
    }

    .flex-cell {
        display: flex;
        align-items: center;
        padding-top: 0.1cm;
    }
</style>
