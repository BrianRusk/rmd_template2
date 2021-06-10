---
title: "Test"
author: "Brian Rusk"
date: "30/05/2021"
output: 
    html_document:
        pandoc_args: [
        "--title-prefix", "Foo", 
        "--id-prefix", "Bar"
        ]
        keep_md: true
        theme: spacelab
        highlight: pygments
        toc: true
        toc_float: true
---



# Some math features {.tabset .tabset-fade .tabset-pills}

## A basic formula

$$f(k) = {n \choose k} p^{k} (1-p)^{n-k}$$

## An array

$$\begin{array}{ccc}
x_{11} & x_{12} & x_{13}\\
x_{11} & x_{12} & x_{13}
\end{array}$$

## A p matrix

$$\Theta = \begin{pmatrix}\alpha & \beta\\
\gamma & \delta
\end{pmatrix}$$

## A b matrix

$$X = \begin{bmatrix}
1 & x_{1}\\
1 & x_{2}\\
1 & x_{3}
\end{bmatrix}$$

# Leaflet Maps {.tabset}

## Tainan Home


```r
library(leaflet)
leaflet() %>% addTiles() %>%
  setView(120.209, 23.018, zoom = 17) %>%
  addPopups(
    120.209, 23.018,
    'Here is my home.'
  )
```

```{=html}
<div id="htmlwidget-001f6c44fac75477b75b" style="width:100%;height:480px;" class="leaflet html-widget"></div>
<script type="application/json" data-for="htmlwidget-001f6c44fac75477b75b">{"x":{"options":{"crs":{"crsClass":"L.CRS.EPSG3857","code":null,"proj4def":null,"projectedBounds":null,"options":{}}},"calls":[{"method":"addTiles","args":["//{s}.tile.openstreetmap.org/{z}/{x}/{y}.png",null,null,{"minZoom":0,"maxZoom":18,"tileSize":256,"subdomains":"abc","errorTileUrl":"","tms":false,"noWrap":false,"zoomOffset":0,"zoomReverse":false,"opacity":1,"zIndex":1,"detectRetina":false,"attribution":"&copy; <a href=\"http://openstreetmap.org\">OpenStreetMap<\/a> contributors, <a href=\"http://creativecommons.org/licenses/by-sa/2.0/\">CC-BY-SA<\/a>"}]},{"method":"addPopups","args":[23.018,120.209,"Here is my home.",null,null,{"maxWidth":300,"minWidth":50,"autoPan":true,"keepInView":false,"closeButton":true,"className":""}]}],"setView":[[23.018,120.209],17,[]],"limits":{"lat":[23.018,23.018],"lng":[120.209,120.209]}},"evals":[],"jsHooks":[]}</script>
```
## Gran's House


```{=html}
<div id="htmlwidget-82985952949e3ef738a7" style="width:100%;height:480px;" class="leaflet html-widget"></div>
<script type="application/json" data-for="htmlwidget-82985952949e3ef738a7">{"x":{"options":{"crs":{"crsClass":"L.CRS.EPSG3857","code":null,"proj4def":null,"projectedBounds":null,"options":{}}},"calls":[{"method":"addTiles","args":["//{s}.tile.openstreetmap.org/{z}/{x}/{y}.png",null,null,{"minZoom":0,"maxZoom":18,"tileSize":256,"subdomains":"abc","errorTileUrl":"","tms":false,"noWrap":false,"zoomOffset":0,"zoomReverse":false,"opacity":1,"zIndex":1,"detectRetina":false,"attribution":"&copy; <a href=\"http://openstreetmap.org\">OpenStreetMap<\/a> contributors, <a href=\"http://creativecommons.org/licenses/by-sa/2.0/\">CC-BY-SA<\/a>"}]},{"method":"addPopups","args":[49.0465,-122.30084,"Here is my Gran's home.",null,null,{"maxWidth":300,"minWidth":50,"autoPan":true,"keepInView":false,"closeButton":true,"className":""}]}],"setView":[[49.047,-122.301],17,[]],"limits":{"lat":[49.0465,49.0465],"lng":[-122.30084,-122.30084]}},"evals":[],"jsHooks":[]}</script>
```
