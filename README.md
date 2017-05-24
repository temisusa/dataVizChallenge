# dataVizChallenge
Data Viz Hack: Seeing Expert Connections

Challenge: Given a csv with experts and their publications, seek insightful and engaging ways to visualize the networks created by co-publishing.


There are two files, the full data set (millions of records) and a smaller subset (20k records). The subset may be easier to work with due to the smaller size, but feel free to trim that down further or use the entire database, as needed.

#### Google Drive links for Download:

[Expert Data Subset](https://drive.google.com/file/d/0B-EV3iSjaYwLYVFhYUcwYXE5ZW8/view?usp=sharing)


[Full Expert Dataset](https://drive.google.com/file/d/0B-EV3iSjaYwLMDZCamhubmJueEE/view?usp=sharing)


#### Info about the data

CSV header: `"documentId", "authorId", "authorName", "authorAffiliation", "authorCountry", "pubDate"`

#### Stats for full file: 
- ~4.3m rows
- 392 Megabytes
- ~2m uniquely identified experts

#### Stats for subset file:
- 20k rows
- 1.8 Megabytes 
- ~10k unique experts (rough estimate, extrapolated from the proportions for the full file)


#### Some background information about the data:
It's a sample of our MEDLINE database, along with expert names.  [Info about MEDLINE](https://www.nlm.nih.gov/pubs/factsheets/medline.html)(nih.gov)


The names have been anonymized. The sample takes all of our records with a publication date of May 1, 2016 and beyond. An article can have many co-authors of course, so what these files do is "flatten" out the articles by co-author: one row per each "incidence" of authorship. For example. If docId 123 has two authors "Alice" and "Bob",  we'll have two records to denote this, which share a docId. Although the names are anonymized, the affiliation & country  data is kept consistent across authorId.








#### example graph with dummy data*:

![Alt text](pics/example_graph.png?raw=true "Title")
![Alt text](pics/example_table.png?raw=true "Title")


*Note -- These images are just for illustrative purposes, feel free to be as creative as you wish. Based on feedback, we've added an additional field called "pubDate" so that your visualizations can have an additional dimension, if desired.



