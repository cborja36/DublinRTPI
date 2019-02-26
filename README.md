# DublinRTPI
Real-time Passenger Information for Dublin city's public transport.  


Code to retrieve real time information about Dublin Bus and Dart services. Allows the aggregation of multiple bus stops.  
**No Luas info currently.**


## Shiny App

The code located in [ShinyApp](/ShinyApp) is an interactive app which will retrieve and display information about the bus and train services in Dublin.  

A live version of the app should be running at [https://aboland.shinyapps.io/DublinTransport/](https://aboland.shinyapps.io/DublinTransport/)

#### Custom URL

A custom url can be used to preload the application with your choices of stops and buses. This can be bookmarked to save time.  
Example: [http://aboland.shinyapps.io:/DublinTransport/?stops=334,336&routes=14,140](http://aboland.shinyapps.io:/DublinTransport/?stops=334,336&routes=14,140)

### Run Locally

The Shiny app can be run locally from within R or RStudio. *The Shiny library must be installed.*  

```r
# install.packages("shiny")
library(shiny)  
runGitHub("aboland/DublinRTPI", subdir = "ShinyApp")
```