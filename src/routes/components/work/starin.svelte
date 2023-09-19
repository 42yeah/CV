<script>
    import Padding from "../sd-pad-top.svelte";

    export let left = false;
    export let right = false;
</script>

<div class="container {right ? 'right' : ''}">
    <div class="time-grid">
        <div>2023</div>
        <div class="name"><strong>独立承包</strong>，广州星印国际物流有限公司</div>
    </div>
    <Padding pad="0.25" />
    <div class="{left ? 'left' : ''}">
        <div class="resp">使用 Svelte 负责完整的物流系统的前端制作，包括入出库，开具收据，物流查询。</div>
        <div class="contribs">
            <ul>
                <li>利用 NGINX 进行路由、SSL 证书、和反向代理管理。</li>
                <li>通过 PDF.js 从前端直接操控打印内容，并对多个移动浏览器做适配，解决了电子收据的打印难点。</li>
                <li>交付时，系统涵盖范围从供应商填写、仓库入库、库存管理直到货物出仓，满足完整物流系统的需求。</li>
            </ul>
        </div>
    </div>
</div>

<style>
    .time-grid {
        display: grid;
        grid-template-columns: 30% auto;
    }

    ul {
        list-style: square;
        padding-left: 13px;
    }

    li {
        padding-top: 0.5em;
    }

    .left {
        border-right: 1px solid #aaa;
        padding-right: 0.5cm;
    }

    .right {
        padding-left: 0.5cm;
    }
</style>
