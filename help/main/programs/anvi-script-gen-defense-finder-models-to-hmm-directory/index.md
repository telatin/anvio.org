---
layout: program
title: anvi-script-gen-defense-finder-models-to-hmm-directory
excerpt: An anvi'o program. This program generates an anvi&#x27;o compatible HMM directory to be used with `anvi-run-hmms` from the MDMParis Defense Finder Models.
categories: [anvio]
comments: false
redirect_from: /m/anvi-script-gen-defense-finder-models-to-hmm-directory
image:
  featurerelative: ../../../images/header.png
  display: true
---

This program generates an anvi&#x27;o compatible HMM directory to be used with `anvi-run-hmms` from the MDMParis Defense Finder Models..

🔙 **[To the main page](../../)** of anvi'o programs and artifacts.


{% include _toc.html %}
<div id="svg" class="subnetwork"></div>
{% capture network_path %}{{ "network.json" }}{% endcapture %}
{% capture network_height %}{{ 300 }}{% endcapture %}
{% include _project-anvio-graph.html %}


## Authors

<div class="anvio-person"><div class="anvio-person-info"><div class="anvio-person-photo"><img class="anvio-person-photo-img" src="../../images/authors/ge0rges.jpg" /></div><div class="anvio-person-info-box"><a href="/people/ge0rges" target="_blank"><span class="anvio-person-name">Georges Kanaan</span></a><div class="anvio-person-social-box"><a href="https://gkanaan.com" class="person-social" target="_blank"><i class="fa fa-fw fa-home"></i>Web</a><a href="mailto:georges@gkanaan.com" class="person-social" target="_blank"><i class="fa fa-fw fa-envelope-square"></i>Email</a><a href="http://twitter.com/scientificgio" class="person-social" target="_blank"><i class="fa fa-fw fa-twitter-square"></i>Twitter</a><a href="http://github.com/ge0rges" class="person-social" target="_blank"><i class="fa fa-fw fa-github"></i>Github</a></div></div></div></div>



## Can consume


<p style="text-align: left" markdown="1"><span class="artifact-r">[hmm-file](../../artifacts/hmm-file) <img src="../../images/icons/TXT.png" class="artifact-icon-mini" /></span></p>


## Can provide


<p style="text-align: left" markdown="1"><span class="artifact-p">[hmm-source](../../artifacts/hmm-source) <img src="../../images/icons/HMM.png" class="artifact-icon-mini" /></span></p>


## Usage


This script downloads all the HMM models made public by the MDM-Paris lab in their [public repository](https://github.com/mdmparis/defense-finder-models) and converts it to an anvi'o compatible [hmm-source](https://anvio.org/help/main/artifacts/hmm-source/).

### Basic usage

The command will create the `hmm-source` in a folder called `DefenseFinder_HMM` in the current directory, if no such folder exists.

<div class="codeblock" markdown="1">
anvi&#45;script&#45;gen&#45;defense&#45;finder&#45;models&#45;to&#45;hmm&#45;directory
</div>

{:.notice}
Edit [this file](https://github.com/merenlab/anvio/tree/master/anvio/docs/programs/anvi-script-gen-defense-finder-models-to-hmm-directory.md) to update this information.


## Additional Resources



{:.notice}
Are you aware of resources that may help users better understand the utility of this program? Please feel free to edit [this file](https://github.com/merenlab/anvio/tree/master/bin/anvi-script-gen-defense-finder-models-to-hmm-directory) on GitHub. If you are not sure how to do that, find the `__resources__` tag in [this file](https://github.com/merenlab/anvio/blob/master/bin/anvi-interactive) to see an example.
