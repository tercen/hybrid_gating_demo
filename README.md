# Getting the best of manual and automated gating: Tercen's hybrid approach

<img src="https://www.tercen.com/static/2e7f074dadb1a6c98e2dc5880a971171/e1bb7/Tercen_logo.webp"></img>

CYTO 2024

__Tercen Team__

## Introduction

Advances in single-cell technologies, such as high parameter flow cytometry, have enabled comprehensive profiling of immune states in health and disease. Such developments have highlighted the broad range of immunophenotypes driving complex immunological responses.

As the amount of data being generated grows, the conventional cytometry data analysis workflow becomes more challenging. It involves several manually performed steps, such as the selection of cells based on parameter values, annotation of the same, and display in either one-dimensional or two-dimensional charts. This process, referred to as manual gating, becomes time-consuming and cumbersome with high-dimensional data, leading to an increase in human operator variability and a decrease in result reproducibility. In this context, it is critical to develop tools and approaches to run robust data analysis while ensuring those approaches remain accessible to anyone. On the other hand, fully-automated approaches, even though they scale well with the size of datasets, may struggle with poorly resolved or complex data and can be less flexible than manual approaches.

Tercen is a biomedical data analysis platform designed to perform flexible analyses of scientific data in a no-code environment. In this presentation, we show that by leveraging Tercen's flexible analysis environment, one can implement a hybrid gating approach that combines the strengths of manual and automated gating while mitigating their respective pitfalls. This approach enables robust and reproducible analysis of high-dimensional flow cytometry data, facilitating comprehensive profiling of immune states in health and disease.


## Data and scientific context

The dataset we use here comes from Krieg et al.'s study. As the inhibition of programmed cell death protein 1 (PD-1) has been found to be effective for the treatment of metastatic melanoma, a large proportion of patients do not show durable responses. They generated high-dimensional single-cell mass cytometry for the in-depth characterization of the immune cell subsets in the peripheral blood of patients with stage IV melanoma before and after 12 weeks of anti-PD-1 immunotherapy.

Our goal here is to reanalyse this dataset in Tercen. We loaded a subset of the data from three donor groups: __healthy donors__, __responders__ and __non-responders__, PBMC 12 weeks after treatment. Our goal is to answer the following questions:

**- Do we observe cell populations that are differentially abundant among groups?**


## Workflows

This project includes the following data analysis workflows:

### 1. Manual Gating

### 2. Automated Gating

### 3. Hybrid Gating

* Approach combining both methods
* Manual gating interface
* No-code platform
* Scalability

__How does Hybrid Gating improve automated gating?__

* Integration of prior biological knowledge
* Finer reference (intermediate values)
* __EXAMPLE__: intermediate values in gating-based reference: better at capturing gd T Cells

__How does Hybrid Gating improve manual gating?__

* No arbitrary threshold
* __EXAMPLE__: CD27+/- B Cells

* Reproducible results based on a data-driven model: no human factor

### How does Hybrid Gating improve automated gating?

__Auto Gating: workflow 2. Pros and cons.__

* Integration of prior biological knowledge
* Fine reference (intermediate values)

### 4. Reporting in Tercen

* Reporting example, R vs. NR barplots
* Powerpoint export

## References

> Blampey Q, Bercovici N, Dutertre CA, Pic I, Ribeiro JM, André F, Cournède PH, A biology-driven deep generative model for cell-type annotation in cytometry, Briefings in Bioinformatics, Volume 24, Issue 5, September 2023, bbad260

* [Link to scyan paper](https://academic.oup.com/bib/article/24/5/bbad260/7231520?login=false)

> Krieg C, Nowicka M, Guglietta S, Schindler S, Hartmann FJ, Weber LM, Dummer R, Robinson MD, Levesque MP, Becher B. High-dimensional single-cell analysis predicts response to anti-PD-1 immunotherapy. Nat Med. 2018 Feb;24(2):144-153. doi: 10.1038/nm.4466. Epub 2018 Jan 8. Erratum in: Nat Med. 2018 Nov;24(11):1773-1775. PMID: 29309059.

* [Link to dataset paper](https://pubmed.ncbi.nlm.nih.gov/29309059/)
