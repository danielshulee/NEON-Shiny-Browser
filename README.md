# NEON-Shiny-Browser

A multifunctional R Shiny tool designed to make NEON data accessible, visualized, and easy to interact with

### Install and Run

To install, change the working directory on your shell to the desired directory, and clone from git:

```
cd /Desktop
git clone https://github.com/Danielslee51/NEON-Shiny-Browser
```

Open an instance of RStudio and navigate to the `/NEON-Shiny-Browser` folder

Click and run `server.R`

## Package Requirements

[Download](https://cran.r-project.org/) the latest version of R, and [RStudio](https://www.rstudio.com/) for your local or virtual machine.

A few packages need to be downloaded: <br>
* [`leaflet`](https://github.com/rstudio/leaflet) and [`leaflet.extras`](https://github.com/bhaskarvk/leaflet.extras): These are responsible for the map and its features.
* [`devtools`](https://cran.r-project.org/web/packages/devtools/index.html): For installing packages from Github.
* [`neonUtilities`](https://github.com/NEONScience/NEON-utilities/tree/master/neonUtilities) and [`nneo`](https://github.com/ropensci/nneo): used to pull datasets from NEON.
* [`shinythemes`](https://github.com/rstudio/shinythemes): alter the appearance of the Shiny app. 
* [`shinyWidgets`](https://github.com/dreamRs/shinyWidgets): provides costumized and "pimp[ed]" up widgets for shiny.
* [`sf`](https://github.com/r-spatial/sf) and [`rgdal`](https://github.com/cran/rgdal): provide access to simple feature geometries.
* [`jsonlite`](https://github.com/cran/jsonlite): helps deal with JSON structures.

```
install.packages(c('leaflet','leaflet.extras','devtools','nneo','shinythemes','shinyWidgets','sf','rgdal','jsonlite'))
devtools::install_github("NEONScience/NEON-utilities/neonUtilities", dependencies=TRUE)
```

**Note: [Mac OS X](https://cran.r-project.org/bin/macosx/tools/) currently requires `gfortran` and `clang` be installed in addition to the latest version of R (v3.5.1 "Feather Spray")** 
