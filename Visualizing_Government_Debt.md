#**Visualizing Government Debt**


<iframe src="https://data.oecd.org/chart/6O87" width="860" height="645" style="border: 0" mozallowfullscreen="true" webkitallowfullscreen="true" allowfullscreen="true"><a href="https://data.oecd.org/chart/6O87" target="_blank">OECD Chart: General government debt, Total, % of GDP, Annual, 2019</a></iframe>

<br/>

<div class="flourish-embed flourish-chart" data-src="visualisation/11132696"><script src="https://public.flourish.studio/resources/embed.js"></script></div>

<br/>


<div class="flourish-embed flourish-scatter" data-src="visualisation/11140377"><script src="https://public.flourish.studio/resources/embed.js"></script></div>

<br/>

### Discussion:

The three visualizations above are sourced the same data ([OECD General Government Debt Data](https://data.oecd.org/gga/general-government-debt.htm)) but convey information in different ways — and, perhaps, to different audiences. The bar chart focuses on a single year of data (2019) and compares all countries, ranking them along the x-axis from lowest to highest ratios. This allows viewers to easily compare countries across 2019, and the interactive pop-up labels for the bars make it easy to identify countries. The second graph, a sparkline facet graph, visualizes the data across time (from 1995-2019), breaking each country out into its own chart. Now, the viewer can spot trends across years in a single country, whereas the prior graph leveraged a static timeframe. However, cross-country comparisons are more difficult: comparing, for example, Greece to Germany forces the viewer to visually inspect two charts, hold information of interest from each, and then compare. The first chart serves better if we expect viewers to quickly glaze over it, whereas the second asks the viewer to take more time in digesting all it has to offer.  

The third visualization is a line chart that focuses on European countries' debt-to-GDP ratios from 1995 to 2019. I wanted to create a graph that contextualized the data geographically, but there were far too many countries to derive a trend at the national level. Further, most of the countries in the data set are European, meaning that broad continental regional analysis was largely drowned out by a web of lines from European countries. I decided to code the data into European regions to highlight an interesting trend in the data: southern European countries, in general, have the highest ratios across this timeframe. Leveraging a colorblind-friendly palette, I chose a bold warm-toned hue (magenta) for southern European countries to visually reinforce the fact that their ratios were the highest (and that high ratios are not desirable). I colored western Europe grey because that region's data had a wide range of ratios, which, if imbued with a non-grey hue, fought against southern Europe's magenta and distracted from the message I wanted to highlight from the data. 

Compared to the prior two graphs, the third offers a narrower, although perhaps richer, lens on the data. It no longer displays all countries, meaning that the viewer loses hold of the fact that Japan's debt-to-GDP ratio is very high. Yet it thematizes the data into geographic regions and the title forefronts the fact that southern European countries tend to have high ratios in comparison to other European countries. Similar to the second chart, viewers can see the data over time, but they no longer have to visually toggle between distinct charts. This compactness allows the viewer to grasp the information in a shorter amount of time, as compared to the second chart.

<br/>

Finished? Return to the [homepage of the repository.](README.md)
