# Amazon Vine Analysis
An analysis of Amazon Vine reviews for musical instruments and accessories using PySpark.

## Overview

Using data extracted from Amazon's review system, this analysis is to determine if there is any positivity bias for reviews in the Amazon Vine program, specific to musical instruments and accessories. Extracting the data using PySpark, we then perform a basic analysis of positive Vine(paid) reviews against positive unpaid reviews to determine any existing bias.

## Results

After filtering down the data to only reviews with >20 votes, where 50% or more of those votes labeled the review as "Helpful", here were the results of our analysis:

### Total Reviews

 - **Total Vine(paid) Reviews**
 
![image](https://user-images.githubusercontent.com/100869713/179423582-a92468fa-535f-404d-98cb-b7d01e554167.png)

 - **Total unpaid Reviews**
 
 ![image](https://user-images.githubusercontent.com/100869713/179423595-167040ce-724b-49a2-8f78-3109a0b01bfd.png)

### Total 5-star Reviews

 - **Total 5-star Vine(paid) Reviews**
 
 ![image](https://user-images.githubusercontent.com/100869713/179423610-c10f944c-b044-4b4c-aff5-bb3dd3806d83.png)

 - **Total 5-star unpaid Reviews**
 
 ![image](https://user-images.githubusercontent.com/100869713/179423621-59d9eb08-a9b3-4b14-ad90-a434c282ffa0.png)

### Percentage of 5-star Reviews

 - **Percentage of 5-star Vine(paid) Reviews**
 
 ![image](https://user-images.githubusercontent.com/100869713/179423643-1c5dd554-a94c-44d1-abcd-1e502a5beabf.png)

 - **Percentage of 5-star unpaid Reviews**
 
 ![image](https://user-images.githubusercontent.com/100869713/179423659-aad25f60-33b0-4359-8a26-8f75f559f4d2.png)
 
 ## Summary
 
 With paid 5-star reviews and unpaid 5-star reviews both rounding up to ~57%, there does not seem to be a positivity bias for Vine reviews in the Musical Instruments product category on Amazon.
 
 To further support this conclusion, we could also perform a comparison of the average review score of Vine reviews against the average review score of unpaid reviews. If these averages match, that supports that there is no bias in the paid reviewer category.
 
 ## Tools Used
 
  - `Google Colab`
  - `Python 3.9.7`
  - `Spark 3.0.3`
