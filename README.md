# spok-dataset

## About

spok-dataset is a dataset created to help correlate numbers belonging to Spok with their respective geographical regions.

This dataset was created in the week of May 2, 2022 - May 8, 2022 by checking 23.36 million numbers against Spok's validation CGI. It is meant to accompany an article I've published on [HackerNoon](https://hackernoon.com/americas-secret-pager-giant).

I will not update this dataset going forward, and I don't encourage you to either. Spok's servers have already endured enough.

## File Contents
- `areadecipher.txt` - Scraped ZIP code data from area-codes.com, correlating central office code with ZIP.

Pro-tip: at the time of writing, the XPath used was:<br>```/html/body/table/tbody/tr/td/table[2]/tbody/tr/td[2]/table[1]/tbody/tr[7]/td[2]/a```

- `areas.csv` - Amount of validated Spok numbers in a given ZIP code. ZIP correlation via Simplemaps.

- `cities.csv` - Amount of validated Spok numbers in a given city. City correlation via Simplemaps.

- `count.csv` - Amount of validated Spok numbers in a given central office code, with that NXX's rate center being listed as well. NXX info from NANPA.

- `counties.csv` - Amount of validated Spok numbers in a given FIPS county. FIPS correlation via Simplemaps.

- `spokareas.txt` - NAA/NXX codes assigned to Spok as of 4/27/22. Info from NANPA.

- `states.csv` - Amount of validates Spok numbers in a given state. NXX info from NANPA.

## Credit/Thanks

- Blair "r000t" Strater - For writing the base scraper code. You're a real king.
- NANPA - [Central Office Code Assignment Records](https://nationalnanpa.com/reports/reports_cocodes_assign.html)
- Simplemaps - [US Zip Codes Database](https://simplemaps.com/data/us-zips)
- area-codes.com - For having an easily scrapable page :P
