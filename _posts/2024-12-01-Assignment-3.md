---
title: "Google Pixel 9 Pro XL Price Comparison Across Countries"
date: 2024-12-01
---
For our assignment, we picked the Google Pixel 9 Pro XL to compare the Canadian price to other countries.

**Section 1.1:** *Importing and defining functions.*
![image](https://github.com/user-attachments/assets/f173c6a8-78cc-432d-bb18-8e48c0caabe1)
![image](https://github.com/user-attachments/assets/fd5ab668-ab29-4185-9c9d-bba87e18f3e5)

We imported all the important libraries to webscrape, work with tables, and plot our graphs.  We also grabbed pre-made functions in order to help us clean data and do statistic analysis.

**Section 1.2:** *Choosing Countries.*
![image](https://github.com/user-attachments/assets/c417f8f9-a7f5-43e6-9d4b-3a4c0b703036)
We chose to work with 10 countries including Canada, so we put their names and relative currency code in an array to be able to use later.

**Section 2.1:** *Prices.*
![image](https://github.com/user-attachments/assets/8fea2f86-fe68-4943-b461-521f4910eedc)
We used this website to scrape a table that tells us the price of the Google Pixel 9 Pro XL in USD across various countries.  In this code, we also only take the countries that we are interested in using the array we defined before.

![image](https://github.com/user-attachments/assets/1884a3f8-88d4-40bf-8215-e1ff89cde2b2)
![image](https://github.com/user-attachments/assets/540ef966-47f0-4825-91b0-8cbb6d8e1569)

We cleaned the units from the original table and converted them into integers to be able to do calculations on.  We also then added and assigned the currency code of each country to the table to use for later.

**Section 2.2:** *Conversion Rates.*
![image](https://github.com/user-attachments/assets/e0953bd0-d400-41aa-85c9-c251061e4d52)
Created arrays and dictionaries to use for our conversion tables later.

*Section 2.2.1: USD to Local*
![image](https://github.com/user-attachments/assets/974eaef3-6a53-48cc-8259-958e4e1cbdf7)
![image](https://github.com/user-attachments/assets/62d2b3d5-dbeb-4e3b-b38f-703bd2dfd121)

Used webscraping on a website with live currency conversion rates to use to convert the original USD prices to local prices for each country.  We then identified the conversion rates we needed and put our pre-established arrays we made earlier in the table to categorize each conversion we needed for each of the currencies we needed to convert.

![image](https://github.com/user-attachments/assets/ab6efcd5-a9ba-47d8-96bf-d21ab2706029)
To make the local conversion rates more accessible to manipulate, we created a "for loop" to put them in a dictionary.

![image](https://github.com/user-attachments/assets/1f8ca202-f7ac-4811-b95d-0840a7d5afd2)
![image](https://github.com/user-attachments/assets/a8b649c3-9bf3-4a4b-b619-d9461209bb24)

We then used a "for loop" to convert each price in USD for each country into that country's local currency using the dictionary we created earlier. We put each of these values in a newly defined table.

*Section 2.2.2: Local to CAD*

![image](https://github.com/user-attachments/assets/46a64181-06af-4270-a6a5-4bb13a57be7e)
![image](https://github.com/user-attachments/assets/7f070730-321f-445d-ab86-e0c82ac78c20)

We now had to convert these local rates into CAD, so using the same website we used earlier we scraped the table of Canadian conversion rates and looked for the conversion rates of only the currencies we were interested in and put them in a new table.

![image](https://github.com/user-attachments/assets/44d5568f-f82d-48d0-a132-378d773bcf32)
Again, to make them more accessible we put these currencies in a dictionary.

![image](https://github.com/user-attachments/assets/c66452a1-aa05-454f-9dbf-576e4f906524)
![image](https://github.com/user-attachments/assets/30356d2b-1e4a-42a0-9aad-50d4d42b98f0)

Again, we used the same method to convert the local prices to CAD prices but this time, we added the CAD conversions instead of creating a new table.

*Section 2.2.3: Calculating the Difference*

![image](https://github.com/user-attachments/assets/196429f0-cae6-4a0f-8472-b2019a0c906b)
![image](https://github.com/user-attachments/assets/3317700d-3655-4f34-8abc-fc599f9d45ae)

We calculated the difference between the Canadian price of the phone with the converted CAD price of the phone of each country, and added them to the table.  We also removed Canada from this table since there's no logic in comparing Canada's price to itself.

**Section 2.3:** *GDP per Capita.*

![image](https://github.com/user-attachments/assets/1c87fe97-e189-4bf0-b51a-8f263bf1b097)
![image](https://github.com/user-attachments/assets/f0ceee5a-7646-48e6-b3b2-4d460f7d97e3)

For our external factor, we decided on country GDP per capita since in a general sense, poorer countries tend to have cheaper goods than richer countries.  We webscraped a website with countries GDP per capita and only took the countries we were interested in.

***Section 3:*** *Tables.*

![image](https://github.com/user-attachments/assets/f7c151e0-2550-42c5-b39f-a0785542d9d5)

We joined the table with GDP and the price differences in CAD for each country and dropped the unnecessary data in order to graph it more simply.  We also then sorted the GDP from largest to smallest to see if we could visually see a pattern in the data.

![image](https://github.com/user-attachments/assets/c4402182-324e-479b-b447-42f9115bf99a)

Code to create the bar graph showcasing each country's GDP per capita.

![image](https://github.com/user-attachments/assets/5ebca870-37ee-4e45-9f5f-d94e519ff603)
We see Australia has the largest GDP per capita while Poland has the smallest.

![image](https://github.com/user-attachments/assets/efaab24f-0c94-4124-b726-8e122d30facb)

Code to create the bar graph showcasing the price difference in CAD of the Google Pixel 9 Pro XL compared to the Canadian price
![image](https://github.com/user-attachments/assets/782ebc37-7fba-4417-b074-e545895eadf3)

This graph is still sorted from largest to smallest GDP per capita.  At first glance, there doesn't seem to be any discernable pattern, but we could maybe make out a slight negative correlation.

![image](https://github.com/user-attachments/assets/12cb4d66-ef26-4ac9-aa24-3f4bb2b44616)

The Code in order to create a scatterplot between the price difference and the GDP per capita for each country minus Canada.  This code also prints out the statistical correlation between the two using a pre-defined function we established earlier.
![image](https://github.com/user-attachments/assets/8b8cd406-4e68-4091-ab74-574baea3d711)

Without the fitline, we could barely see a pattern in the data, but the fitline tells us that theres a slight negative correlation.  To corroborate this, our function tells us that the correlation is -0.24.  This is a small negative correlation which doesn't necessarily mean that these two variables actually have a pure negative correlation, even if its a small one.  We also have to keep in mind this correlation can change as our data for currency conversion is live.  This means our hypothesis was wrong, and that it was not a positive correlation.  However, we only have 10 countries to base this conclusion and they are all Western countries, which could influence the data.

Using this data, we see that Canada has the cheapest Google Pixel 9 Pro XL and that the UK has the most expensive one, with Poland coming second.  This means we luckily have the best deal for the latest Google Pixel phone right here at home!
