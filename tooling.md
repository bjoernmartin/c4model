---
layout: default
title: Tooling
nav_order: 6
permalink: /tooling
---

# Tooling

For design sessions, you might find a whiteboard or flip chart paper better for collaboration, and iterating quickly.
For long-lived documentation, there are a number of tools can help create software architecture diagrams based upon
the C4 model.

Don't forget to ask yourself some questions when looking at tooling, to understand the features you need:

- Who are the diagram authors, and how technical are they?
- A "drag and drop" UI vs "diagrams as code"?
- Data stored in git next to your source code vs stored in the tool/cloud service?
- Closed vs open data format?
- Interactive vs static diagrams?
- Free vs paid vs open source?
- Short-lived vs long-lived documentation?
- Team only diagramming vs enterprise-wide modelling?
- Who is the diagram audience, and how would they access the diagrams/documentation?

<script type="application/javascript" src="https://code.jquery.com/jquery-3.7.1.slim.min.js"></script>

<style>
.toolingOptionFilter {
    margin: 10px 20px 20px 10px;
    display: inline-block;
}
.toolingOption {
    font-size: 16px;
    display: inline-block;
    margin: 10px;
    border: solid 1px #1168BD;
    padding: 5px 10px 5px 10px;
    border-radius: 5px;
}
.toolingOption:hover {
    background: #1168BD;
    color: #ffffff;
}
.toolingOption:hover a {
    color: #ffffff;
}
.toolingOption a {
    text-decoration: none;
}
.toolingOption a:hover {
    background: #1168BD;
    color: #ffffff;
    text-decoration: none;
}
.centered {
    text-align: center;
}
.faded {
    opacity: 0.2;
}
.small {
    font-size: 13px;
}
.smaller {
    font-size: 11px;
}
</style>

<table>
<tr>
<td style="vertical-align: top">
    <h4>Supported diagram types</h4>
    <div class="toolingOptionFilter">
        <label><input id="toolingStaticDiagramsFilter" type="checkbox" checked="checked" disabled="disabled"> Static diagrams</label>
        <div class="smaller">(e.g. system context, container, and component diagrams)</div>
    </div>

    <div class="toolingOptionFilter">
        <label><input id="toolingDynamicDiagramsFilter" type="checkbox"> Dynamic diagrams</label>
        <div class="smaller">(e.g. collaboration or sequence diagrams)</div>
    </div>

    <div class="toolingOptionFilter">
        <label><input id="toolingDeploymentDiagramsFilter" type="checkbox"> Deployment diagrams</label>
        <div class="smaller">(e.g. diagrams showing deployment and infrastructure concerns)</div>
    </div>
</td>
<td style="vertical-align: top">
    <h4>Diagramming vs modelling</h4>
    <div class="toolingOptionFilter">
        <label><input id="toolingDiagrammingFilter" name="diagramVsModel" type="radio"> Diagramming tool</label>
        <div class="smaller">(i.e. a modelling tool - to keep multiple diagrams in sync automatically when you rename elements)</div>
    </div>

    <div class="toolingOptionFilter">
        <label><input id="toolingModelBasedFilter" name="diagramVsModel" type="radio" checked="checked"> Reuse elements across multiple diagrams</label>
        <div class="smaller">(i.e. a modelling tool - to keep multiple diagrams in sync automatically when you rename elements)</div>
        <div style="margin-top: 10px">
        <span class="smaller" style="font-weight: normal; background: #02b621; color: #ffffff; padding: 5px; margin-top: 10px;">Recommended</span>
        </div>
    </div>
</td>
<td style="vertical-align: top">
    <h4>Authoring</h4>
    <div class="toolingOptionFilter">
        <label><input id="toolingWithUIFilter" name="authoring" type="radio"> Graphical user interface</label>
        <div class="smaller">(drag and drop modelling UI)</div>
    </div>

    <div class="toolingOptionFilter">
        <label><input id="toolingAsCodeFilter" name="authoring" type="radio" checked="checked"> Diagrams and models as code</label>
        <div class="smaller">(for easy version control and integration into build pipelines/other tools)</div>
    </div>
</td>
<td style="vertical-align: top">
    <h4>Other</h4>
    <div class="toolingOptionFilter">
        <label><input id="toolingOpenSourceFilter" type="checkbox"> Open source</label>
        <div class="smaller">(free, fork/customize, etc)</div>
    </div>

    <div class="toolingOptionFilter">
        <label><input id="toolingRenderingToolIndependentFilter" type="checkbox"> Rendering tool independent</label>
        <div class="smaller">(to render diagrams with different tools or visualisation formats such as <a href="#AlternativeVisualisations">diagrams, graphs, etc</a>)</div>
    </div>
</td>
</tr>
</table>

<div class="centered">
    <div class="toolingOption toolingOpenSource toolingModelBased toolingStaticDiagrams toolingDynamicDiagrams toolingDeploymentDiagrams">
        <a href="https://www.archimatetool.com/blog/2020/04/18/c4-model-architecture-viewpoint-and-archi-4-7/" target="_blank">Archi</a>
    </div>
    <div class="toolingOption toolingOpenSource toolingDiagramming toolingAsCode toolingStaticDiagrams">
        <a href="https://github.com/lonely-lockley/archinsight" target="_blank">Archinsight</a>
    </div>
    <div class="toolingOption toolingModelBased toolingWithUI toolingStaticDiagrams toolingDeploymentDiagrams">
        <a href="https://www.archipeg.com/learn/c4-model-v1-metamodel" target="_blank">Archipeg</a>
    </div>
    <div class="toolingOption toolingModelBased toolingWithUI toolingStaticDiagrams toolingDynamicDiagrams toolingDeploymentDiagrams">
        <a href="https://github.com/ChangeVision/astah-c4model-plugin" target="_blank">Astah</a>
    </div>
    <div class="toolingOption toolingOpenSource toolingDiagramming toolingAsCode toolingStaticDiagrams toolingDynamicDiagrams toolingDeploymentDiagrams">
        <a href="https://github.com/plantuml-stdlib/C4-PlantUML" target="_blank">C4-PlantUML</a>
    </div>
    <div class="toolingOption toolingOpenSource toolingDiagramming toolingAsCode toolingStaticDiagrams toolingDynamicDiagrams toolingDeploymentDiagrams">
        <a href="https://adrianvlupu.github.io/C4-Builder" target="_blank">c4builder</a>
    </div>
    <div class="toolingOption toolingOpenSource toolingModelBased toolingAsCode toolingStaticDiagrams">
        <a href="https://github.com/SlavaVedernikov/C4InterFlow" target="_blank">C4InterFlow</a>
    </div>
    <div class="toolingOption toolingOpenSource toolingDiagramming toolingAsCode toolingStaticDiagrams toolingDeploymentDiagrams">
        <a href="https://github.com/8T4/c4sharp" target="_blank">C4Sharp</a>
    </div>
    <div class="toolingOption toolingOpenSource toolingDiagramming toolingAsCode toolingStaticDiagrams">
        <a href="https://owulveryck.github.io/cue4puml4c4/" target="_blank">CUE4Puml4C4</a>
    </div>
    <div class="toolingOption toolingOpenSource toolingDiagramming toolingAsCode toolingStaticDiagrams">
        <a href="https://diagrams.mingrammer.com/docs/nodes/c4" target="_blank">Diagrams</a>
    </div>
    <div class="toolingOption toolingOpenSource toolingDiagramming toolingWithUI toolingStaticDiagrams toolingDynamicDiagrams toolingDeploymentDiagrams">
        <a href="https://www.diagrams.net/blog/c4-modelling" target="_blank">diagrams.net</a>
    </div>
    <div class="toolingOption toolingWithUI toolingDiagramming toolingStaticDiagrams toolingDynamicDiagrams toolingDeploymentDiagrams">
        <a href="https://libraries.excalidraw.com/#dmitry-burnyshev-c4-architecture" target="_blank">Excalidraw</a>
    </div>
    <div class="toolingOption toolingWithUI toolingDiagramming toolingStaticDiagrams toolingDynamicDiagrams toolingDeploymentDiagrams">
        <a href="https://www.figma.com/templates/c4-model-examples/" target="_blank">Figma</a>
    </div>
    <div class="toolingOption toolingWithUI toolingOpenSource toolingModelBased toolingStaticDiagrams toolingDynamicDiagrams toolingDeploymentDiagrams">
        <a href="https://gaphor.org" target="_blank">Gaphor</a>
    </div>
    <div class="toolingOption toolingWithUI toolingDiagramming toolingStaticDiagrams toolingDynamicDiagrams toolingDeploymentDiagrams">
        <a href="https://www.gliffy.com/blog/c4-model" target="_blank">Gliffy</a>
    </div>
    <div class="toolingOption toolingWithUI toolingModelBased toolingStaticDiagrams toolingDynamicDiagrams">
        <a href="https://icepanel.io/c4-model" target="_blank">IcePanel</a>
    </div>
    <div class="toolingOption toolingOpenSource toolingDiagramming toolingAsCode toolingStaticDiagrams toolingDynamicDiagrams toolingDeploymentDiagrams">
        <a href="https://keadex.dev/en/projects/keadex-mina" target="_blank">Keadex Mina</a>
    </div>
    <div class="toolingOption toolingWithUI toolingDiagramming toolingStaticDiagrams toolingDynamicDiagrams toolingDeploymentDiagrams">
        <a href="https://www.lucidchart.com/pages/templates/c-4-model-example" target="_blank">Lucidchart</a>
    </div>
    <div class="toolingOption toolingWithUI toolingDiagramming toolingStaticDiagrams toolingDynamicDiagrams toolingDeploymentDiagrams">
        <a href="https://github.com/pihalve/c4model-visio-stencil" target="_blank">Microsoft Visio</a>
    </div>
    <div class="toolingOption toolingOpenSource toolingDiagramming toolingAsCode toolingStaticDiagrams toolingDynamicDiagrams toolingDeploymentDiagrams">
        <a href="https://mermaid.js.org/syntax/c4.html" target="_blank">Mermaid</a>
    </div>
    <div class="toolingOption toolingWithUI toolingDiagramming toolingStaticDiagrams toolingDynamicDiagrams toolingDynamicDiagrams toolingDeploymentDiagrams">
        <a href="https://miro.com/miroverse/c4-architecture/" target="_blank">Miro</a>
    </div>
    <div class="toolingOption toolingOpenSource toolingModelBased toolingAsCode toolingStaticDiagrams toolingDynamicDiagrams toolingDeploymentDiagrams">
        <a href="https://github.com/goadesign/model" target="_blank">Model</a>
    </div>
    <div class="toolingOption toolingWithUI toolingModelBased toolingStaticDiagrams">
        <a href="https://supportportal.moodinternational.com/hc/en-us/articles/360015465100-MooD-and-the-C4-model" target="_blank">MooD</a>
    </div>
    <div class="toolingOption toolingWithUI toolingDiagramming toolingStaticDiagrams toolingDynamicDiagrams toolingDeploymentDiagrams">
        <a href="https://stenciltown.omnigroup.com/stencils/c4/" target="_blank">OmniGraffle</a>
    </div>
    <div class="toolingOption toolingOpenSource toolingModelBased toolingAsCode toolingStaticDiagrams toolingDynamicDiagrams toolingDeploymentDiagrams">
        <a href="https://github.com/soulspace-org/overarch" target="_blank">Overarch</a>
    </div>
    <div class="toolingOption toolingOpenSource toolingModelBased toolingAsCode toolingStaticDiagrams toolingDynamicDiagrams toolingDeploymentDiagrams">
        <a href="https://github.com/DrMarkusVoss/pumla/blob/main/test/examples/C4example/pumlaC4Example.md" target="_blank">pumla</a>
    </div>
    <div class="toolingOption toolingOpenSource toolingModelBased toolingAsCode toolingStaticDiagrams">
        <a href="https://github.com/nielsvanspauwen/pystructurizr" target="_blank">PyStructurizr</a>
    </div>
    <div class="toolingOption toolingWithUI toolingModelBased toolingStaticDiagrams toolingDynamicDiagrams toolingDeploymentDiagrams">
        <a href="http://www.sparxsystems.eu/c4/" target="_blank">Sparx Enterprise Architect</a>
    </div>
    <div class="toolingOption toolingOpenSource toolingModelBased toolingAsCode toolingStaticDiagrams">
        <a href="https://rdbmodel.github.io" target="_blank">RDB modeling</a>
    </div>
    <div class="toolingOption toolingOpenSource toolingModelBased toolingAsCode toolingRenderingToolIndependent toolingStaticDiagrams toolingDynamicDiagrams toolingDeploymentDiagrams">
        <a href="https://structurizr.org" target="_blank">Structurizr</a>
    </div>
    <div class="toolingOption toolingWithUI toolingDiagramming toolingStaticDiagrams toolingDynamicDiagrams toolingDeploymentDiagrams">
        <a href="https://online.visual-paradigm.com/diagrams/features/c4-model-tool/" target="_blank">Visual Paradigm</a>
    </div>
    <div class="toolingOption toolingWithUI toolingDiagramming toolingStaticDiagrams toolingDynamicDiagrams toolingDeploymentDiagrams">
        <a href="https://github.com/Ferhat67/C4-yEd" target="_blank">yEd</a>
    </div>
</div>

<script>
    $('#toolingOpenSourceFilter, #toolingDiagrammingFilter, #toolingModelBasedFilter, #toolingAsCodeFilter, #toolingWithUIFilter, #toolingRenderingToolIndependentFilter, #toolingStaticDiagramsFilter, #toolingDynamicDiagramsFilter, #toolingDeploymentDiagramsFilter').change(function() {
        filterToolingOptions();
    });

    function filterToolingOptions() {
        var classes = '';

        if ($('#toolingOpenSourceFilter').is(":checked")) {
            classes = classes + '.toolingOpenSource';
        }
        
        if ($('#toolingDiagrammingFilter').is(":checked")) {
            classes = classes + '.toolingDiagramming';
        }
        
        if ($('#toolingModelBasedFilter').is(":checked")) {
            classes = classes + '.toolingModelBased';
        }
        
        if ($('#toolingAsCodeFilter').is(":checked")) {
            classes = classes + '.toolingAsCode';
        }
        
        if ($('#toolingWithUIFilter').is(":checked")) {
            classes = classes + '.toolingWithUI';
        }
        
        if ($('#toolingRenderingToolIndependentFilter').is(":checked")) {
            classes = classes + '.toolingRenderingToolIndependent';
        }
        
        if ($('#toolingStaticDiagramsFilter').is(":checked")) {
            classes = classes + '.toolingStaticDiagrams';
        }
        
        if ($('#toolingDynamicDiagramsFilter').is(":checked")) {
            classes = classes + '.toolingDynamicDiagrams';
        }
        
        if ($('#toolingDeploymentDiagramsFilter').is(":checked")) {
            classes = classes + '.toolingDeploymentDiagrams';
        }
        
        if (classes.length === 0) {
            $('.toolingOption').removeClass('faded');
        } else {
            $('.toolingOption').addClass('faded');
            $('.toolingOption').filter(classes).removeClass('faded');
        }
    }

    filterToolingOptions();
</script>