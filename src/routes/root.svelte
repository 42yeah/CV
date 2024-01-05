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
    import Project3 from "./components/work/project3.svelte";
    import GAC from "./components/work/gac.svelte";
    import Starin from "./components/work/starin.svelte";
    import Education from "./components/education.svelte";
    import Awards from "./components/awards.svelte";
    import Papers from "./components/papers.svelte";
    import QR from "./components/qr.svelte";
    import Portrait from "./components/portrait.svelte";
</script>

<div class="viewport">
    <QR />
    <Portrait />
    <div class="print-margin">
        <NameTag />
        <Padding pad="0.25" />
        <Tags />
        <Padding />
        <Education />

        <Padding />
        <Title>科研经历</Title>
        <Padding pad="0.25" />
        <div>
            <GAC />
            <Padding pad="0.5" />
            <Project3 />
            <Padding pad="0.5" />
            <Starin />
            <Padding pad="0.5" />
            <Kingswell />
        </div>

        <Padding />
        <Awards />

        <Padding />
        <Title>成果发表</Title>
        <Padding pad="0.25" />
        <Papers />

        <Padding />
        <Title>专业技能</Title>
        <Padding pad="0.25" />
        <GamerTags />
    </div>
</div>


<style>
    .viewport {
        max-width: 210mm;
        min-height: 297mm;
        max-height: 297mm;
        border: 1px solid red;
        position: relative;
        background-color: white;
    }

    .print-margin {
        padding: 1cm;
    }

    ul {
        list-style: square;
        padding-left: 13px;
    }

    li {
        padding-top: 0.5em;
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
