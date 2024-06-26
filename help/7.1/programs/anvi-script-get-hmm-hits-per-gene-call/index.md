---
layout: help
title: anvi-script-get-hmm-hits-per-gene-call [program]
categories: [anvio]
comments: false
redirect_from: /7.1/anvi-script-get-hmm-hits-per-gene-call
image:
  featurerelative: ../../../images/header.png
  display: true
---

A simple script to generate a TAB-delimited file gene caller IDs and their HMM hits for a given HMM source.

🔙 **[To the main page](../../)** of anvi'o programs and artifacts.


{% include _toc.html %}
<div id="svg" class="subnetwork"></div>
{% capture network_path %}{{ "network.json" }}{% endcapture %}
{% capture network_height %}{{ 300 }}{% endcapture %}
{% include _project-anvio-graph.html %}


## Authors

<div class="anvio-person"><div class="anvio-person-info"><div class="anvio-person-photo"><img class="anvio-person-photo-img" src="../../images/authors/meren.jpg" /></div><div class="anvio-person-info-box"><span class="anvio-person-name">A. Murat Eren (Meren)</span><div class="anvio-person-social-box"><a href="http://meren.org" class="person-social" target="_blank"><i class="fa fa-fw fa-home"></i>Web</a><a href="mailto:a.murat.eren@gmail.com" class="person-social" target="_blank"><i class="fa fa-fw fa-envelope-square"></i>Email</a><a href="http://twitter.com/merenbey" class="person-social" target="_blank"><i class="fa fa-fw fa-twitter-square"></i>Twitter</a><a href="http://github.com/meren" class="person-social" target="_blank"><i class="fa fa-fw fa-github"></i>Github</a></div></div></div></div>



## Can consume


<p style="text-align: left" markdown="1"><span class="artifact-r">[contigs-db](../../artifacts/contigs-db) <img src="../../images/icons/DB.png" class="artifact-icon-mini" /></span> <span class="artifact-r">[hmm-source](../../artifacts/hmm-source) <img src="../../images/icons/HMM.png" class="artifact-icon-mini" /></span> <span class="artifact-r">[hmm-hits](../../artifacts/hmm-hits) <img src="../../images/icons/CONCEPT.png" class="artifact-icon-mini" /></span></p>


## Can provide


<p style="text-align: left" markdown="1"><span class="artifact-p">[functions-txt](../../artifacts/functions-txt) <img src="../../images/icons/TXT.png" class="artifact-icon-mini" /></span></p>


## Usage


This program lets you convert the <span class="artifact-n">[hmm-hits](/help/7.1/artifacts/hmm-hits)</span> within a <span class="artifact-n">[contigs-db](/help/7.1/artifacts/contigs-db)</span> into a <span class="artifact-n">[functions-txt](/help/7.1/artifacts/functions-txt)</span>.

It is similar to <span class="artifact-n">[anvi-export-functions](/help/7.1/programs/anvi-export-functions)</span>, except it deals specifically with <span class="artifact-n">[hmm-hits](/help/7.1/artifacts/hmm-hits)</span> (which are generated by <span class="artifact-n">[anvi-run-hmms](/help/7.1/programs/anvi-run-hmms)</span>; in contrast, <span class="artifact-n">[anvi-export-functions](/help/7.1/programs/anvi-export-functions)</span> works with the more abstract <span class="artifact-n">[functions](/help/7.1/artifacts/functions)</span> artifact. 

Here is an example run of this program:

<div class="codeblock" markdown="1">
anvi&#45;script&#45;get&#45;hmm&#45;hits&#45;per&#45;gene&#45;call &#45;c <span class="artifact&#45;n">[contigs&#45;db](/help/7.1/artifacts/contigs&#45;db)</span> \ 
                                       &#45;o path/to/<span class="artifact&#45;n">[functions&#45;txt](/help/7.1/artifacts/functions&#45;txt)</span> 
</div>

You also have the option to specify a specific <span class="artifact-n">[hmm-source](/help/7.1/artifacts/hmm-source)</span>, so that only hits from that source are outputted. For example: 

<div class="codeblock" markdown="1">
anvi&#45;script&#45;get&#45;hmm&#45;hits&#45;per&#45;gene&#45;call &#45;c <span class="artifact&#45;n">[contigs&#45;db](/help/7.1/artifacts/contigs&#45;db)</span> \ 
                                       &#45;o path/to/<span class="artifact&#45;n">[functions&#45;txt](/help/7.1/artifacts/functions&#45;txt)</span> \
                                       &#45;&#45;hmm&#45;source Bacteria_71
</div>


{:.notice}
Edit [this file](https://github.com/merenlab/anvio/tree/master/anvio/docs/programs/anvi-script-get-hmm-hits-per-gene-call.md) to update this information.


## Additional Resources



{:.notice}
Are you aware of resources that may help users better understand the utility of this program? Please feel free to edit [this file](https://github.com/merenlab/anvio/tree/master/bin/anvi-script-get-hmm-hits-per-gene-call) on GitHub. If you are not sure how to do that, find the `__resources__` tag in [this file](https://github.com/merenlab/anvio/blob/master/bin/anvi-interactive) to see an example.
