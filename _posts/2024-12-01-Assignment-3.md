---
title: "Google Pixel 9 Pro XL Price Comparion Across Countries"
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
