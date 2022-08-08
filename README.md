# Investigative Genetic Genealogy Map
Author: Ole Westh  
Date: 07-08-2022  

## Step 1: Purpose = Visualizing development across the world
My interest to create this map came from a citizen proposal to change the Danish legislation in order to use Investigative Genetic Genealogy (IGG).

**Citizen proposal: Danish Police must be able to use genetic genealogy in the investigation of murder and serious crime dangerous to persons**
Source: [Borgerforslag: Dansk Politi skal kunne bruge genetisk slægtsforskning i efterforskning af drab og grov personfarlig kriminalitet](https://www.borgerforslag.dk/se-og-stoet-forslag/?Id=FT-11761) (Located 07-08-2022)

### Golden State Killer
Furthermore IGG was used to locate the Golden State Killer, which Science Magazine recognized as on of the breakthrough scientific methods in 2018:
* "*In April, police announced they had arrested a suspect in one of the coldest of cold cases: a series of rapes and murders in California in the 1970s and 1980s. It was a stunning development, and so was the way investigators fingered the alleged Golden State Killer. They identified his relatives by uploading a profile of DNA recovered from one of the crime scenes to a public genealogy DNA database.*"

### Questions
This made me wonder about the following:
1. Which countries have implemented investigative genetic genealogy? And when?
2. Which countries have conducted pilot studies? And when?


## Step 2: Prepare data sources
First I needed a table with country all country names. From [kaggle.com](https://www.kaggle.com) I found a dataset named [*Countries of the World*](https://www.kaggle.com/datasets/fernandol/countries-of-the-world). Downloaded in csv-format.

## Step 3: Process 
I uploaded the csv file from Kaggle to Google Sheets, where I added the following columns:

- Investigative genetic genealogy (Options: Yes, Pilot study, No)
- Year of first use
- Note: Quote from source
- Source: Link


Exported the new table with the added columns in csv.

## Step 4: Creating the map in Tableau
I choose the public version of Tableau to easily create a shareable interactive map.

### Color palette
First of I used built in colors that were changed to trafic light:  
- Green = Have implemented the technique ```Hex: 309143```
- Yellow = Pilot study ```Hex: ffda66```
- Red = Have not implemented

As not to indicate red being a 'bad' choice I changed that to grey  
```Hex: c8d0d9```

Personal opinion: Implementing new investigative techniques tends to end up broadly being perceived as a choice between giving away individual freedom to the state versus easing the opportinities to catch more criminals. 

In other words: "*Proportionality is a key concept in forensics when attempting to balance the privacy rights of the individual versus the need for public safety*" (D. Kling et al., 2021).

Therefore I see grey as a more neutral color choice compared to red. 

### Country label: Year of first use
To quickly see the year the technique was first used - without having to hover the cursor over the specific country - I choose putting the year of first use on the map.  
At first I called this the 'Year of implementation', but that could be misleading as the legal basis for in the countries is not necessarily the same.

![ Tableau map example](/color_palette.png "Color palette example")
As seen above only Canada have a year of implementation added. I could see that having this label would require me to go back and update the columns of all countries with the technique implemented.

### Source of information for further reading
Adding a link to the source serves to purposes:
1. Validity of the map information
2. Providing an opportunity for the curious reader to *investigate* further in the sources material.

The end result of hovering over each country would look something similar to this:
![Hovering over each country leading to source link](/hovering_source_link.png "hovering source link") 

## Step 5: Analysis
From inspecting the map the current answers to the questions are.

1. Which countries have implemented investigative genetic genealogy? And when?
   * [United States of America in 2018](https://vis.sciencemag.org/breakthrough2018/finalists/#forensic-genealogy) and [Canada in 2019](https://isogg.org/wiki/Investigative_genetic_genealogy_FAQs#Which_countries_are_using_investigative_genetic_genealogy.3F).

2. Which countries have conducted pilot studies? And when?
   * [The Netherlands in 2018](https://www.forensicinstitute.nl/news/news/2018/01/29/netherlands%E2%80%99-largest-ever-familial-dna-investigation), [Sweden from 2019 to 2020](https://polisen.se/siteassets/dokument/forensik/forensic-dna-traces-and-genealogy.pdf/download?v=e31330453befc3ad03b222eb546c79b2) and [Australia in 2021](https://www.monash.edu/medicine/news/latest/2021-articles/forensic-scientists-identify-long-term-jane-and-john-does-in-australian-first).


## Step 6: Sharing results
1. Sharing the actual visaulization in Tableau
2. Creating a LinkedIn post to share the Tableau visualization


## Bibliography
- [D. Kling et al. (January 30, 2021). *Investigative genetic genealogy: Current methods, knowledge and practice*](https://doi.org/10.1016/j.fsigen.2021.102474)


- [isogg.org (2020). *Which countries are using investigative genetic genealogy?*
](https://isogg.org/wiki/Investigative_genetic_genealogy_FAQs#Which_countries_are_using_investigative_genetic_genealogy.3F)

- [A. Tilmar et al. (July 2021). *Getting the conclusive lead with investigative genetic genealogy – A successful case study of a 16 year old double murder in Sweden*](https://www.sciencedirect.com/science/article/pii/S1872497321000636)
  * "*On the morning of October 19, 2004, an eight-year-old boy and a 56-year-old woman were stabbed to death on an open street in the city of Linköping, Sweden. The perpetrator left his DNA at the crime scene, and after 15 years of various investigation efforts, including more than 9000 interrogations and mass DNA screening of more than 6000 men, there were still no clues about the identity of the unknown murderer.*"
  * "*The genealogy work resulted in two candidates, one matching crime scene samples.*"

- [The Swedish Police Authority, National Forensic Centre (November 2021). *Forensic DNA traces and genealogy: Use of investigative genetic genealogy in criminal investigations*](https://polisen.se/siteassets/dokument/forensik/forensic-dna-traces-and-genealogy.pdf/download?v=e31330453befc3ad03b222eb546c79b2) (44 pages report)
  * *"In this report a new and most powerful tool for Swedish criminal investigations and forensic science is presented. With the support of legal inquiries a pilot case study has been successfully completed and with the use of the tool Investigative Genetic Genealogy a serious crime has been solved. (…)  
  Herein, an overview of investigative genetic genealogy is presented. In addition, the case study is described in some detail as well as experiences gained and conclusions drawn."* 
  
- [Borgerforslag FT-11761 (2022). *Dansk Politi skal kunne bruge genetisk slægtsforskning i efterforskning af drab og grov personfarlig kriminalitet*](https://www.borgerforslag.dk/se-og-stoet-forslag/?Id=FT-11761)
  * Danish citizen proposal 2022: *Danish Police must be able to use genetic genealogy in the investigation of murder and serious crime dangerous to persons*  

- [Jill Sederstrom (July 1, 2020). *‘We Got The Right Ending’: Genetic Genealogist Who Helped Put Golden State Killer Away Reflects On His Guilty Plea*](https://www.oxygen.com/crime-news/barbara-rae-vente-reacts-to-golden-state-killer-joseph-deangelos-guilty-plea)  
    * "*Barbara Rae Venter used crime scene DNA to determine the most likely suspect in a series of murders and rapes that had baffled investigators for decades, pointing authorities in the direction of Joseph DeAngelo.*"
