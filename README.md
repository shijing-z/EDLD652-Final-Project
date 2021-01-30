# EDLD652-Final-Project

# Proposal
The project will use a dataset found in the [TidyTuesday](https://github.com/rfordatascience/tidytuesday) project repository. 


## [Ramen Ratings](https://github.com/rfordatascience/tidytuesday/tree/master/data/2019/2019-06-04)
The data is from the [The Ramen Rater](https://www.theramenrater.com/resources-2/the-list/).

Data dictionary is at the end of the document.

Link to the data:
```
ramen_ratings <- readr::read_csv("https://raw.githubusercontent.com/rfordatascience/tidytuesday/master/data/2019/2019-06-04/ramen_ratings.csv")
```


## Preliminary Ideas
I would like to visualize a few analyses for different audience to answer different questions. 

**Audience 1**: A food import company

**Visualization 1 & 2** - bar graph, possibly facet by different grouping variables

*Questions to answer by Visualization 1 & 2*: (*variable used*)

1. Based on the average rating (*stars*), which country (*country*) has the best ramen overall (i.e., ranking of rating by countries)? 

2. Based on the average rating (*stars*), what are the leading countries (*country*) for best ramens by different package style (*style*)? 

**Audience 2**: Ramen lover/Customer 

**Visualization 3** - not sure yet (have idea but might be repetitive)

*Questions to answer in Visualization 3*: (*variable used*)

3. What is the brand ranking (*stars*) by average rating (*stars*) within different countries of origin (*country*)?

**Audience 3**: Ramen Companies/Brands

**Visualization 4** - not sure yet (have idea but might be repetitive)

*Questions to answer in Visualization 4*: (*variable used*)

4. What is the most popular container style (*style*) by rating (*stars*) within different brands (*brand*)?


## Hope to get some help from Daniel...
Is there a way to make use of the variable *variety*? The values vary too much, and I can't figure out a way to group those values. I thought about extracting keywords, but it is hard to even extract keywords with over 3000+ observations. I think I will be able to answer some more interesting questions if I can make some use of *variety*. Otherwise those visualizations might look too similar to each other. 

Or should I use a dataset with more variables, such as [Anime Dataset](https://github.com/rfordatascience/tidytuesday/tree/master/data/2019/2019-04-23) and [Coffee Ratings
](https://github.com/rfordatascience/tidytuesday/tree/master/data/2020/2020-07-07)? Those two seem to be interesting  to me as well. 

Another selection: [NYC Squirrel Census](https://github.com/rfordatascience/tidytuesday/tree/master/data/2019/2019-10-29)


## Data Dictionary

### `ramen_ratings.csv`

|variable      |class     |description |
|:---|:---|:----------|
|review_number |integer   | Ramen review number, increasing from 1 |
|brand         |character | Brand of the ramen |
|variety       |character | The ramen variety, eg a flavor, style, ingredient |
|style         |character | Style of container (cup, pack, tray, |bowl, box, restaurant, can, bar)
|country       |character | Origin country of the ramen brand |
|stars         |double    | 0-5 rating of the ramen, 5 is best, 0 is worst |

