# SC1015-project
Lab Group: SC17
Muhammad Hisham Bin Khairul Annuar
Ong Li Han

 
# Data sources
Resale flats: https://data.gov.sg/dataset/resale-flat-prices
MRT stations: https://github.com/hxchua/datadoubleconfirm/blob/master/datasets/mrtsg.csv
Hospitals: https://www.healthhub.sg/directory/hospitals
Schools: https://data.gov.sg/dataset/school-directory-and-information
OneMap API: https://www.onemap.gov.sg/docs/

# Purpose
- Is the price of this flat listing reasonable? Ie. Can we predict the price of a flat accurately, which we can then use to decide whether a flat listing is reasonable?
- What should I look for if I want a cheaper flat? Ie. What characteristics of a flat affects its price?
- Does distance to nearby amenities really affect price?

# Methodology
1. Obtain 9000+ unique flat addresses from 120,000+ flat listings, by grouping on street_name and block #.
2. Obtain addresses of each amenity (MRT/hospital/school)
3. Use OneMap API to convert addresses to coordinates
4. Use Haversine Distance to convert pairs of coordinates to distances, then find out for each flat addresss, the closest amenity for each amenity type.
5. Associate each flat addresss with each unique flat listing
6. Analyse the data!


