<h2 style="color:#6f1802;">Portfolio</h2>
***
<h3 style="margin-bottom:0;">Vaux’s Swift Migration Along the Pacific Flyway (GBIF, 2023)</h3>
<p style="margin-top:2px; font-size:0.9em; font-weight:normal; color:#777;">
  28 October 2025
</p>
<p>
Using GBIF occurrence records from 2023 joined to EPA ecoregions, I mapped Vaux’s swift (Chaetura vauxi) observations by month and normalized counts for sampling effort. The dataset shows northbound movements in April–May and southbound passage in August–September, with concentrations along the Pacific coast and lower Cascade ecoregions—consistent with known migration routes.</p>

<p><img src="img/Vauxs-Swifts-Chapman-IMG_6065-SC-768x886.jpg" alt="Vauxs Swifts" title="Vaux's Swifts enter the Chapman Elementary School Chimney, Portland, OR, photo by Scott Carpenter" style="float:right; width:200px; height:auto; margin:0 0 6px 12px; border-radius:4px;">Vaux’s swifts are remarkable aerialists, spending nearly their entire lives in flight. They feed, drink, court, and collect nesting material in flight. Each fall, thousands gather at roosts such as Portland’s Chapman Elementary chimney, the largest known aggregation in the world, before continuing south to Central America and Venezuela.</p>

Historically, the species nested in hollow old-growth snags, but many now use chimneys as substitutes. Once a suitable site is found, swifts often return year after year, clinging vertically to rest before resuming flight at dusk.

<iframe
  src="img/vaux_migration.html"
  style="width:900px; height:900px; border:0; transform:scale(0.6667); transform-origin:top left; display:block;"
  title="Vaux's Swift Migration Map">
</iframe>

  <figcaption style="font-size:0.9em; color:#555; margin-top:6px;">
    <b>Figure 1</b>. Monthly observations of Vaux's Swifts by ecoregion, effort-normalized. Use the slider to compare northbound and southbound migration periods.
  </figcaption>

<br/><b>Data & methods</b><br/>
GBIF occurrence data (tab-delimited CSV), EPA ecoregions, GeoPandas spatial join, monthly/ecoregion group-by, effort normalization, and hvPlot/Panel for visualization. Duplicate records and repeated checklist submissions were filtered to unique eventIDs per month and ecoregion to minimize oversampling at known roost locations.

<b>References</b><br/>
GBIF.org (28 October 2025) GBIF Occurrence Download https://doi.org/10.15468/dl.5x7k7q<br/>
Bird Alliance of Oregon. (n.d.). Vaux’s Swifts. Retrieved October 28, 2025, from https://birdallianceoregon.org/our-work/rehabilitate-wildlife/having-a-wildlife-problem/vauxs-swifts/<br/>
GBIF Secretariat. (n.d.). Chaetura vauxi (J.K. Townsend, 1839). Retrieved October 28, 2025, from https://www.gbif.org/species/5228612

***
<h3 style="margin-bottom:0;">Veery Migration Across North America (GBIF, 2023)</h3>
<p style="margin-top:2px; font-size:0.9em; font-weight:normal; color:#777;">
  26 October 2025
</p>
<p><img src="img/Veery_in_CP_(43277).jpg" alt="Veery" title="Veery in Central Park by the Ramble Stone Arch. Source: Wikimedia" style="float:right; width:200px; height:auto; margin:0 0 6px 12px; border-radius:4px;">
Using GBIF observations joined to EPA ecoregions, I mapped Veery (Catharus fuscescens) records by month and normalized counts for sampling effort. Two clear pulses show up: a spring push in May–June into the northern hardwoods and Great Lakes ecoregions, and a broader fall movement in August–October as birds head to South America. Normalizing by month and ecoregion helps reveal the underlying pattern despite uneven observer effort.</p>

Veery is primarily an eastern species. In the Pacific Northwest, and Portland specifically, it’s scarce and irregular. Local checklists show only occasional migrants, usually in riparian or forest patches during fall. In other words: Portland sits well outside the species’ core flyway, so most of the signal comes from the Upper Midwest and Northeast.

<iframe
  src="img/migration.html"
  style="width:900px; height:900px; border:0; transform:scale(0.6667); transform-origin:top left; display:block;"
  title="Veery Migration Map">
</iframe>

  <figcaption style="font-size:0.9em; color:#555; margin-top:6px;">
    <b>Figure 1</b>. Veery observations by ecoregion, filtered by month. Use the bottom slider to step through the calendar and compare spring vs. fall patterns.
  </figcaption>

<br/><b>Data & methods</b><br/>
GBIF occurrence data (tab-delimited CSV), EPA ecoregions, GeoPandas spatial join, monthly/ecoregion group-by, effort-normalized counts, and hvPlot/Panel for the interactive map.

***
<h3 style="margin-bottom:0;">50 Years of Warming in Portland, OR (1959-2009)</h3>
<p style="margin-top:2px; font-size:0.9em; font-weight:normal; color:#777;">
  29 September 2025
</p>
Over 50 years, Portland, Oregon has warmed at an average rate of 0.016 °C per year (about 0.16 °C per decade), based on NOAA’s Global Historical Climatology Network Daily (GHCND) dataset (NOAA NCEI, 2024a). This rate is slightly lower than the global average warming calculated by NOAA for 1982–2023 (0.20 °C per decade) (NOAA NCEI, 2024b), but it still represents a clear long-term warming signal. The R² value of 0.088 shows that much of the year-to-year variation comes from natural climate variability, yet the overall slope remains positive.

<figure style="text-align:center;">
  <img src="img/Portland_climate.png" alt="Portland Climate Plot" style="max-width:100%; height:auto;">
  <figcaption style="font-size:0.9em; color:#555; margin-top:6px;">
    <b>Figure 1</b>. Annual average temperature in Portland, OR 
    (NOAA GHCND Station USC00358634, 1959–2009) with linear regression 
    trend line and 95% confidence interval.
  </figcaption>
</figure>

Portland’s proximity to the Pacific Ocean means its climate is strongly influenced by large-scale patterns such as the Pacific Decadal Oscillation (PDO) (NOAA PSL, 2024) and the El Niño–Southern Oscillation (ENSO) (NOAA Climate.gov, 2024). These oscillations can mask or amplify the underlying warming trend. For example, the late 1970s and early 1980s show a stretch of cooler years that align with a cool phase of the PDO, while the 1990s and the 2010s contain clusters of notably warm years, some coinciding with strong El Niño events. These alternating cool and warm stretches illustrate the “noise” of natural variability on top of the long-term trend.

Background research on regional climate (ClimateStations, 2024) describes Portland’s climate as mild, with wet winters and dry summers, moderated by maritime influences. That Portland shows a persistent warming trend despite this moderation underscores the broader signal of climate change in the Pacific Northwest.

<a href="https://tkbravo.github.io/img/09_Portfolio_Climate_Portland.html" target="_blank">View the full climate analysis</a>

<b>References</b>
<div style="margin-top:4px; font-size:0.9em; color:#555; line-height:1.5;">
  ClimateStations. (2024). Portland, OR Climate Information. Retrieved from 
  <a href="https://www.climatestations.com/portland-or/" target="_blank">https://www.climatestations.com/portland-or/</a><br>
  
  NOAA Climate.gov. (2024). El Niño–Southern Oscillation (ENSO) Overview. Retrieved from 
  <a href="https://www.climate.gov/enso" target="_blank">https://www.climate.gov/enso</a><br>
  
  NOAA NCEI. (2024a). Global Historical Climatology Network Daily (GHCND): Troutdale, OR (USC00358634). Retrieved from 
  <a href="https://www.ncdc.noaa.gov/cdo-web/datasets/GHCND/stations/GHCND:USC00358634/detail" target="_blank">https://www.ncdc.noaa.gov/cdo-web/datasets/GHCND/stations/GHCND:USC00358634/detail</a><br>
  
  NOAA NCEI. (2024b). Climate at a Glance: Global Time Series. Retrieved from 
  <a href="https://www.ncei.noaa.gov/access/monitoring/climate-at-a-glance/" target="_blank">https://www.ncei.noaa.gov/access/monitoring/climate-at-a-glance/</a><br>
  
  NOAA PSL. (2024). Pacific Decadal Oscillation (PDO) Index. Retrieved from 
  <a href="https://www.ncei.noaa.gov/access/monitoring/pdo/" target="_blank">https://www.ncei.noaa.gov/access/monitoring/pdo/</a>
</div><br/>

***

<h3 style="margin-bottom:0;">Map from OpenStreetMap</h3>
<p style="margin-top:2px; font-size:0.9em; font-weight:normal; color:#777;">
  8 September 2025
</p>
This interactive map in Python highlights the central campus of Indiana University in Bloomington, Indiana. The flagship campus of the IU system, it is a major public research institution, and the map shows its academic buildings, administrative areas, and green spaces.
<embed type="text/html" src="img/start.html" width="600" height="600">
