HD3 Transfers
================

### Analyzing Patient Transfers in the Atlanta HD3 Area

In my work as a data analyst with a government agency, I was given a dataset of digitized case reports of people who came in to private practice doctors, public hospitals, and nursing facilities. Some of these cases tested positive for a certain antibiotic-resistant infection (ARI). By tracking where these people went (transfers between hospitals), I generated a network map of where the ARI went. Here's a de-identified (unlabeled) version of that map:

![Antibiotic-Resistant Transfers](Visuals/ARI%20Network.gif) [PDF Version](Visuals/ARI%20Network.pdf)

[Check out the code in `ari-transfers.R`](ari-transfers.R)

I also have a dataset of all of the patient transfers in the state of Georgia, regardless of whether or not they tested positive for the ARI. If we consider the ARI data to be the "numerator" data, this is the baseline "denominator" data. If we can find a significant correlation between these maps, then we can use general patient transfer data in order to model the spread of the ARI we care about. Here's what that overlay looks like:

![ARI Overlaid on Denominator Data](Visuals/Denominator%20Network%20(ARI%20Overlay).png) [PDF Version](Visuals/Denominator%20Network%20(ARI%20Overlay).pdf)

[Check out the code in `all-transfers.R`](all-transfers.R)
