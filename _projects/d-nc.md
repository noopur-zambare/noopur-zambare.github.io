---
title: "Neaural Network Pruning Algorithm"
collection: projects
permalink: /projects/project-4

image: /images/debiased_pruning/diagram.png

excerpt: "<div style='text-align: justify;'> 
<ul>
<li>Neural Collapse-Inspired Pruning: Preserves class separability during pruning in imbalanced datasets.</li>
<li>Bias Mitigation & Robustness: Reduces bias towards majority classes and tests model robustness under noisy conditions.</li>
<li>Experimental Results: Demonstrates effective accuracy retention and fairness, especially for minority classes in imbalanced data.</li>
</ul>
</div>"
---

<h2>Overview</h2>

<p>
This project implements a novel pruning technique inspired by Neural Collapse (NC) geometry to enhance the robustness of pruned neural networks, particularly in imbalanced datasets. The proposed method utilizes the within-class scatter matrix to maintain class-separability during pruning, ensuring that minority class features are retained. This approach addresses the bias introduced by traditional pruning methods, which tend to favor majority classes in imbalanced data.
</p>

<h2>Key Features</h2>

<ul>
    <li>Neural Collapse-Inspired Pruning: A pruning technique using the within-class scatter matrix to preserve class-separability in the pruned network.</li>
    <li>Bias Mitigation: Reduces bias towards majority classes in imbalanced datasets by maintaining minority class features.</li>
    <li>Robustness Testing: Includes robustness testing against noisy data using perturbation sensitivity.</li>
</ul>

<h2>Research Questions</h2>

<ul>
    <li>Can Neural Collapse-inspired pruning improve performance under imbalanced datasets?</li>
    <li>Does this pruning method enhance model robustness?</li>
</ul>

<h2>Contributions</h2>

<ul>
    <li>Analysis of pruned neural network performance under different pruning techniques.</li>
    <li>Introduction of a geometry-based pruning algorithm inspired by Neural Collapse.</li>
    <li>Evaluation of robustness and generalization in pruned networks.</li>
</ul>

<h2>Proposed Solution</h2>

<!-- IMAGE WITH BORDER -->
<div style="margin-top: 10px;">
  <img src="/images/debiased_pruning/diagram.png"
       alt="Proposed Solution Diagram"
       style="
         width: 90%;
         display: block;
         margin: 0 auto;
         border: 1px solid #ddd;
         border-radius: 4px;
         padding: 2px;
         background: #fff;
       ">
</div>