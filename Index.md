---
title       : Beaches of Britanny, France
subtitle    : Locate and get average temperature
author      : tardive5
job         : Data Scientist student
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : [bootstrap, shiny, interactive] # {mathjax, quiz, bootstrap}
ext_widgets: {rCharts: [libraries/nvd3]}
mode        : selfcontained # {selfcontained,standalone, draft}
knit        : slidify::knit2slides
---

## Myproject uses French tourism open data to show 

1. A sample of beaches among 341 references 
2. These beaches location on a Google map
3. Average temperature of the sample

## Source

"Beaches of Brittany" is a simple open data produced by offices of tourism.

source URL: http://www.data-tourisme-bretagne.com/web/guest/data

For the demo, "invented" air temperature per beach, in celsius degrees, has been added.

Further agreement with institutions will be needed to collect more open real data.

--- .class #id 

## Inputs

Sampling is possible in 2 ways:

<h3> 1.Selecting one or several areas of Britanny </h3>

Areas names are not official but they are quite easy to understand.

<h3> 2. Giving a number of samples among the selected areas</h3>

That helps for visibility on the map and can be useful for further experience.

--- .class #id 

## Outputs

<h3> 1. A Google map enables easy visualization of beaches </h3> 

Each tip designates the town where beach is located. Some lucky towns have several beaches.

<h3> 2. The average air temperature of the samples given in Celsius degrees </h3>

<br>
<img src="appsimage.jpg" align="middle" alt="A view of myproject apps">

--- .class #id 

## Next steps !
Richer open data can definitely provide useful statistics for sea and tourism professionals.
For ex., we could imagine correlation between the number of cars parked around beaches and temperatures per area. 



<div id = 'extraPlot' class = 'rChart nvd3'></div>
<script type='text/javascript'>
 $(document).ready(function(){
      drawextraPlot()
    });
    function drawextraPlot(){  
      var opts = {
 "dom": "extraPlot",
"width":    800,
"height":    400,
"x": "TEMP",
"y": "NBCAR",
"group": "AREA",
"type": "multiBarChart",
"id": "extraPlot" 
},
        data = [
 {
 "AREA": "South Coast",
"TEMP": 17,
"NBCAR": 277 
},
{
 "AREA": "South Coast",
"TEMP": 17,
"NBCAR": 111 
},
{
 "AREA": "South Coast",
"TEMP": 17,
"NBCAR": 173 
},
{
 "AREA": "South Coast",
"TEMP": 17,
"NBCAR": 88 
},
{
 "AREA": "South Coast",
"TEMP": 17,
"NBCAR": 92 
},
{
 "AREA": "South Coast",
"TEMP": 17,
"NBCAR": 96 
},
{
 "AREA": "South Coast",
"TEMP": 17,
"NBCAR": 344 
},
{
 "AREA": "South Coast",
"TEMP": 17,
"NBCAR": 104 
},
{
 "AREA": "South Coast",
"TEMP": 17,
"NBCAR": 220 
},
{
 "AREA": "South Coast",
"TEMP": 17,
"NBCAR": 196 
},
{
 "AREA": "South Coast",
"TEMP": 17,
"NBCAR": 126 
},
{
 "AREA": "South Coast",
"TEMP": 17,
"NBCAR": 247 
},
{
 "AREA": "South Coast",
"TEMP": 17,
"NBCAR": 289 
},
{
 "AREA": "South Coast",
"TEMP": 17,
"NBCAR": 221 
},
{
 "AREA": "South Coast",
"TEMP": 17,
"NBCAR": 211 
},
{
 "AREA": "South Coast",
"TEMP": 17,
"NBCAR": 219 
},
{
 "AREA": "South Coast",
"TEMP": 17,
"NBCAR": 312 
},
{
 "AREA": "South Coast",
"TEMP": 17,
"NBCAR": 163 
},
{
 "AREA": "The most beautiful",
"TEMP": 17,
"NBCAR": 65 
},
{
 "AREA": "The most beautiful",
"TEMP": 17,
"NBCAR": 234 
},
{
 "AREA": "The most beautiful",
"TEMP": 17,
"NBCAR": 259 
},
{
 "AREA": "The most beautiful",
"TEMP": 17,
"NBCAR": 187 
},
{
 "AREA": "The most beautiful",
"TEMP": 17,
"NBCAR": 295 
},
{
 "AREA": "The most beautiful",
"TEMP": 17,
"NBCAR": 44 
},
{
 "AREA": "The most beautiful",
"TEMP": 17,
"NBCAR": 189 
},
{
 "AREA": "The most beautiful",
"TEMP": 17,
"NBCAR": 235 
},
{
 "AREA": "The most beautiful",
"TEMP": 17,
"NBCAR": 223 
},
{
 "AREA": "The most beautiful",
"TEMP": 17,
"NBCAR": 146 
},
{
 "AREA": "The most beautiful",
"TEMP": 17,
"NBCAR": 94 
},
{
 "AREA": "The most beautiful",
"TEMP": 17,
"NBCAR": 246 
},
{
 "AREA": "The most beautiful",
"TEMP": 17,
"NBCAR": 192 
},
{
 "AREA": "The most beautiful",
"TEMP": 17,
"NBCAR": 156 
},
{
 "AREA": "The most beautiful",
"TEMP": 17,
"NBCAR": 265 
},
{
 "AREA": "In front of Canada",
"TEMP": 17,
"NBCAR": 51 
},
{
 "AREA": "In front of Canada",
"TEMP": 17,
"NBCAR": 255 
},
{
 "AREA": "In front of Canada",
"TEMP": 17,
"NBCAR": 61 
},
{
 "AREA": "In front of Canada",
"TEMP": 17,
"NBCAR": 120 
},
{
 "AREA": "In front of Canada",
"TEMP": 17,
"NBCAR": 72 
},
{
 "AREA": "In front of Canada",
"TEMP": 17,
"NBCAR": 296 
},
{
 "AREA": "In front of Canada",
"TEMP": 17,
"NBCAR": 133 
},
{
 "AREA": "In front of Canada",
"TEMP": 17,
"NBCAR": 202 
},
{
 "AREA": "In front of Canada",
"TEMP": 17,
"NBCAR": 76 
},
{
 "AREA": "In front of Canada",
"TEMP": 17,
"NBCAR": 130 
},
{
 "AREA": "In front of Canada",
"TEMP": 17,
"NBCAR": 298 
},
{
 "AREA": "In front of Canada",
"TEMP": 17,
"NBCAR": 83 
},
{
 "AREA": "In front of Jersey",
"TEMP": 17,
"NBCAR": 142 
},
{
 "AREA": "In front of Jersey",
"TEMP": 17,
"NBCAR": 242 
},
{
 "AREA": "In front of Jersey",
"TEMP": 17,
"NBCAR": 149 
},
{
 "AREA": "South Coast",
"TEMP": 18,
"NBCAR": 258 
},
{
 "AREA": "South Coast",
"TEMP": 18,
"NBCAR": 98 
},
{
 "AREA": "South Coast",
"TEMP": 18,
"NBCAR": 342 
},
{
 "AREA": "South Coast",
"TEMP": 18,
"NBCAR": 323 
},
{
 "AREA": "South Coast",
"TEMP": 18,
"NBCAR": 270 
},
{
 "AREA": "South Coast",
"TEMP": 18,
"NBCAR": 112 
},
{
 "AREA": "South Coast",
"TEMP": 18,
"NBCAR": 231 
},
{
 "AREA": "South Coast",
"TEMP": 18,
"NBCAR": 92 
},
{
 "AREA": "South Coast",
"TEMP": 18,
"NBCAR": 288 
},
{
 "AREA": "South Coast",
"TEMP": 18,
"NBCAR": 162 
},
{
 "AREA": "South Coast",
"TEMP": 18,
"NBCAR": 210 
},
{
 "AREA": "South Coast",
"TEMP": 18,
"NBCAR": 265 
},
{
 "AREA": "South Coast",
"TEMP": 18,
"NBCAR": 238 
},
{
 "AREA": "South Coast",
"TEMP": 18,
"NBCAR": 139 
},
{
 "AREA": "South Coast",
"TEMP": 18,
"NBCAR": 82 
},
{
 "AREA": "South Coast",
"TEMP": 18,
"NBCAR": 262 
},
{
 "AREA": "South Coast",
"TEMP": 18,
"NBCAR": 145 
},
{
 "AREA": "South Coast",
"TEMP": 18,
"NBCAR": 264 
},
{
 "AREA": "The most beautiful",
"TEMP": 18,
"NBCAR": 298 
},
{
 "AREA": "The most beautiful",
"TEMP": 18,
"NBCAR": 63 
},
{
 "AREA": "The most beautiful",
"TEMP": 18,
"NBCAR": 141 
},
{
 "AREA": "The most beautiful",
"TEMP": 18,
"NBCAR": 83 
},
{
 "AREA": "The most beautiful",
"TEMP": 18,
"NBCAR": 72 
},
{
 "AREA": "The most beautiful",
"TEMP": 18,
"NBCAR": 267 
},
{
 "AREA": "The most beautiful",
"TEMP": 18,
"NBCAR": 214 
},
{
 "AREA": "The most beautiful",
"TEMP": 18,
"NBCAR": 44 
},
{
 "AREA": "The most beautiful",
"TEMP": 18,
"NBCAR": 53 
},
{
 "AREA": "The most beautiful",
"TEMP": 18,
"NBCAR": 282 
},
{
 "AREA": "The most beautiful",
"TEMP": 18,
"NBCAR": 75 
},
{
 "AREA": "The most beautiful",
"TEMP": 18,
"NBCAR": 183 
},
{
 "AREA": "The most beautiful",
"TEMP": 18,
"NBCAR": 75 
},
{
 "AREA": "The most beautiful",
"TEMP": 18,
"NBCAR": 135 
},
{
 "AREA": "The most beautiful",
"TEMP": 18,
"NBCAR": 125 
},
{
 "AREA": "The most beautiful",
"TEMP": 18,
"NBCAR": 174 
},
{
 "AREA": "In front of Canada",
"TEMP": 18,
"NBCAR": 292 
},
{
 "AREA": "In front of Canada",
"TEMP": 18,
"NBCAR": 162 
},
{
 "AREA": "In front of Canada",
"TEMP": 18,
"NBCAR": 193 
},
{
 "AREA": "In front of Canada",
"TEMP": 18,
"NBCAR": 88 
},
{
 "AREA": "In front of Canada",
"TEMP": 18,
"NBCAR": 172 
},
{
 "AREA": "In front of Canada",
"TEMP": 18,
"NBCAR": 220 
},
{
 "AREA": "In front of Canada",
"TEMP": 18,
"NBCAR": 136 
},
{
 "AREA": "In front of Canada",
"TEMP": 18,
"NBCAR": 166 
},
{
 "AREA": "In front of Jersey",
"TEMP": 18,
"NBCAR": 213 
},
{
 "AREA": "In front of Jersey",
"TEMP": 18,
"NBCAR": 164 
},
{
 "AREA": "In front of Jersey",
"TEMP": 18,
"NBCAR": 185 
},
{
 "AREA": "In front of Jersey",
"TEMP": 18,
"NBCAR": 53 
},
{
 "AREA": "South Coast",
"TEMP": 19,
"NBCAR": 163 
},
{
 "AREA": "South Coast",
"TEMP": 19,
"NBCAR": 132 
},
{
 "AREA": "South Coast",
"TEMP": 19,
"NBCAR": 124 
},
{
 "AREA": "South Coast",
"TEMP": 19,
"NBCAR": 209 
},
{
 "AREA": "South Coast",
"TEMP": 19,
"NBCAR": 235 
},
{
 "AREA": "South Coast",
"TEMP": 19,
"NBCAR": 135 
},
{
 "AREA": "South Coast",
"TEMP": 19,
"NBCAR": 98 
},
{
 "AREA": "South Coast",
"TEMP": 19,
"NBCAR": 238 
},
{
 "AREA": "South Coast",
"TEMP": 19,
"NBCAR": 110 
},
{
 "AREA": "South Coast",
"TEMP": 19,
"NBCAR": 237 
},
{
 "AREA": "South Coast",
"TEMP": 19,
"NBCAR": 261 
},
{
 "AREA": "South Coast",
"TEMP": 19,
"NBCAR": 287 
},
{
 "AREA": "South Coast",
"TEMP": 19,
"NBCAR": 216 
},
{
 "AREA": "South Coast",
"TEMP": 19,
"NBCAR": 129 
},
{
 "AREA": "South Coast",
"TEMP": 19,
"NBCAR": 155 
},
{
 "AREA": "South Coast",
"TEMP": 19,
"NBCAR": 112 
},
{
 "AREA": "South Coast",
"TEMP": 19,
"NBCAR": 201 
},
{
 "AREA": "South Coast",
"TEMP": 19,
"NBCAR": 263 
},
{
 "AREA": "South Coast",
"TEMP": 19,
"NBCAR": 345 
},
{
 "AREA": "South Coast",
"TEMP": 19,
"NBCAR": 180 
},
{
 "AREA": "The most beautiful",
"TEMP": 19,
"NBCAR": 188 
},
{
 "AREA": "The most beautiful",
"TEMP": 19,
"NBCAR": 143 
},
{
 "AREA": "The most beautiful",
"TEMP": 19,
"NBCAR": 284 
},
{
 "AREA": "The most beautiful",
"TEMP": 19,
"NBCAR": 34 
},
{
 "AREA": "The most beautiful",
"TEMP": 19,
"NBCAR": 197 
},
{
 "AREA": "The most beautiful",
"TEMP": 19,
"NBCAR": 129 
},
{
 "AREA": "The most beautiful",
"TEMP": 19,
"NBCAR": 246 
},
{
 "AREA": "The most beautiful",
"TEMP": 19,
"NBCAR": 259 
},
{
 "AREA": "The most beautiful",
"TEMP": 19,
"NBCAR": 85 
},
{
 "AREA": "The most beautiful",
"TEMP": 19,
"NBCAR": 159 
},
{
 "AREA": "The most beautiful",
"TEMP": 19,
"NBCAR": 139 
},
{
 "AREA": "The most beautiful",
"TEMP": 19,
"NBCAR": 35 
},
{
 "AREA": "The most beautiful",
"TEMP": 19,
"NBCAR": 180 
},
{
 "AREA": "The most beautiful",
"TEMP": 19,
"NBCAR": 84 
},
{
 "AREA": "The most beautiful",
"TEMP": 19,
"NBCAR": 234 
},
{
 "AREA": "The most beautiful",
"TEMP": 19,
"NBCAR": 56 
},
{
 "AREA": "The most beautiful",
"TEMP": 19,
"NBCAR": 30 
},
{
 "AREA": "The most beautiful",
"TEMP": 19,
"NBCAR": 284 
},
{
 "AREA": "The most beautiful",
"TEMP": 19,
"NBCAR": 30 
},
{
 "AREA": "The most beautiful",
"TEMP": 19,
"NBCAR": 277 
},
{
 "AREA": "In front of Canada",
"TEMP": 19,
"NBCAR": 223 
},
{
 "AREA": "In front of Canada",
"TEMP": 19,
"NBCAR": 124 
},
{
 "AREA": "In front of Canada",
"TEMP": 19,
"NBCAR": 222 
},
{
 "AREA": "In front of Canada",
"TEMP": 19,
"NBCAR": 287 
},
{
 "AREA": "In front of Canada",
"TEMP": 19,
"NBCAR": 186 
},
{
 "AREA": "In front of Canada",
"TEMP": 19,
"NBCAR": 32 
},
{
 "AREA": "In front of Canada",
"TEMP": 19,
"NBCAR": 292 
},
{
 "AREA": "In front of Canada",
"TEMP": 19,
"NBCAR": 113 
},
{
 "AREA": "In front of Canada",
"TEMP": 19,
"NBCAR": 284 
},
{
 "AREA": "In front of Canada",
"TEMP": 19,
"NBCAR": 255 
},
{
 "AREA": "In front of Canada",
"TEMP": 19,
"NBCAR": 181 
},
{
 "AREA": "In front of Canada",
"TEMP": 19,
"NBCAR": 80 
},
{
 "AREA": "In front of Canada",
"TEMP": 19,
"NBCAR": 173 
},
{
 "AREA": "In front of Canada",
"TEMP": 19,
"NBCAR": 218 
},
{
 "AREA": "In front of Canada",
"TEMP": 19,
"NBCAR": 133 
},
{
 "AREA": "In front of Canada",
"TEMP": 19,
"NBCAR": 93 
},
{
 "AREA": "In front of Jersey",
"TEMP": 19,
"NBCAR": 142 
},
{
 "AREA": "In front of Jersey",
"TEMP": 19,
"NBCAR": 120 
},
{
 "AREA": "In front of Jersey",
"TEMP": 19,
"NBCAR": 134 
},
{
 "AREA": "In front of Jersey",
"TEMP": 19,
"NBCAR": 203 
},
{
 "AREA": "South Coast",
"TEMP": 20,
"NBCAR": 170 
},
{
 "AREA": "South Coast",
"TEMP": 20,
"NBCAR": 165 
},
{
 "AREA": "South Coast",
"TEMP": 20,
"NBCAR": 125 
},
{
 "AREA": "South Coast",
"TEMP": 20,
"NBCAR": 254 
},
{
 "AREA": "South Coast",
"TEMP": 20,
"NBCAR": 169 
},
{
 "AREA": "South Coast",
"TEMP": 20,
"NBCAR": 137 
},
{
 "AREA": "South Coast",
"TEMP": 20,
"NBCAR": 170 
},
{
 "AREA": "South Coast",
"TEMP": 20,
"NBCAR": 150 
},
{
 "AREA": "South Coast",
"TEMP": 20,
"NBCAR": 184 
},
{
 "AREA": "South Coast",
"TEMP": 20,
"NBCAR": 135 
},
{
 "AREA": "South Coast",
"TEMP": 20,
"NBCAR": 234 
},
{
 "AREA": "South Coast",
"TEMP": 20,
"NBCAR": 90 
},
{
 "AREA": "South Coast",
"TEMP": 20,
"NBCAR": 249 
},
{
 "AREA": "South Coast",
"TEMP": 20,
"NBCAR": 214 
},
{
 "AREA": "South Coast",
"TEMP": 20,
"NBCAR": 116 
},
{
 "AREA": "South Coast",
"TEMP": 20,
"NBCAR": 299 
},
{
 "AREA": "South Coast",
"TEMP": 20,
"NBCAR": 272 
},
{
 "AREA": "South Coast",
"TEMP": 20,
"NBCAR": 162 
},
{
 "AREA": "South Coast",
"TEMP": 20,
"NBCAR": 255 
},
{
 "AREA": "South Coast",
"TEMP": 20,
"NBCAR": 273 
},
{
 "AREA": "South Coast",
"TEMP": 20,
"NBCAR": 278 
},
{
 "AREA": "South Coast",
"TEMP": 20,
"NBCAR": 262 
},
{
 "AREA": "The most beautiful",
"TEMP": 20,
"NBCAR": 218 
},
{
 "AREA": "The most beautiful",
"TEMP": 20,
"NBCAR": 181 
},
{
 "AREA": "The most beautiful",
"TEMP": 20,
"NBCAR": 38 
},
{
 "AREA": "The most beautiful",
"TEMP": 20,
"NBCAR": 238 
},
{
 "AREA": "The most beautiful",
"TEMP": 20,
"NBCAR": 98 
},
{
 "AREA": "The most beautiful",
"TEMP": 20,
"NBCAR": 203 
},
{
 "AREA": "The most beautiful",
"TEMP": 20,
"NBCAR": 31 
},
{
 "AREA": "The most beautiful",
"TEMP": 20,
"NBCAR": 265 
},
{
 "AREA": "The most beautiful",
"TEMP": 20,
"NBCAR": 42 
},
{
 "AREA": "The most beautiful",
"TEMP": 20,
"NBCAR": 232 
},
{
 "AREA": "The most beautiful",
"TEMP": 20,
"NBCAR": 279 
},
{
 "AREA": "The most beautiful",
"TEMP": 20,
"NBCAR": 295 
},
{
 "AREA": "The most beautiful",
"TEMP": 20,
"NBCAR": 219 
},
{
 "AREA": "The most beautiful",
"TEMP": 20,
"NBCAR": 147 
},
{
 "AREA": "The most beautiful",
"TEMP": 20,
"NBCAR": 112 
},
{
 "AREA": "In front of Canada",
"TEMP": 20,
"NBCAR": 95 
},
{
 "AREA": "In front of Canada",
"TEMP": 20,
"NBCAR": 36 
},
{
 "AREA": "In front of Canada",
"TEMP": 20,
"NBCAR": 149 
},
{
 "AREA": "In front of Canada",
"TEMP": 20,
"NBCAR": 289 
},
{
 "AREA": "In front of Canada",
"TEMP": 20,
"NBCAR": 243 
},
{
 "AREA": "In front of Canada",
"TEMP": 20,
"NBCAR": 80 
},
{
 "AREA": "In front of Canada",
"TEMP": 20,
"NBCAR": 220 
},
{
 "AREA": "In front of Canada",
"TEMP": 20,
"NBCAR": 33 
},
{
 "AREA": "In front of Canada",
"TEMP": 20,
"NBCAR": 103 
},
{
 "AREA": "In front of Canada",
"TEMP": 20,
"NBCAR": 191 
},
{
 "AREA": "In front of Jersey",
"TEMP": 20,
"NBCAR": 56 
},
{
 "AREA": "In front of Jersey",
"TEMP": 20,
"NBCAR": 64 
},
{
 "AREA": "In front of Jersey",
"TEMP": 20,
"NBCAR": 130 
},
{
 "AREA": "In front of Jersey",
"TEMP": 20,
"NBCAR": 78 
},
{
 "AREA": "In front of Jersey",
"TEMP": 20,
"NBCAR": 209 
},
{
 "AREA": "South Coast",
"TEMP": 21,
"NBCAR": 328 
},
{
 "AREA": "South Coast",
"TEMP": 21,
"NBCAR": 446 
},
{
 "AREA": "South Coast",
"TEMP": 21,
"NBCAR": 336 
},
{
 "AREA": "South Coast",
"TEMP": 21,
"NBCAR": 400 
},
{
 "AREA": "South Coast",
"TEMP": 21,
"NBCAR": 292 
},
{
 "AREA": "South Coast",
"TEMP": 21,
"NBCAR": 334 
},
{
 "AREA": "South Coast",
"TEMP": 21,
"NBCAR": 327 
},
{
 "AREA": "South Coast",
"TEMP": 21,
"NBCAR": 336 
},
{
 "AREA": "South Coast",
"TEMP": 21,
"NBCAR": 265 
},
{
 "AREA": "South Coast",
"TEMP": 21,
"NBCAR": 353 
},
{
 "AREA": "South Coast",
"TEMP": 21,
"NBCAR": 483 
},
{
 "AREA": "South Coast",
"TEMP": 21,
"NBCAR": 218 
},
{
 "AREA": "South Coast",
"TEMP": 21,
"NBCAR": 541 
},
{
 "AREA": "South Coast",
"TEMP": 21,
"NBCAR": 379 
},
{
 "AREA": "South Coast",
"TEMP": 21,
"NBCAR": 481 
},
{
 "AREA": "South Coast",
"TEMP": 21,
"NBCAR": 242 
},
{
 "AREA": "South Coast",
"TEMP": 21,
"NBCAR": 215 
},
{
 "AREA": "South Coast",
"TEMP": 21,
"NBCAR": 477 
},
{
 "AREA": "The most beautiful",
"TEMP": 21,
"NBCAR": 166 
},
{
 "AREA": "The most beautiful",
"TEMP": 21,
"NBCAR": 498 
},
{
 "AREA": "The most beautiful",
"TEMP": 21,
"NBCAR": 491 
},
{
 "AREA": "The most beautiful",
"TEMP": 21,
"NBCAR": 477 
},
{
 "AREA": "The most beautiful",
"TEMP": 21,
"NBCAR": 320 
},
{
 "AREA": "The most beautiful",
"TEMP": 21,
"NBCAR": 332 
},
{
 "AREA": "The most beautiful",
"TEMP": 21,
"NBCAR": 311 
},
{
 "AREA": "The most beautiful",
"TEMP": 21,
"NBCAR": 487 
},
{
 "AREA": "The most beautiful",
"TEMP": 21,
"NBCAR": 302 
},
{
 "AREA": "The most beautiful",
"TEMP": 21,
"NBCAR": 478 
},
{
 "AREA": "The most beautiful",
"TEMP": 21,
"NBCAR": 475 
},
{
 "AREA": "The most beautiful",
"TEMP": 21,
"NBCAR": 359 
},
{
 "AREA": "The most beautiful",
"TEMP": 21,
"NBCAR": 376 
},
{
 "AREA": "The most beautiful",
"TEMP": 21,
"NBCAR": 395 
},
{
 "AREA": "In front of Canada",
"TEMP": 21,
"NBCAR": 441 
},
{
 "AREA": "In front of Canada",
"TEMP": 21,
"NBCAR": 451 
},
{
 "AREA": "In front of Canada",
"TEMP": 21,
"NBCAR": 146 
},
{
 "AREA": "In front of Canada",
"TEMP": 21,
"NBCAR": 485 
},
{
 "AREA": "In front of Canada",
"TEMP": 21,
"NBCAR": 247 
},
{
 "AREA": "In front of Canada",
"TEMP": 21,
"NBCAR": 446 
},
{
 "AREA": "In front of Canada",
"TEMP": 21,
"NBCAR": 342 
},
{
 "AREA": "In front of Canada",
"TEMP": 21,
"NBCAR": 495 
},
{
 "AREA": "In front of Canada",
"TEMP": 21,
"NBCAR": 251 
},
{
 "AREA": "In front of Canada",
"TEMP": 21,
"NBCAR": 434 
},
{
 "AREA": "In front of Jersey",
"TEMP": 21,
"NBCAR": 455 
},
{
 "AREA": "In front of Jersey",
"TEMP": 21,
"NBCAR": 213 
},
{
 "AREA": "In front of Jersey",
"TEMP": 21,
"NBCAR": 455 
},
{
 "AREA": "South Coast",
"TEMP": 22,
"NBCAR": 435 
},
{
 "AREA": "South Coast",
"TEMP": 22,
"NBCAR": 395 
},
{
 "AREA": "South Coast",
"TEMP": 22,
"NBCAR": 456 
},
{
 "AREA": "South Coast",
"TEMP": 22,
"NBCAR": 286 
},
{
 "AREA": "South Coast",
"TEMP": 22,
"NBCAR": 352 
},
{
 "AREA": "South Coast",
"TEMP": 22,
"NBCAR": 511 
},
{
 "AREA": "South Coast",
"TEMP": 22,
"NBCAR": 356 
},
{
 "AREA": "South Coast",
"TEMP": 22,
"NBCAR": 509 
},
{
 "AREA": "South Coast",
"TEMP": 22,
"NBCAR": 389 
},
{
 "AREA": "South Coast",
"TEMP": 22,
"NBCAR": 404 
},
{
 "AREA": "South Coast",
"TEMP": 22,
"NBCAR": 349 
},
{
 "AREA": "South Coast",
"TEMP": 22,
"NBCAR": 225 
},
{
 "AREA": "South Coast",
"TEMP": 22,
"NBCAR": 271 
},
{
 "AREA": "South Coast",
"TEMP": 22,
"NBCAR": 458 
},
{
 "AREA": "The most beautiful",
"TEMP": 22,
"NBCAR": 339 
},
{
 "AREA": "The most beautiful",
"TEMP": 22,
"NBCAR": 249 
},
{
 "AREA": "The most beautiful",
"TEMP": 22,
"NBCAR": 293 
},
{
 "AREA": "The most beautiful",
"TEMP": 22,
"NBCAR": 429 
},
{
 "AREA": "The most beautiful",
"TEMP": 22,
"NBCAR": 313 
},
{
 "AREA": "The most beautiful",
"TEMP": 22,
"NBCAR": 116 
},
{
 "AREA": "The most beautiful",
"TEMP": 22,
"NBCAR": 321 
},
{
 "AREA": "The most beautiful",
"TEMP": 22,
"NBCAR": 160 
},
{
 "AREA": "In front of Canada",
"TEMP": 22,
"NBCAR": 338 
},
{
 "AREA": "In front of Canada",
"TEMP": 22,
"NBCAR": 192 
},
{
 "AREA": "In front of Canada",
"TEMP": 22,
"NBCAR": 245 
},
{
 "AREA": "In front of Canada",
"TEMP": 22,
"NBCAR": 353 
},
{
 "AREA": "In front of Canada",
"TEMP": 22,
"NBCAR": 224 
},
{
 "AREA": "In front of Canada",
"TEMP": 22,
"NBCAR": 128 
},
{
 "AREA": "In front of Canada",
"TEMP": 22,
"NBCAR": 288 
},
{
 "AREA": "In front of Canada",
"TEMP": 22,
"NBCAR": 319 
},
{
 "AREA": "In front of Canada",
"TEMP": 22,
"NBCAR": 316 
},
{
 "AREA": "In front of Canada",
"TEMP": 22,
"NBCAR": 152 
},
{
 "AREA": "In front of Jersey",
"TEMP": 22,
"NBCAR": 335 
},
{
 "AREA": "In front of Jersey",
"TEMP": 22,
"NBCAR": 200 
},
{
 "AREA": "In front of Jersey",
"TEMP": 22,
"NBCAR": 429 
},
{
 "AREA": "In front of Jersey",
"TEMP": 22,
"NBCAR": 166 
},
{
 "AREA": "In front of Jersey",
"TEMP": 22,
"NBCAR": 463 
},
{
 "AREA": "South Coast",
"TEMP": 23,
"NBCAR": 195 
},
{
 "AREA": "South Coast",
"TEMP": 23,
"NBCAR": 444 
},
{
 "AREA": "South Coast",
"TEMP": 23,
"NBCAR": 258 
},
{
 "AREA": "South Coast",
"TEMP": 23,
"NBCAR": 349 
},
{
 "AREA": "South Coast",
"TEMP": 23,
"NBCAR": 470 
},
{
 "AREA": "South Coast",
"TEMP": 23,
"NBCAR": 363 
},
{
 "AREA": "South Coast",
"TEMP": 23,
"NBCAR": 531 
},
{
 "AREA": "South Coast",
"TEMP": 23,
"NBCAR": 515 
},
{
 "AREA": "South Coast",
"TEMP": 23,
"NBCAR": 304 
},
{
 "AREA": "South Coast",
"TEMP": 23,
"NBCAR": 290 
},
{
 "AREA": "South Coast",
"TEMP": 23,
"NBCAR": 231 
},
{
 "AREA": "South Coast",
"TEMP": 23,
"NBCAR": 167 
},
{
 "AREA": "South Coast",
"TEMP": 23,
"NBCAR": 540 
},
{
 "AREA": "South Coast",
"TEMP": 23,
"NBCAR": 438 
},
{
 "AREA": "South Coast",
"TEMP": 23,
"NBCAR": 526 
},
{
 "AREA": "South Coast",
"TEMP": 23,
"NBCAR": 170 
},
{
 "AREA": "South Coast",
"TEMP": 23,
"NBCAR": 550 
},
{
 "AREA": "South Coast",
"TEMP": 23,
"NBCAR": 366 
},
{
 "AREA": "South Coast",
"TEMP": 23,
"NBCAR": 164 
},
{
 "AREA": "South Coast",
"TEMP": 23,
"NBCAR": 328 
},
{
 "AREA": "The most beautiful",
"TEMP": 23,
"NBCAR": 357 
},
{
 "AREA": "The most beautiful",
"TEMP": 23,
"NBCAR": 250 
},
{
 "AREA": "The most beautiful",
"TEMP": 23,
"NBCAR": 295 
},
{
 "AREA": "The most beautiful",
"TEMP": 23,
"NBCAR": 450 
},
{
 "AREA": "The most beautiful",
"TEMP": 23,
"NBCAR": 436 
},
{
 "AREA": "The most beautiful",
"TEMP": 23,
"NBCAR": 295 
},
{
 "AREA": "The most beautiful",
"TEMP": 23,
"NBCAR": 400 
},
{
 "AREA": "The most beautiful",
"TEMP": 23,
"NBCAR": 400 
},
{
 "AREA": "The most beautiful",
"TEMP": 23,
"NBCAR": 448 
},
{
 "AREA": "The most beautiful",
"TEMP": 23,
"NBCAR": 380 
},
{
 "AREA": "The most beautiful",
"TEMP": 23,
"NBCAR": 355 
},
{
 "AREA": "The most beautiful",
"TEMP": 23,
"NBCAR": 112 
},
{
 "AREA": "The most beautiful",
"TEMP": 23,
"NBCAR": 364 
},
{
 "AREA": "The most beautiful",
"TEMP": 23,
"NBCAR": 124 
},
{
 "AREA": "The most beautiful",
"TEMP": 23,
"NBCAR": 377 
},
{
 "AREA": "The most beautiful",
"TEMP": 23,
"NBCAR": 278 
},
{
 "AREA": "The most beautiful",
"TEMP": 23,
"NBCAR": 399 
},
{
 "AREA": "The most beautiful",
"TEMP": 23,
"NBCAR": 262 
},
{
 "AREA": "The most beautiful",
"TEMP": 23,
"NBCAR": 312 
},
{
 "AREA": "In front of Canada",
"TEMP": 23,
"NBCAR": 416 
},
{
 "AREA": "In front of Canada",
"TEMP": 23,
"NBCAR": 117 
},
{
 "AREA": "In front of Canada",
"TEMP": 23,
"NBCAR": 210 
},
{
 "AREA": "In front of Canada",
"TEMP": 23,
"NBCAR": 146 
},
{
 "AREA": "In front of Canada",
"TEMP": 23,
"NBCAR": 479 
},
{
 "AREA": "In front of Canada",
"TEMP": 23,
"NBCAR": 182 
},
{
 "AREA": "In front of Canada",
"TEMP": 23,
"NBCAR": 438 
},
{
 "AREA": "In front of Canada",
"TEMP": 23,
"NBCAR": 253 
},
{
 "AREA": "In front of Canada",
"TEMP": 23,
"NBCAR": 445 
},
{
 "AREA": "In front of Canada",
"TEMP": 23,
"NBCAR": 212 
},
{
 "AREA": "In front of Canada",
"TEMP": 23,
"NBCAR": 226 
},
{
 "AREA": "In front of Canada",
"TEMP": 23,
"NBCAR": 227 
},
{
 "AREA": "In front of Canada",
"TEMP": 23,
"NBCAR": 263 
},
{
 "AREA": "In front of Canada",
"TEMP": 23,
"NBCAR": 166 
} 
]
  
      if(!(opts.type==="pieChart" || opts.type==="sparklinePlus" || opts.type==="bulletChart")) {
        var data = d3.nest()
          .key(function(d){
            //return opts.group === undefined ? 'main' : d[opts.group]
            //instead of main would think a better default is opts.x
            return opts.group === undefined ? opts.y : d[opts.group];
          })
          .entries(data);
      }
      
      if (opts.disabled != undefined){
        data.map(function(d, i){
          d.disabled = opts.disabled[i]
        })
      }
      
      nv.addGraph(function() {
        var chart = nv.models[opts.type]()
          .width(opts.width)
          .height(opts.height)
          
        if (opts.type != "bulletChart"){
          chart
            .x(function(d) { return d[opts.x] })
            .y(function(d) { return d[opts.y] })
        }
          
         
        chart
  .reduceXTicks(false)
  .showControls(false)
          
        chart.xAxis
  .axisLabel("Temperature (Celsius degrees)")

        
        
        
      
       d3.select("#" + opts.id)
        .append('svg')
        .datum(data)
        .transition().duration(500)
        .call(chart);

       nv.utils.windowResize(chart.update);
       return chart;
      });
    };
</script>

<h3 align="center"> Have fun and let's progress! </h3>
