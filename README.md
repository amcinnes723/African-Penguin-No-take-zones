# African-Penguin-no-take-zones
Marine habitat use by African penguins was assessed using telemetry data. Logger deployments were conducted between 2008 and 2022 at six colonies in South Africa: Dassen and Robben islands on the west coast, Stony Point and Dyer Island on the south coast, and St Croix and Bird islands on the east coast.To identify important marine habitat for African penguins, i.e. areas mostly available to penguins around each colony (foraging range) and areas of intense or preferred use around each colony (core foraging area), methods developed to identify marine Iimportant Bird Areas were used (Lascelles et al., 2016; Beal et al., 2021) using the R package track2KBA (Beal et al., 2021). 
Code to generate core foraging areas and foraging ranges is in Programme R with 2 files for each of 6 colonies - all have been zipped. Input files of tracking data will need to be requested from the BirdLife International Seabird Tracking database (see below for relevant links for each colony).
A trade-off mechanism following Punt et al. (2023) was used to assess the fishery no-take design that balaned the needs of both penguins and purse-seine fisheries. To construct trade-off curves we plotted benefit-cost points for all no-take zones (at a given colony), as well as points representing the industry-optimised scenario (fisheries cost = penguin benefit = 0) and the penguin-optimised scenario (fisheries cost = penguin benefit = 1). We then find the convex hull of all these points and construct the trade-off curve by fitting a monotone non-decreasing spline to the points on the boundary of the convex hull. The ‘balance point’ can then be found by numerically evaluating where the slope of the trade-off curve equals one, that is, where the rate of increase in penguin benefits equals the rate of increase in fisheries costs.
Input files and code (R) for the trade-off mechanism have been uploaded.

Seabird Tracking Database links to African Penguin breeding tracks

Dassen Island
https://data.seabirdtracking.org/index.php/dataset/2212
Robben Island
https://data.seabirdtracking.org/dataset/2213
Stony Point
https://data.seabirdtracking.org/index.php/dataset/2214
Dyer Island
https://data.seabirdtracking.org/index.php/dataset/2217
St Croix Island
https://data.seabirdtracking.org/index.php/dataset/2215
Bird Island
https://data.seabirdtracking.org/index.php/dataset/2216
