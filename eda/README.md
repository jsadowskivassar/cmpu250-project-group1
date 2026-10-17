# Exploring the Data:

**What is your outcome variable(s)?**

Our outcome variables are Average WAR per year played and FV (Future Value Rating). WAR is Fangraphs all in one player production metric and FV is Fangraphs way of grading prospects on the 20-80 scale.  

**How well does it measure the outcome you are interested in?**

These variables very effectively measure both a prospects projected production and actual production allowing us to dive into the traits that go into prospect evaluation. However of course, neither metric is perfect. There are tons of intangibles that can't be factored in to metrics like WAR that definitely impact player value. WAR also features positional adjustments which many people criticize. Intangibles by definition are immeasurable and there is a relatively even distribution of positions in our dataset so I don't think these two downfalls really impact WARs reliability for our purpose.  

**How does it relate to your expectations?**

We expect certain traits to be undervalued or overvalued by FV based on their correlation with WAR. These differences in value may reflect systemic bias in the prospect ranking process.

**What are your key explanatory variables?**

Some of our key explanatory variables are prospect background, age, hitting/pitching grade, and height and weight. All variables can be found in codebook.

# Data Cleaning:
**What data cleaning did you have to do?**

We had to trim the data to only include a prospects latest ranking, add the Average WAR, Background, Height and Weight Build, Had Tommy John, and Position group columns, and translate the FV, Height, Signing Bonus, and Grade columns to useable numeric values. 

**How did you prepare the data?**

We cleaned the columns we are using (in codebook) and got rid of the ones we are not  

**Are you deciding to exclude any observations? If so, why?**

Every player in the dataset has the majority of metrics. Depending on position and how low in the rankings the prospect was some don't have all (especially numeric metrics like Max exit velocity and hard hit%) but these are often the prospects that over perform their grades so they are still useful datapoints. As a result we didn't exclude any observations. 

**Did you have to create any new variables from existing variables? If so, how and why?**

The Average WAR, Background, Height and Weight Build, Had Tommy John, and Position group columns were all made from other columns. They provide a cleaner way to interpret the different traits and demographics in the dataset. More information on how we created these columns and what they mean can be found in the EDA codebook and notebook. 



