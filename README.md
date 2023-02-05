
# Understanding Channel / Product Overlap In Colab R

The goal if this project is to showcase some of the applications of the ggVennDiagram package in a marketing / business setting to inform decision making.

## Context

This analysis plays on the Markov chain concept, which aims to distribute the credit evenly across your multiple marketing touchpoints. However, the goal here is not to assign conversion credit but to understand the pathways users / your customers are taking en route to your site.

The singular paths see the bulk of the volume, but you will also observe an overlap across specific channels. For example, you may see a strong/weak overlap between Organic Search and Social, meaning a significant portion of your traffic is using both paths en route to your site or vice versa.
## The Challenge to Solve

Build multiple Venn diagrams using the ggVennDiagram package in R to help your clients, marketing department, or SEO teams better understand how users visit their website. 

The ggVennDiagram package allows you to understand the relationship between marketing channels, products, or channels. You are looking for a relationship where a user or item in one set also occurs in another set or lack thereof. 
## Resources Needed

You will need the following resources to conduct this type of analysis, assuming you already have access to `RStudio` through your local machine or `Google Colab`:
- Access to your dataset in the format displayed in the **`channelGrouping.csv`** data file
    - There’s a starter BigQuery query called **`Cross_Channel_Viewership_Query_BQ`** if you’re interested in how I pulled the data in that format.
## Authors

- [@dataexplorer](https://www.github.com/dataexplorer)


## Acknowledgements

 - [All You Need to Know About The ggVennDiagram Packages](https://cran.r-project.org/web/packages/ggVennDiagram/readme/README.html)
