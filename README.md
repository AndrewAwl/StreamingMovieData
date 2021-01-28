# StreamingMovieData

# Goal

To understand the movies available on some of the big streaming platformsThere is a dataset that looks at movies found on some of the big streaming platforms, Netflix, Prime Video, Hulu, and Disney +. I may try to find a movie recommendation or two based on average ratings maybe in a couple of categories that I have not seen already. If I am able to I will try to tie this dataset to the IMDB movie dataset (found here https://www.kaggle.com/stefanoleone992/imdb-extensive-dataset), and also have a list of separately tracked movies I’ve personally seen via icheckmovies.com that has imdb links so can link to that as well to rule out movies I’ve already seen.


# Potential questions to investigate
```
·        What is the average rating of a movie on each platform? 
·        What has the highest # of quality films (need to set a benchmark for what I think that is)
·        What has the highest # of low quality films
·        Want to also try to link this to the IMDB data, that can get trickier to link the data, maybe by name - year - director? To maybe look at demographics of the ratings
·        how many movies appear on multiple platforms, are there any that appear on all 4? This is a bit more unlikely due to the nature of content on Disney+ compared to the other 3
·        What is the age of the films on the streaming platforms? Can produce this graphically
·        Look at some of these cuts by category (will have to pull out unique categories as many of the films are listed as multiple categories)
·        If able to tie last part of data together with movies watched, will see what have I watched the most of services wise, what have I watched the least of (and would be able to find most new content)
·        What are the highest rated movies on each service that I have not watched yet? Might also be able to pull in IMDB Top100 list here
```
# Limitations of data
Don’t know how this data was pulled so hopefully it is trustworthy, it is a bit stale (8 months) so not sure if all of the movies are relevant, will not account for some newer items
Based on comments this is based on streaming available in USA region only
Streaming dataset does not have an IMDB link so will have to figure out how to link data to IMDB, especially given potential overlap of titles throughout the years (Movie name – Director – Year?)

# Findings
```
·  Ran into a lot of issues with merging the streaming data set and imdb movie dataset, would like to work further / identify better ways to do this (initial step would be comparing streaming title to original title of imdb dataset as this was wildly inconsistent and imdb title is awful). Was only able to get ~5k matches out of ~17k streaming records
· Prime Video had far and away the most robust library in terms of volume (3x the other platforms), but as I saw in a few different areas, they had more lower quality movies as well which brought down their overall rating. They also were more likely to include 'older' movies with lower ratings (1930's to 2000 really stood out)
·  Disney+ had a ~0.2 higher avg rating than the other streaming services, makes sense since the other 3 platforms are more aggregators than producing their own content (until more recently)
·  Looking across platforms, only found 10 movies that were consistent between 3 platforms (none were on all 4)
·  In terms of age distribution, Disney+ was the only one to have more movies in a decade that was not the most recent one (2000's)
·  There is a lot more that could be done with the data, did not really get a chance to look at the Top250 dataset although I incorporated it, with more time can definitely look at more cross-cuts including language, runtimes, etc.
```