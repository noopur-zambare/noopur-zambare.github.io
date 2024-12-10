---
title: "Dense Network Pruning using Neural Collapse under Imbalanced Dataset"
excerpt: "<div style='text-align: justify;'> 
<b><li>Neural Network Pruning Algorithm</li></b>
<li>Neural Collapse-Inspired Pruning: Preserves class separability during pruning, particularly for minority classes in imbalanced datasets.</li>
<li>Bias Mitigation & Robustness: Reduces bias towards majority classes and tests model robustness under noisy conditions.</li>
<li>Experimental Results: Demonstrates effective accuracy retention and fairness, especially for minority classes in imbalanced data.</li>"
collection: projects
permalink: /projects/project-3

---
<h2>Overview</h2>
    <p>This project implements a novel pruning technique inspired by Neural Collapse (NC) geometry to enhance the robustness of pruned neural networks, particularly in imbalanced datasets. The proposed method utilizes the within-class scatter matrix to maintain class-separability during pruning, ensuring that minority class features are retained. This approach addresses the bias introduced by traditional pruning methods, which tend to favor majority classes in imbalanced data.</p>

<h2>Key Features</h2>
<ul>
    <li>Neural Collapse-Inspired Pruning: A pruning technique using the within-class scatter matrix to preserve the class-separability in the pruned network.</li>
    <li>Bias Mitigation: Reduces bias towards majority classes in imbalanced datasets by maintaining minority class features during pruning.</li>
    <li>Robustness Testing: Includes robustness testing against noisy data using perturbation sensitivity to assess model robustness.
</li>
</ul>

<h2>Research Questions</h2>
    <ul>
        <li>Can Neural Collapse-inspired pruning improve the performance of pruned networks under imbalanced datasets?</li>
        <li>Does this pruning method enhance the robustness of the model?</li>
    </ul>

<h2>Contributions</h2>
<ul>
    <li>Analysis of pruned neural network performance under various pruning techniques.</li>
    <li>Introduction of a pruning algorithm based on feature space geometry inspired by Neural Collapse.</li>
    <li>Evaluation of robustness and generalization in pruned networks.</li>
</ul>



