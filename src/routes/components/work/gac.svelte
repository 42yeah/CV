<script>
    import Padding from "../sd-pad-top.svelte";

    export let left = false;
</script>

<div class="container">
    <div class="time-grid">
        <div>2023 至今</div>
        <div class="name"><strong>电池参数获取方法研究，广州汽车集团股份有限公司</strong></div>
    </div>
    <div class="{left ? 'left' : ''}">
        <div class="resp">负责和广汽研究院对接，统筹整个项目的管理和推进。</div>
        <div class="contribs">
            <ul>
                <li>负责建立电池参数的获取方法和测试数据的处理方法，并对参数结果进行一致性分析。</li>
                <li>与广汽研究院进行沟通和协调，为对方提供必要的技术咨询及支持。</li>
            </ul>
        </div>
    </div>
</div>

<style>
    .time-grid {
        display: grid;
        grid-template-columns: 15% auto;
        padding-bottom: 0.5em;
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

    .name {
        font-family: "Source Hans Sans";
    }

</style>
