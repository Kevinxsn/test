---
title: Home
layout: home
---


## Table of Contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Overview

Housing prices serve as a key indicator of a region's economic health. The fluctuation of housing prices over time offers insights into the region's development to a certain degree. In this project, you will explore notable trends in housing prices over the past decade, alongside their correlation with changes in environmental conditions such as precipitation and temperature. An exciting aspect of this project is the opportunity to select the datasets you find most compelling for the topic you chose. You will engage in data manipulation techniques such as concatenation and merging of DataFrames, skills that were introduced at the start of this course!

## Getting The Data
You can get the data from [`here`](). 

The data about housing prices is provided by [`Zillow`](https://www.zillow.com/). The data about the weather is provided by [`United States Census Bureau`](https://www.census.gov/). 

## Data Introduction

### population.csv

| Header | Description |
| --- | --- |
| **STATE** | Numbered starting from 1, in the order of the first letter of each state. |
| **COUNTY** | Numbered starting from 1, in the order of the first letter of each county in each state. |
| **STNAME** | Name of each state. |
| **CTYNAME** | Name of each county. |
| **POPESTIMATE XXXX** | Estimated population based on census in year XXXX. |
| **NPOPCHG XXXX** | Estimated population change based on census in year XXXX. |
| **BIRTHS XXXX** | Estimated number of births based on census in year XXXX. |
| **DEATHS XXXX** | Estimated number of deaths based on census in year XXXX. |
| **NATURALCHG XXXX** | Estimated number of deaths based on census in year XXXX. |
| **INTERNATIONALMIG XXXX** | Estimated number of international imigrant based on census in year XXXX. |
| **DOMESTICMIG XXXX** | Estimated number of domestic imigrant based on census in year XXXX. |
| **NETMIG XXXX** | Estimated number of net imigrant based on census in year XXXX. |
| **RBIRTH XXXX** | Estimated birth rate based on census in year XXXX. |
| **RDEATH XXXX** | Estimated death rate based on census in year XXXX. |
| **RNATURALCHG XXXX** | Estimated rate of natural population change based on census in year XXXX. |
| **RINTERNATIONALMIG XXXX** | Estimated rate of international imigrant change based on census in year XXXX. |
| **RDOMESTICMIG XXXX** | Estimated rate of demostic imigrant change based on census in year XXXX. |
| **RNETMIG XXXX** | Estimated rate of net inmigrant change based on census in year XXXX. |


### housing_price.csv

| Header | Description |
| --- | --- |
| **RegionID** | ID of each county in the US. |
| **SizeRank** | Ranking of each county based on size. |
| **RegionName** | Name of each region. |
| **RegionType** | Type of each region, in this case, allof them are countyes. |
| **StateName** | The name of state that this region belongs to. |
| **Metro** | The name of metro that this region belongs to. |
| **StateCodeFIPS** | County FIPS codes in the United States are usually (with a few exceptions) in the same sequence as alphabetized county names within a state. |



### perXXXX.csv
It's a dataset contains the precipitation for the year of XXXX. Feel free to only load the dataset file that useful for your project. 

| Header | Description |
| --- | --- |
| **Name** | Name of each county. |
| **State** | The name of state that this county belongs to. |
| **Value** | mean precipitation for this year in this county in inches. |
| **Rank** | Ranking of the precipitation of the this county among all of the counties in the US, from low to high. |
| **Anomaly (1901-2000 base period)** | The degree of abnormality observed over the past few years(based on 1901-2000). |
| **1901-2000 Mean** | The mean precipitation of this region from 1901-2000. |





This is a *bare-minimum* template to create a Jekyll site that uses the [Just the Docs] theme. You can easily set the created site to be published on [GitHub Pages] – the [README] file explains how to do that, along with other details.

If [Jekyll] is installed on your computer, you can also build and preview the created site *locally*. This lets you test changes before committing them, and avoids waiting for GitHub Pages.[^1] And you will be able to deploy your local build to a different platform than GitHub Pages.

More specifically, the created site:

- uses a gem-based approach, i.e. uses a `Gemfile` and loads the `just-the-docs` gem
- uses the [GitHub Pages / Actions workflow] to build and publish the site on GitHub Pages

Other than that, you're free to customize sites that you create with this template, however you like. You can easily change the versions of `just-the-docs` and Jekyll it uses, as well as adding further plugins.

[Browse our documentation][Just the Docs] to learn more about how to use this theme.

To get started with creating a site, simply:

1. click "[use this template]" to create a GitHub repository
2. go to Settings > Pages > Build and deployment > Source, and select GitHub Actions

If you want to maintain your docs in the `docs` directory of an existing project repo, see [Hosting your docs from an existing project repo](https://github.com/just-the-docs/just-the-docs-template/blob/main/README.md#hosting-your-docs-from-an-existing-project-repo) in the template README.

----

[^1]: [It can take up to 10 minutes for changes to your site to publish after you push the changes to GitHub](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/creating-a-github-pages-site-with-jekyll#creating-your-site).

[Just the Docs]: https://just-the-docs.github.io/just-the-docs/
[GitHub Pages]: https://docs.github.com/en/pages
[README]: https://github.com/just-the-docs/just-the-docs-template/blob/main/README.md
[Jekyll]: https://jekyllrb.com
[GitHub Pages / Actions workflow]: https://github.blog/changelog/2022-07-27-github-pages-custom-github-actions-workflows-beta/
[use this template]: https://github.com/just-the-docs/just-the-docs-template/generate
