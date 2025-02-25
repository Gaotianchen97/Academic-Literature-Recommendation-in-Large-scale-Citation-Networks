# Academic-Literature-Recommendation-in-Large-scale-Citation-Networks
This repository shares the data from the paper “Academic Literature Recommendation in Large-scale Citation Networks Enhanced by Large Language Models” authored by Kun Liu, Yan Zhang, Rui Pan, Tianchen Gao, and Hansheng Wang.

## citation_network.csv

The file `citation_network.csv` contains the citation relationships between articles in the citation network. It can be used to construct a directed graph where each article is a node, and each citation is a directed edge from the citing article to the cited article. This file can be used to construct a directed citation network using graph analysis tools such as NetworkX in Python. The `source` and `target` IDs correspond to the `paper_ID` column in the `paper_info.csv` file.

|  Col Name  | Data Type | Description |
|-------------|------------|-------------|
| `source`      |     String    | The ID of the citing article (the article that makes the citation). |
| `target`      |     String    | The ID of the cited article (the article that is being cited). |


## paper_info.csv

The file `paper_info.csv` contains detailed information about each article in the citation network. It provides metadata such as article titles, publishers, abstracts, and publication year, which can be used to enrich the citation network analysis. This dataset contains 190,381 articles from 70 journals, covering statistics, econometrics, and computer science, spanning from 1981 to 2022. The `id` column in this file corresponds to the `source` and `target` columns in the `citation_network.csv` file.

| Column Name | Data Type | Description |
|-------------|-----------|-------------|
| `id`             | String       | Unique identifier for each article. |
| `title`          | String       | Title of the article. |
| `publisher` | String       | Publisher of the article. |
| `abstract`   | String       | Abstract of the article. |
| `year`         | Integer    | Publication year of the article. |


### Contact

For any questions or issues regarding this file, please contact tianchengao97@gmail.com.

