<head>
    <style>
        p, h1, h2, h3, h4, h5, li::marker, ul { margin-left: 20px; margin-right: auto; width: 40em; font-size: large}
        .CrosstabViewComponent { margin-bottom: 20px }      
    </style>
</head>

# Getting the best of manual and automated gating: Tercen's hybrid approach

<img src="https://www.tercen.com/static/2e7f074dadb1a6c98e2dc5880a971171/e1bb7/Tercen_logo.webp"></img>

CYTO 2024

__Tercen Team - support@tercen.com__

### Introduction

* Tercen is a __biomedical data analysis platform__ designed to perform flexible analyses of scientific data in a __no-code__ environment.
* We provide a way to build analysis __workflows__ by combining __building blocks__ (operators and apps) performing __computation__ or producing __charts__.
* The goal is to create __reproducible__, __reusable__ and __scalable__ workflows as dataset sizes increase.

### Data and scientific context

We have CyTOF data for two donor groups: __responders__ and __non-responders__, PBMC at baseline. Our goal for today is to answer the following questions:

**- Do we observe differences in cell proportions among groups (responders, non-responders)?**

### What is Hybrid Gating?

* Approach combining both methods
* Manual gating interface
* No-code platform
* Scalability

### How does Hybrid Gating improve manual gating?

__Manual Gating: workflow 1. Pros and cons.__

* No arbitrary threshold
* Reproducible results based on a data-driven model

### How does Hybrid Gating improve automated gating?

__Auto Gating: workflow 2. Pros and cons.__

* Integration of prior biological knowledge
* Fine reference (intermediate values)

### From Raw Data to Report

* Reporting example, R vs. NR barplots

## DONE

* 3 templates with unit tests: simple_workflow, flow_core_immunophenotyping, flow_scyan_immunophenotyping
* 3-4 demo workflows for CYTO
* some datasets added to the library

## TO DO

* Update tercenctl to support workflow runner
* Release flow templates (2 immunophenotyping workflows)
* populate CYTO Demo project README: identify specific cases (manual gating improvements, etc.)
* Polish workflows (report tab, plots, step descriptions and visualisations)
* all required datasets added to the library
