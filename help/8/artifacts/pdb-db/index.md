---
layout: artifact
title: pdb-db
excerpt: A DB-type anvi'o artifact. This artifact is typically generated, used, and/or exported by anvi'o (and not provided by the user)..
categories: [anvio]
comments: false
redirect_from: /8/pdb-db
image:
  featurerelative: ../../../images/header.png
  display: true
---


{% include _toc.html %}


<img src="../../images/icons/DB.png" alt="DB" style="width:100px; border:none" />

A DB-type anvi'o artifact. This artifact is typically generated, used, and/or exported **by anvi'o** (and not provided by the user)..

🔙 **[To the main page](../../)** of anvi'o programs and artifacts.

## Provided by


<p style="text-align: left" markdown="1"><span class="artifact-p">[anvi-setup-pdb-database](../../programs/anvi-setup-pdb-database)</span></p>


## Required or used by


<p style="text-align: left" markdown="1"><span class="artifact-r">[anvi-gen-structure-database](../../programs/anvi-gen-structure-database)</span></p>


## Description


## What is this thing?  

This is a comprehensive database of protein structures downloaded from the PDB RSCB that are non-redundant. Currently, it is used for those who want to run <span class="artifact-p">[anvi-gen-structure-database](/help/8/programs/anvi-gen-structure-database)</span> without an internet connection.


## Where does it come from?  

A <span class="artifact-n">[pdb-db](/help/8/artifacts/pdb-db)</span> can be created via the program <span class="artifact-p">[anvi-setup-pdb-database](/help/8/programs/anvi-setup-pdb-database)</span>. Alternatively, a <span class="artifact-n">[pdb-db](/help/8/artifacts/pdb-db)</span> that contains custom structures not found in the [RCSB PDB](https://www.rcsb.org/) can in theory be generated by the user, but anvi'o currrently offers no reasonable way of doing this.


## Notes 

The <span class="artifact-n">[pdb-db](/help/8/artifacts/pdb-db)</span> generated via <span class="artifact-p">[anvi-setup-pdb-database](/help/8/programs/anvi-setup-pdb-database)</span> is ~20GB.  



{:.notice}
Edit [this file](https://github.com/merenlab/anvio/tree/master/anvio/docs/artifacts/pdb-db.md) to update this information.
