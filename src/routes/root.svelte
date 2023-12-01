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
    import Academia from "./components/work/academia.svelte";
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
        <Title>工作经历</Title>
        <Padding pad="0.25" />
        <div>
            <Kingswell />
        </div>

        <Padding />
        <Title>科研经历</Title>
        <Padding pad="0.25" />
        <div>
            <Academia />
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
        <!--<Padding />
        <Title>自我评价</Title>
        <Padding pad="0.25" />
        <p>
            本人从本科一年级至今投身于锂离子电池材料与钠离子电池材料的研究；工作积极认真，细心负责，熟练运用办公自动化软件，善于在工作中提出问题、发现问题、解决问题，有较强的分析能力；勤奋好学，踏实肯干，动手能力强，有很强的社会责任感；拥有强壮的体魄，注重劳逸结合。
        </p>-->
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
        padding-bottom: 0;
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
