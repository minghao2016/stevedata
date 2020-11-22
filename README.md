
# `stevedata`: Steve’s Toy Data

<img src="http://svmiller.com/images/stevedata-hexlogo.png" alt="My stevedata  hexlogo" align="right" width="200" style="padding: 0 15px; float: right;"/>

`stevedata` is an R package full of toy data sets that you may find
useful for various purposes. Namely, I’ve created probably over a
hundred toy data sets along the way, either to riff on some topic on [my
blog](http://svmiller.com/blog), show my students something in one of
[my many classes](http://svmiller.com/teaching), or just to entertain
myself for [spamming Twitter with my assorted
thoughts](https://twitter.com/stevenvmiller). I had stuffed a lot of
these into [`stevemisc`](https://github.com/svmiller/stevemisc), but I
want to keep that package mostly about the functions (and whatever data
are useful for showing off the functions). `stevedata` will have all my
toy data going forward.

I will also be having my methods students (undergraduate and graduate)
download this package to work through problem sets in the R programming
language. It’d be a benefit to them (and less hassle/headache for
myself) to have my students download this package from CRAN rather than
workthrough potential Curl issues by installing through Github.

## Installation

The goal is to get this on CRAN, eventually. Until then, you can install
the development version of `stevedata` from Github via the `devtools`
package. I suppose using the `remotes` package would work as well.

``` r
devtools::install_github("svmiller/stevedata")
```

## Usage

The usage, as of writing, is minimal. This should be a pretty rich data
package when I’m done with it. Until then, you can do this to see what’s
in it.

``` r
data(package = "stevedata")
```

The ensuing output will look like this.

| **Object Name**          | **Title/Description**                                                       |
| :----------------------- | :-------------------------------------------------------------------------- |
| Arca                     | NYSE Arca Steel Index data, 2017–present                                    |
| DJIA                     | Dow Jones Industrial Average, 1885-Present                                  |
| DST                      | Casualties/Fatalities in the U.S. for Drunk-Driving, Suicide, and Terrorism |
| Datasaurus               | The Datasaurus Dozen                                                        |
| ESS9GB                   | British Attitudes Toward Immigration (2018-19)                              |
| LOTI                     | Land-Ocean Temperature Index, 1880-2020                                     |
| LTPT                     | Long-Term Price Trends for Computers, TVs, and Related Items                |
| LTWT                     | “Let Them Watch TV”                                                         |
| ODGI                     | Ozone Depleting Gas Index Data, 1992-2019                                   |
| Presidents               | U.S. Presidents and Their Terms in Office                                   |
| TV16                     | The Individual Correlates of the Trump Vote in 2016                         |
| aluminum\_premiums       | LME Aluminum Premiums Data                                                  |
| anes\_prochoice          | Abortion Attitudes (ANES, 2012)                                             |
| arcticseaice             | Arctic Sea Ice Extent Data, 1901-2015                                       |
| arg\_tariff              | Simple Mean Tariff Rate for Argentina                                       |
| asn\_stats               | Aviation Safety Network Statistics, 1942-2019                               |
| clemson\_temps           | Daily Clemson Temperature Data                                              |
| co2emissions             | Carbon Dioxide Emissions Data                                               |
| coffee\_imports          | Coffee Imports for Select Importing Countries                               |
| coffee\_price            | The Primary Commodity Price for Coffee (Arabica, Robustas)                  |
| election\_turnout        | State-Level Education and Voter Turnout in 2016                             |
| eq\_passengercars        | Export Quality Data for Passenger Cars, 1963-2014                           |
| eustates                 | EU Member States (Current as of 2019)                                       |
| fakeLogit                | Fake Data for a Logistic Regression                                         |
| fakeTSCS                 | Fake Data for a Time-Series Cross-Section                                   |
| fakeTSD                  | Fake Data for a Time-Series                                                 |
| ghp100k                  | Gun Homicide Rate per 100,000 People, by Country                            |
| gss\_abortion            | Abortion Opinions in the General Social Survey                              |
| gss\_wages               | The Gender Pay Gap in the General Social Survey                             |
| mvprod                   | Motor Vehicle Production by Country, 1950-2019                              |
| quartets                 | Anscombe’s (1973) Quartets                                                  |
| recessions               | United States Recessions, 1855-present                                      |
| sealevels                | Global Average Absolute Sea Level Change, 1880–2015                         |
| so2concentrations        | Sulfur Dioxide Emissions, 1980-2017                                         |
| steves\_clothes          | Steve’s (Professional) Clothes, as of March 3, 2019                         |
| sugar\_price             | IMF Primary Commodity Price Data for Sugar                                  |
| uniondensity             | Cross-National Rates of Trade Union Density                                 |
| usa\_chn\_gdp\_forecasts | United States-China GDP and GDP Forecasts, 1960-2050                        |
| usa\_computers           | Percentage of U.S. Households with Computer Access, by Year                 |
| usa\_states              | State Abbreviations, Names, and Regions/Divisions                           |
| wvs\_ccodes              | Syncing Word Values Survey Country Codes with CoW Codes                     |
| wvs\_immig               | Attitudes about Immigration in the World Values Survey                      |
| yugo\_sales              | Yugo Sales in the United States, 1985-1992                                  |

Here is a simple scraping job to provide more information (by way of the
`description` field in the associated R Documentation file).

| **Object Name**          | **Description**                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| :----------------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Arca                     | Daily data on the NYSE Arca Steel Index. These data are useful for me in teaching how Trump’s 2018 steel tariffs didn’t do much good for the steel industry.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| DJIA                     | This data set contains the value of the Dow Jones Industrial Average on daily close for all available dates (to the best of my knowledge) from 1885 to the most recently concluded calendar year. Extensions shouldn’t be too difficult with existing packages.                                                                                                                                                                                                                                                                                                                                                                                                       |
| DST                      | These are fatalities (and, in the case of terrorism, casualties as well) for drunk-driving, suicide, and acts of terrorism in the U.S. spanning 1970 to 2018. Only one of these is sufficiently important to command public attention despite being the least severe public bad. Do you want to guess which one?                                                                                                                                                                                                                                                                                                                                                      |
| Datasaurus               | An illustrative exercise in never trusting the summary statistics without also visualizing them.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| ESS9GB                   | This is a replication data originally set to accompany a blog post and presentation to students at the University of Nottingham in March 2020. However, COVID-19 led to the cancellation of the talk.                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| LOTI                     | These data contain monthly mean temperature anomalies expressed as deviations from the corresponding 1951-1980 means. They are useful for showing how we can measure climate change.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| LTPT                     | These data are a monthly time-series of changes in the consumer price index relative to a Dec. 1997 starting date for televisions, computers, and related items. I use this as in-class illustration that globalization has made consumer electronics cheaper across the board for Americans.                                                                                                                                                                                                                                                                                                                                                                         |
| LTWT                     | These data contain price indices for various items for the general urban consumer. Categories include medical services, college tuition, college textbooks, child care, housing, food and beverages, all items (i.e. general CPI), new vehicles, apparel, and televisions. The base period in value was originally the 1982-4 average, but I converted the base period to January 2000. I use these data for in-class discussion about how liberalized trade has made consumer electronics (like TVs) fractions of their past prices. Yet, young adults face mounting costs for college, child-raising, and health care that government policy has failed to address. |
| ODGI                     | The NOAA Earth System Research Laboratory has an “ozone depleting gas index” (ODGI) data set from 1992 to 2018. This dataset summarizes Table 1 and Table 2 from its website. The primary interest here (for my purposes) is the ODGI indices (including the new 2012 measure). The data set includes constituent greenhouse gases/chlorines as well in parts per trillion. The primary use here is for in-class illustration.                                                                                                                                                                                                                                        |
| Presidents               | This should be self-evident. Here are all U.S. presidents who have completed their terms in office (i.e. excluding the current one).                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| TV16                     | These data come from the 2016 CCES and allow interested students to model the individual correlates of the Trump vote in 2016. Code/analysis heavily indebted to a 2017 analysis I did on my blog (see references).                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| aluminum\_premiums       | A near daily data set on the price of aluminum premiums (USD/MT) for LME in the U.S., Western Europe, East Asia, and Southeast Asia. I like these data as illustrative of some of the shortsightedness of the aluminum tariffs that Donald Trump announced in March 2018. The tariffs had no discernible effect on manufacturing employment or earnings, but they created a supply shock that made aluminum more expensive.                                                                                                                                                                                                                                           |
| anes\_prochoice          | A simple data set for in-class illustration about how to estimate and interpret interactive relationships. The data here are deliberately minimal for that end.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| arcticseaice             | This data set from Connelly et al. (2017) measures the Arctic sea ice extent in 10^6 square kilometers. It includes lower bounds and upper bounds on annual averages.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| arg\_tariff              | Simple mean tariff rate for Argentina, starting in 1980. The goal is to keep these data current.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| asn\_stats               | These are yearly counts on air accidents and fatalities, including measures for corporate jet accidents and hijackings. The hijackings are of particular interest to me, at least from a historical terrorism perspective.                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| clemson\_temps           | This data set contains daily temperatures (highs) for Clemson, South Carolina from Jan. 1, 1930 to the end of the most recent calendar year. The goal is to update this periodically with new data for as long as I live in this town.                                                                                                                                                                                                                                                                                                                                                                                                                                |
| co2emissions             | This is a sample data set, cobbled from various sources, about carbon dioxide emissions in the history of the planet from 800,000 BCE to the most recently concluded calendar year. I use this for a data visualization example for a lecture on climate change and international politics. Data communicate yearly averages/estimates.                                                                                                                                                                                                                                                                                                                               |
| coffee\_imports          | A simple time series on coffee imports for select importing countries (i.e. European Union + Japan + Russia + Tunisia + United States).                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| coffee\_price            | This is primary commodity price data for coffee (Arabica, Robustas) from 1980 to the present. I manually update these data since FRED’s coverage since 2017 has been spotty.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| election\_turnout        | A simple data set on education and state-level (+ DC) turnout in the 2016 presidential election. This is inspired by what Pollock (2012) does in his book.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| eq\_passengercars        | Data from the International Monetary Fund for the export quality and unit/trade value of passenger cars for all available countries and years from 1963 to 2014.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| eustates                 | European Union membership by accession date                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| fakeLogit                | This is a simple fake data set to illustrate a logistic regression.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| fakeTSCS                 | This is a toy (i.e. “fake”) data set created by the fabricatr package. There are 100 observations for 25 hypothetical countries. The outcome y is a linear function of a baseline for each hypothetical country, plus a yearly growth trend as well as varying growth errors for each country. x1 is supposed to have a linear effect of .5 on y, all things considered. x2 is supposed to have a linear effect of 1 on y for each unit change in x2, all things considered.                                                                                                                                                                                          |
| fakeTSD                  | This is a toy (i.e. “fake”) data set created by the fabricatr package. There are 100 observations. The outcome y is a linear function of 20 + (.25 \* year) + .(25 \* x1) + (1 \* x2) + e. This clearly implies some autocorrelation in the data. I.e. it’s a time-series.                                                                                                                                                                                                                                                                                                                                                                                            |
| ghp100k                  | This is the yearly rate of gun homicides per 100,000 people in the population, selecting on “Western” countries of interest.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| gss\_abortion            | This is a toy data set derived from the General Social Survey that I intend to use for several purposes. First, the battery of abortion items can serve as toy data to illustrate mixed effects modeling as equivalent to a one-parameter (Rasch) model. Second, I include some covariates to also do some basic regressions. I think abortion opinions are useful learning tools for statistical inference for college students. Third, there’s a time-series component as well for understanding how abortion attitudes have changed over time.                                                                                                                     |
| gss\_wages               | Wage data from the General Social Survey (1974-2018) to illustrate wage discrepancies by gender (while also considering respondent occupation, age, and education).                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| mvprod                   | Data, largely from Organisation Internationale des Constructeurs d’Automobiles (OICA), on motor vehicle production in various countries (and the world totals) from 1950 to 2019 at various intervals. Tallies include production of passenger cars, light commercial vehicles, minibuses, trucks, buses and coaches.                                                                                                                                                                                                                                                                                                                                                 |
| quartets                 | These are four x-y data sets, combined into a long format, which have the same traditional statistical properties (mean, variance, correlation, regression line, etc.). However, they look quite different.                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| recessions               | Data on U.S. recessions, past to present. Data include information on contraction, expansion, and cycle.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| sealevels                | These data describe how sea level has changed over time, in both relative and absolute terms. Absolute sea level change refers to the height of the ocean surface regardless of whether nearby land is rising or falling.                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| so2concentrations        | This data set contains yearly observations by the Environmental Protection Agency on the concentration of sulfur dioxide in parts per billion, based on 35 sites. I use this for in-class illustration. Note that the national standard is 75 parts per billion.                                                                                                                                                                                                                                                                                                                                                                                                      |
| steves\_clothes          | I cobbled together this data set of the professional clothes (polos, long-sleeve dress shirts, pants) in my closet, largely for illustration on the origins of apparel in the U.S. for an intro lecture on trade.                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| sugar\_price             | This is primary commodity price data for sugar globally, in the United States, and in Europe for every month from 1980 to (roughly) the present. Prices are nominal U.S. cents per pound and are not seasonally adjusted (“NSA”).                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| uniondensity             | Cross-national data on relative size of the trade unions and predictors in 20 countries. This is a data set of interest to replicating Western and Jackman (1994), who themselves were addressing a debate between Wallerstein and Stephens on which of two highly correlated predictors explains trade union density.                                                                                                                                                                                                                                                                                                                                                |
| usa\_chn\_gdp\_forecasts | This is a toy data set to examine the time in which we should expect China to overtake the United States in total gross domestic product (GDP), given current trends. It includes an OECD long-term GDP forecast from 2014, and forecasts from the forecast and prophet packages in R.                                                                                                                                                                                                                                                                                                                                                                                |
| usa\_computers           | This is a simple and regrettably incomplete time-series on the percentage of U.S. households with access to a computer, by year.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| usa\_states              | A simple data set from state.abb, state.name, state.region, and state.division (+ District of Columbia). I’d rather just have all these in one place.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| wvs\_ccodes              | A simple data set that syncs World Values Survey country codes (s003) with corresponding country codes from the Correlates of War state system membership data.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| wvs\_immig               | A data set on attitudes about immigration for all observations in the third to sixth wave of the World Values Survey. I use these data for in-class illustration.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| yugo\_sales              | A data set on Yugo sales vis-a-vis two competing models in the United States from 1985 to 1992.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
