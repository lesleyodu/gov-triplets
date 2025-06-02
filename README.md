# Temporally Extending Existing Web Archive Collections for Longitudinal Analysis

The Environmental Governance and Data Initiative (EDGI) regularly crawled US federal environmental websites between 2016 and 2020 to capture changes between two presidential administrations. However, because it does not include the previous administration ending in 2008, the collection is unsuitable for answering our research question, "Were the website terms deleted by the Trump administration added by the Obama administration?" Thus, like many researchers using the Wayback Machine’s holdings for historical analysis, we do not have access to a complete collection suiting our needs. To answer our research question, we must extend the EDGI collection back to January, 2008. This includes discovering relevant pages that were not included in the EDGI collection that persisted through 2020, not just going further back in time with the existing pages. We pieced together artifacts collected by various organizations for their purposes through many means (Save Page Now, Archive-It, and more) in order to curate a dataset sufficient for our intentions.

In this paper, we contribute a methodology to extend existing web archive collections temporally to enable longitudinal analysis, including a dataset extended with this methodology. We identified the reasons URL candidates could be missing from the initial EDGI dataset, and crawled the past web of 2008 in order to identify these missing pages. We also identified small domains that were vulnerable to being missed by our past web crawl, and found that these domains benefited from a complete web archive index lookup instead. We probed another large collection, the End of Term 2008 dataset, for additional longitudinal candidates, but found that crawler traps were inflating the size of the dataset, leading to only a small number of additional URLs. By analyzing the provenance of the final collection, we determined that this new longitudinal dataset covering three US presidential administrations only exists because of aggregation of artifacts collected by many organizations. We also found that automated brute-force methods alone were not sufficient to create this collection, and that iterative manual analysis of automated results produced more seeds for candidates. Our new dataset includes 1,220 archived triplets (2008, 2016, and 2020) of US federal environmental webpages.

We use our new dataset to analyze our question, "Were the website terms deleted by the Trump administration added by the Obama administration?" We find that 81 percent of the pages in the dataset changed between 2008 and 2020, and that 87 percent of the pages with terms deleted by the Trump administration were terms added during the Obama administration. We probed for change trends: when agencies had the same terms repeatedly removed across their websites. We found that certain agencies experienced a large number of change trends, including OSHA, NIH, and NOAA, while 17 of the 30 agencies, including NASA and the Department of Energy, experienced no change trends. Finally, we analyzed the 56 deleted terms and phrases tracked by EDGI and found that the terms fell into two categories: climate and regulation, and identified that there were more change trends in regulation term deletions than climate term deletions.

## Data

We present the dataset of 1200 triplets 2008–2016–2020 as a csv file in this repository.

Additional data available upon request:
* TimeMaps collected with [MemGator](https://github.com/oduwsdl/MemGator)
* WARCs collected with [Hypercane](https://github.com/oduwsdl/hypercane)
* CDX files collected via [grab-cdx.py](https://gist.github.com/lesleyodu/e5efc43646df58db1a93c0ddbe7f8d8f)


## References

Lesley Frew, Michael L. Nelson, and Michele C. Weigle. Temporally Extending Existing Web Archive Collections for Longitudinal Analysis. Presented at the 6th Research Infrastructure for the Study of Archived Web Materials (RESAW) Conference, 2025. ([arXiv:2505.24091](https://arxiv.org/abs/2505.24091), [slides](https://docs.google.com/presentation/d/16h76RtmIxyezdM_wDxYahnzqCIRnHEnnN9qRxoA-SJk/edit?usp=sharing))
