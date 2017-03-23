# social_investment_analytical_layer
Standardised tables for doing cross agency work in the IDI

# Overview

The SIU has create a Social Investment Analytical Layer (SIAL): events-structured tables that arrange a version of the data held in Statistics New Zealand's IDI into a consistent format, making it easier and faster for authorised IDI users (researches and analysts) to use and understand.

The SIAL is designed to be reusable. It reformats most of the social sector tables available in the IDI into tables based on events (events-structured). For most tables available in the IDI there is a corresponding events structured table.

Expect warnings around the quoted string being processed has become more than 262 characters long. This is because the pricing table queries are read in as strings.
It does not have an impact on the pricing table.


# Installation
1. Download the zip file containing the sial scripts from github
2. Email access2microdata@stats.govt.nz and ask them to drop the files into your project
3. Unzip the files into your project
4. Paste the social_investment_analytical_layer-master folder into the top level of your project folder and rename it social_investment_analytical_layer
5. Open  main_sial.sas in SAS EG
6. Go to the main_sial.sas script at the top of the script there are two macro variables called targetschema and sial_code_path
7. Change the targetschema to the location you wish to write your files to e.g. the SIU schema is DL-MAA2016-15
8. Change the sial_code_path to the location where you stored the scripts on the network E.g. for the SIU our location is \\wprdfs08\MAA2016-15 Supporting the Social Investment Unit\social_investment_analytical_layer

Note that each time you run main_sial.sas it will uninstall all the SIAL tables you currently have before creating the SIAL tables

# Getting Help
More information will be coming

For now email info@siu.govt.nz


