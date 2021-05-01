# Ford GoBike TripData Exploration

## Dataset

The dataset includes information about individual rides made in a bike-sharing system covering the greater San Francisco Bay area of the ford gobike for the year 2018.

For this analysis, I have downloaded 2018 datasets, which are 12 CSVs for each month.

**Brief description about the data :**
- Trip Duration (seconds)
- Start Time and Date
- End Time and Date
- Start Station ID
- Start Station Name
- Start Station Latitude
- Start Station Longitude
- End Station ID
- End Station Name
- End Station Latitude
- End Station Longitude
- Bike ID
- User Type (“Subscriber” = Member or “Customer” = Casual)
- Member Year of Birth
- Member Gender
- Bike Share for all Trip

**DataSource:** [Ford GoBike](https://s3.amazonaws.com/fordgobike-data/index.html)

Also, you can get the merged data [here](https://www.kaggle.com/keerthanamanoharan/ford-gobike-tripdata-2018)


## Summary of Findings

In the exploration, I found that there was a strong relationship between the
price of a diamond and its carat weight, with modifying effects from the cut,
color, and clarity grades given to the diamond. The relationship is
approximately linear between price and carat when price is transformed to be on
a logarithmic scale and carat transformed to be on a cube-root scale. I found a
somewhat surprising result initially when the marginal trend for the cut, color,
and clarity variables indicated that higher diamond quality was associated with
lower price. However, higher diamond quality was also associated with smaller
diamonds. When I isolated diamonds of a single carat weight, there was a clear
positive relationship between higher diamond quality and higher diamond price.

Outside of the main variables of interest, I verified the relationship between
diamond carat weight and its x, y, and z dimensions. For the dataset given,
there was an interesting interaction in the categorical diamond quality
features. The lower clarity grades looked like they had slightly better
distribution of cut and color grades than diamonds with the higher clarity
grades.


## Key Insights for Presentation

For the presentation, I focus on just the influence of the four Cs of diamonds
and leave out most of the intermediate derivations. I start by introducing the
price variable, followed by the pattern in carat distribution, then plot the
transformed scatterplot.

Afterwards, I introduce each of the categorical variables one by one. To start,
I use the violin plots of price and carat across clarity. I'm only looking at
the clarity grade plot here since it's the clearest example of how the
categorical quality grades affect diamond pricing. The other two categorical
variables, cut and color, are covered afterwards, using point plots. I've made
sure to use different color palettes for each quality variable to make sure it
is clear that they're different between plots.

