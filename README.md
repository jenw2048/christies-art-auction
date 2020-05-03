# Post-War and Contemporary Art
## Goal
The goal of the notebooks is to show a fairly detailed exploration data analysis on artwork sold on Christie's, an auction house.

## Executive Summary
Ever wondered what drives the price of a painting? Contrast the following examples.

![High](https://i.imgur.com/2KM3P3I.png)
![Low](https://i.imgur.com/ahpMQ5U.png)

Two similar artwork but prices differ by approximately a 100 times. Can humans tell? Or can algorithms tell? Hence, this notebook aims to answer such questions.

## Dataset
The dataset covers auction results scraped from Christie's (https://www.christies.com/results/?did=74) and it dates from 8 February 2006 to 26 June 2019.

## Workflow
0. Scraped results using `BeautifulSoup` and `Selenium`.
1. Cleaned the dataset.
2. Checked for analomies.
3. Converted prices in foreign currency to USD based on historical monthly data provided by Bank for International Settlements (https://www.bis.org/statistics/xrusd.htm).
4. Extracted dimensions of painting, art media used, the age of the painting up to the point it is sold, etc. from descriptions using `spaCy`.

## Fun Facts
1. The most expensive paintings ever sold was *Salvador Mundi* by Leonardo da Vinci. This painting is also know as the male version of *Mona Lisa*. It was sold for 450 mil USD. (Source: https://www.christies.com/lotfinder/Lot/leonardo-da-vinci-1452-1519-salvator-mundi-6110563-details.aspx)
2. The most popular artist was Andy Warhol, who painted the famous *Campbell's Soup Can*.
3. New York hosted the most auctions, followed by London.
4. The year 2009 had the lowest sales record ever since 2006 while 2015 was the best year.
5. Oil is the most popular traditional paint medium.
6. Artwork executed between year 1890 to 1914 fetched the highest average realized price.
7. Amedeo Modigliani had the highest average realized price for his artworks. According to Wikipedia, he is best known for portraits and nudes in a modern style characterized by elongation of faces or necks.
8. The painting that has the biggest difference between its lower estimate and realized price was Andy Warhol's *Big Campbell's Soup Can with Can Opener*. (Source: https://www.christies.com/lotfinder/Lot/andy-warhol-1928-1987-big-campbells-soup-can-6076452-details.aspx)
9. The painting that has the biggest difference between its upper estimate and realized price was Mark Rothko's *Orange, Red, Yellow*. Its higher estimate was 45 mil USD but was realized at 86.9 mil USD. (Source: https://www.christies.com/lotfinder/Lot/mark-rothko-1903-1970-orange-red-yellow-5559196-details.aspx)
10. There were around 70 items that have appeared more than once on the auction market. An example was *Crio+Cristo+Critico*. It was first sold at 19,100 EUR in 2007 and resold for 12,800 EUR in 2008.

