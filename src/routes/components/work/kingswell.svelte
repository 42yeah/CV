<script>
    import Padding from "../sd-pad-top.svelte";

    export let left = false;
</script>

<div class="container">
    <div class="time-grid">
        <div>2018-2019</div>
        <div class="name"><strong>实习生</strong>，深圳金思维实业有限公司</div>
    </div>
    <Padding pad="0.25" />
    <div class="{left ? 'left' : ''}">
        <div class="resp">用 C++/MFC 在郑州市东⻛日产厂内负责整个二号流水线的轮胎机器人流水线系统的制作。</div>
        <div class="contribs">
            <ul>
                <li>使用 UDP socket 编程，通过跟踪包 ID 实现跟总控的无连接稳定数据传输。</li>
                <li>通过 OPC 协议控制 PLC 机器臂，原本的单一安装方式改进为了可高度自定义的轮胎安装。</li>
                <li>利用 MFC 和 Win32 接口制作上位机用戶界面。</li>
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

</style>
