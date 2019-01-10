Glossary
========

This document is currently a work-in-progress QIIME 2 terminology glossary.

.. glossary::

   Action
      A general term for a *method*, *visualizer*, or *pipeline*. Actions accept parameters and/or files (:term:`artifacts <Artifact>` or :term:`metadata`) as input, and generate some kind of output.

   Artifact
      Data that can be used as input to a QIIME *method* or *visualizer*, or that can be generated as output from a QIIME *method*. Artifacts typically have the extension ``.qza`` when written to file.

   Feature
      A unit of observation, frequently a sequence variant or OTU. Many other types of feature data can be imported into QIIME 2 (genes, metabolites, proteins, etc.). Stronger support for these data types may come in the near future, so we use the generic term feature.

   Feature Table
      A matrix of feature abundances from a given sample. (i.e. how many times each feature appeared in a given sample)

   Frequency
      The number of observations of a feature within a single unit of measure - in QIIME 2 this is generally the number of occurences of a given sequence within a single sample.

   Input
      In the context of QIIME 2, an *artifact* input to an *action*. Compare with *parameter*.

   Method
      An *action* that takes some combination of *artifacts* and *parameters* as input, and produces one or more *artifacts* as output. These output *artifacts* could subsequently be used as input to other QIIME 2 *methods* or *visualizers*. *Methods* can produce intermediate or terminal outputs in a QIIME analysis.

   Parameter
      A primitive (i.e., non-*artifact*) input to an *action*. For example, strings, integers, and booleans are primitives. Primitives are never output from an *action*.

   Pipeline
      A single "action" which combines two or more existing *actions* in one command. Pipelines accept some combination of QIIME 2 *artifacts* and *parameters* as *input*, and produce one or more QIIME 2 *artifacts* and/or *visualizations* as *output*.

   Plugin
      A plugin provides microbiome (i.e. domain-specific) analysis functionality that is accessible to users through a variety of interfaces built around the QIIME 2 framework. Plugins can be developed and distributed by anyone. In more technical terms, a plugin is a Python 3 package that instantiates a ``qiime2.plugin.Plugin`` object, and registers *actions*, *data formats*, and/or *semantic types* that become discoverable in the QIIME 2 framework.

   Relative Frequency
      The proportion of all sequences within a given sample comprised of a single feature.

   Result
      A general term for an *artifact* or *visualization*. A *result* is produced by a *method*, *visualizer*, or *pipeline*.

   Visualization
         Data that has been generated as output from a QIIME 2 *visualizer*. Visualizations typically have the extension ``.qzv`` when written to file.

   Visualizer
      An *action* that takes some combination of *artifacts* and *parameters* as input, and produces exactly one *visualization* as output. Output *visualizations*, by definition, cannot be used as input to other QIIME 2 *methods* or *visualizers*. *Visualizers* can only produce terminal output in a QIIME analysis.
