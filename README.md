# Politician Mapping
A silly project inspired by this tweet:

<blockquote class="twitter-tweet"><p lang="en" dir="ltr">When Fetterman takes office in January, 10% of all U.S. senators will be named John/Jon</p>&mdash; Grace Segers (@Grace_Segers) <a href="https://twitter.com/Grace_Segers/status/1590432772812079104?ref_src=twsrc%5Etfw">November 9, 2022</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>

# Data description

### Senators

**Current data** is pulled from Wikipedia. Special considerations need to be made because the data includes footnotes. These need to be stripped in order to properly convert the data variables into the correct values (like dates, or proper names).
* Source: https://en.wikipedia.org/wiki/List_of_current_United_States_senators

### Representatives
**Current data** is pulled from Wikipedia, as with the current Senator data. The same considerations need to be made when processing this data.
* Source: https://en.wikipedia.org/wiki/List_of_current_members_of_the_United_States_House_of_Representatives

### General Congress

**Historical data** could potentially be pulled from the senate website, but it looks different than the current data that's available on Wikipedia. The data from the source below is downloadable as a compressed zip file. This extracts into a bunch of JSON files that then need to be processed to extract useful information. There's also a discrepancy in the dates, where the range of dates in these files matches with the start/stop of a given congress session.
* Source: https://bioguide.congress.gov/search

## Acknowledgements
Special shoutout to the following resources I used to develop this project:
* Details on parsing Wikipedia tables:

   https://medium.com/analytics-vidhya/web-scraping-a-wikipedia-table-into-a-dataframe-c52617e1f451