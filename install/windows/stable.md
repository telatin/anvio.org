---
layout: page
title: "Installing anvi'o on Windows"
excerpt: "Instructions to install the current release of the platform."
modified: 2023-09-26
tags: []
categories: [anvio]
comments: false
image:
  feature: https://github.com/merenlab/anvio/raw/master/anvio/data/interactive/images/logo.png
---


{% include _project-anvio-version.html %}

This page describes the anvi'o installation process for the current stable release on _Microsoft Windows_.

## (1) Things you need before you start

{% include install/windows/things_you_need.md %}

{:.warning}
If the WSL installation fails with an error that looks like this: `WslRegisterDistribution failed with error: 0x80070032`. Then you could try the following solution: Open the Start menu and search for 'Turn Windows Features On or Off'. In the resulting pop-up box, click the checkboxes to activate "Windows Subsystem for Linux" and "Virtual Machine Platform". Then try the WSL installation again.

## (2) Set up conda

{:.notice}
Anvi'o will only run inside the WSL (Windows Subsystem for Linux, see above). If you prompt includes something like "C:\Users" you are inside the Windows Powershell (not WSL). From powershell type `wsl` to open your Linux subsystem.
To ensure you are inside the WS, type `uname` (should print "Linux"). 

{% include install/commons/stable/conda_setup.md %}

## (3) Setup an anvi'o environment

{% include install/commons/stable/initial_setup.md %}

At the time of writing these lines, running `mamba` after this step gave an error about a missing file for `libarchive` library on WSL. To see if this is really the case, you can first type `mamba` in your terminal:

```
mamba
```

If you are not getting an error (and instead seeing a nice help menu), then this problem does not affect your system and _you can skip the next command_. But if you indeed get a `libarchive` error, please run the following command and see if it solves the problem for you (this essentially creates a symbolic link to an existing file that `mamba` complains about):

```bash
ln -s ${CONDA_PREFIX}/lib/libarchive.so.19 \
      ${CONDA_PREFIX}/lib/libarchive.so.13
```

And test to make sure that `mamba` is okay now:

```
mamba
```

{% include install/commons/conda_packages.md %}

## (4) Install anvi'o

{% include install/windows/stable/pip_install.md %}

## (5) Common problems

{% include install/commons/known_issues.md %}

## (6) Check your installation

{% include install/windows/interactive_interface_note.md %}

{% include install/commons/check_installation.md %}

## Other installation options

{% include install/commons/stable/other_options.md %}

---

{:.notice}
{% include _fixthispage.html source="install/windows-stable.md" %}
