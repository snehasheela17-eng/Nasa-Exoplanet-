1. Dashboard Alignment — Power BI + Python
An interactive Power BI dashboard was created using the cleaned NASA Exoplanet dataset. The dashboard was
designed to visually represent important insights related to exoplanet discoveries, planetary mass, radius, and
detection methods.
Chart 1 — Average Planet Mass Over Time (Line Chart)
• Columns used: disc_year (X-axis), pl_bmasse (Y-axis — averaged)
• Shows how the average mass of discovered exoplanets changed from 1992 to 2026
• A filled area beneath the line adds depth and visual clarity
• Gold markers highlight each data point per year

Chart 2 — Planet Mass vs Planet Radius (Scatter Plot)
• Columns used: pl_rade (X-axis), pl_bmasse (Y-axis), discoverymethod (color/legend)
• Both axes use logarithmic scale to spread out the dense cluster of smaller planets
• Each discovery method is color-coded for easy comparison
• Reveals the mass-radius relationship across thousands of exoplanets

Chart 3 — Average Planet Mass by Discovery Method (Bar Chart)
• Columns used: discoverymethod (Y-axis), pl_bmasse (X-axis — averaged)
• Horizontal bar layout with log-scale X-axis to handle large mass differences
• The highest-average method bar is highlighted in gold
• Value labels displayed at end of each bar for direct readability

Chart 4 — Discovery Method Contribution (Donut Chart)
• Columns used: discoverymethod (legend/slices), pl_bmasse (count per method)
• Donut design with total planet count shown in the center (3,303 after cleaning)
• Percentage labels placed directly on each slice for methods above 2%
• Right-side legend shows method name with exact planet count

Interactive Filters (Slicers)
• hostname — filter by specific star system
• discoverymethod — filter by detection technique

• pl_bmasse — range slider to filter by planet mass
• disc_year — range slider to filter by discovery year

2. Summary of Findings
• The dataset contains 6,273 confirmed exoplanets discovered between 1992 and 2026, cleaned by
removing outliers and filling missing values.
• Transit is the most used discovery method, accounting for nearly 67% of all discoveries, mainly due to
the Kepler and TESS space telescopes.
• Transit finds smaller, lighter planets, while Imaging and Astrometry find fewer but much more massive
planets like gas giants.
• Exoplanet discoveries peaked around 2014–2016 during the Kepler mission, after which newer
instruments started finding smaller, Earth-like planets.
• A strong correlation exists between planet mass and radius — heavier planets are generally larger,
with some exceptions due to differences in density and composition.
• The average host star temperature is 5,390K, which is very close to our Sun (5,778K), suggesting most
discovered exoplanets orbit Sun-like stars.
• Despite thousands of discoveries, over 73% of all exoplanets were found by just one method
(Transit), revealing a strong observational bias in our current exoplanet catalog.
3. Key Insights — Trends, Anomalies, Correlations
1. Transit Method Dominates (66.9% of All Discoveries) The Transit method accounts for 4,196 out of 6,273
exoplanet discoveries, driven by the Kepler Space Telescope (2009–2018) and TESS (2018–present). The
dominance of one method introduces observational bias — our catalog over-represents smaller, close-in planets
that Transit can easily detect.

2. Discovery Rate Peaked 2014–2016, Now Finding Smaller Planets Early discoveries favored massive Hot
Jupiters as they were easiest to detect. As Kepler refined its data, it found thousands of smaller, lighter planets —
pulling the average mass down. Post-2018, TESS continues this trend by focusing on nearby, smaller planets.
3. Strong Mass-Radius Correlation with Outliers The scatter plot confirms heavier planets generally have
larger radii. However, outliers exist — some high-mass planets have small radii (dense iron-core planets) and
some low-mass planets have large radii (puffy gas worlds), revealing extreme planetary compositions.
4. Imaging Discovers the Most Massive Planets on Average Despite contributing less than 1% of total
discoveries, Imaging finds the most massive planets (often 1,000+ Earth masses). These are young, hot giant
planets far from their host stars — glowing brightly enough to be directly photographed.
5. Average Star Temperature is 5,390K — Similar to Our Sun Our Sun's temperature is about 5,778K, and the
dataset average is 5,390K — meaning most exoplanet host stars are Sun-like. This may reflect observational bias
toward Sun-like stars or suggest they are more likely to host detectable planets.
4. Recommendations for Decision-Making
• Space agencies should invest more in direct Imaging technology to discover massive planets that
Transit cannot detect.
• Diversifying detection methods beyond Transit will help reduce observational bias in the exoplanet
catalog.
• Future telescope missions like James Webb and Roman Space Telescope should focus on smaller,
Earth-like planets in habitable zones.
• Data from Radial Velocity and Astrometry methods should be expanded to find planets in wider orbital
ranges.
Machine learning models can be applied to predict discovery methods based on planetary features,
improving telescope targeting strategies.
5. The Final Story — What the Dashboard Reveals

1. The dashboard clearly explains the relationship between discovery methods, planetary mass,
radius, and discovery year.
2. The KPI cards provide an overall summary using total exoplanets, average star temperature, and
average planet radius.
3. The donut chart and bar chart show that the Transit method dominates exoplanet discovery and
finds lower mass planets on average.
4. The scatter plot helps identify planetary outliers and confirms the mass-radius relationship across
thousands of exoplanets.
5. The line chart shows how average planet mass changed over time, reflecting improvements in
telescope technology.
6. Overall, the dashboard provides meaningful insights that help understand exoplanet discovery
trends, planetary characteristics, and the effectiveness of different detection methods.
