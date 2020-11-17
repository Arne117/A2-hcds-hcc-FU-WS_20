# `A2` - Reproducibility Workflow - Monthly Wikipedia traffic

## Project goal
The goal of this project is to construct, analyze, and publish a data set of the monthly traffic on Wikipedia.

## Data sources
We use Wikipedia traffic data from January 2008 until October 2020 collect from two different APIs:

1. The **Legacy Pagecounts API** ([documentation](https://wikitech.wikimedia.org/wiki/Analytics/AQS/Legacy_Pagecounts), [endpoint](https://wikimedia.org/api/rest_v1/#!/Pagecounts_data_(legacy)/get_metrics_legacy_pagecounts_aggregate_project_access_site_granularity_start_end)) provides access to desktop and mobile traffic data from December 2007 through July 2016.
1. The **Pageviews API** ([documentation](https://wikitech.wikimedia.org/wiki/Analytics/AQS/Pageviews), [endpoint](https://wikimedia.org/api/rest_v1/#!/Pageviews_data/get_metrics_pageviews_aggregate_project_access_agent_granularity_start_end)) provides access to desktop, mobile web, and mobile app traffic data from July 2015 through last month.

**License**

[Data license](https://creativecommons.org/publicdomain/zero/1.0/)


**Terms and conditions**

[Wikimedia REST API terms and conditions](https://www.mediawiki.org/wiki/Wikimedia_REST_API#Terms_and_conditions)

## Special considerations
- The data from the legacy page count API and the new page view API overlap from July 2015 to July 2016.
- The legacy page count API included traffic from bots and crawlers. The new page view API should resemble organic traffic.
# Replication
## Getting started

We use the  "Amazing Python Data Workflow with Poetry, Pandas, and Jupyter"<sup>[1]</sup> to make sure everyone in the course uses the same environment and we don't run into any dependency hell.

## Prerequisites

Ensure that you have a Python version greater or equal to `3.9`, a working installation of Poetry and git installed.
## Setup

```sh
# 1. Clone this repository (or use SSH) and move it into the repo root
git clone https://github.com/Arne117/A2-hcds-hcc-FU-WS_20.git
cd A2-hcds-hcc-FU-WS_20

# 2. Install the dependencies in the repo root
poetry install

# 3. Create a subshell within the virtual environment by running:
poetry shell

# 4. Open the project with Jupyter in your browser.
jupyter notebook
```

---
## Licence
This project is licensed with the [MIT License](./LICENSE).

---- 
`[1]` https://mungingdata.com/python/jupyter-workflow-poetry-pandas/, accessed: 2020-11-15
