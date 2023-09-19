<script>
    import NameTag from "./components/nametag.svelte";
    import Tags from "./components/tags.svelte";
    import Padding from "./components/sd-pad-top.svelte";
    import Intro from "./components/intro.svelte";
    import GamerTags from "./components/gamertags.svelte";
    import Title from "./components/title.svelte";
    import ThreeSep from "./components/threesep.svelte";
    import Project from "./components/project.svelte";
    import TwoSep from "./components/twosep.svelte";
    import Kingswell from "./components/work/kingswell.svelte";
    import Starin from "./components/work/starin.svelte";
    import Education from "./components/education.svelte";
    import Awards from "./components/awards.svelte";
    import Papers from "./components/papers.svelte";
    import QR from "./components/qr.svelte";
</script>

<div class="viewport">
    <QR />
    <div class="print-margin">
        <NameTag />
        <Padding pad="0.25" />
        <Tags />
        <Padding pad="0.5" />
        <GamerTags />
        <Padding pad="0.5" />
        <Intro />
        <Padding />
        <Title>过往项目</Title>
        <Padding pad="0.5" />
        <ThreeSep>
            <Project name="SHPlayground" thumbnail="/shp.jpg">
                <ul>
                    <li>CUDA 实现的预计算辐射传输</li>
                    <li>用 OpenGL/ImGui 渲染</li>
                    <li>支持读取 OpenEXR HDR 环境光图</li>
                </ul>
            </Project>
            <Project name="Recon3D" thumbnail="/recon3d.png">
                <ul>
                    <li>自实现 SfM 恢复点云</li>
                    <li>OpenMVS 稠密化</li>
                    <li>Marching Cubes 网格输出</li>
                </ul>
            </Project>
            <Project last name="Scotty3D" thumbnail="/scotty3d.jpeg">
                <ul>
                    <li>基于半边实现的网格编辑器</li>
                    <li>支持网格细分和 Garland 简化</li>
                    <li>拥有 MIS 路径追踪器的完整实现</li>
                </ul>
            </Project>
        </ThreeSep>

        <Padding />
        <Title>工作经历</Title>
        <Padding pad="0.5" />
        <TwoSep>
            <Kingswell left />
            <Starin right />
        </TwoSep>

        <Padding />
        <TwoSep>
            <Education />
            <Awards />
        </TwoSep>

        <Padding />
        <Title>成果发表</Title>
        <Padding pad="0.5" />
        <Papers />
    </div>
</div>


<style>
    .viewport {
        max-width: 210mm;
        max-height: 297mm;
        border: 1px solid red;
        position: relative;
    }

    .print-margin {
        padding: 1cm;
    }

    ul {
        list-style: square;
        padding-left: 10px;
    }

    @page {
        margin: 0;
    }

    @media print {
        page {
            margin: 0;
        }

        .viewport {
            border: 0;
            background-color: white;
        }
    }

</style>
