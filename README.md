# Springboard Capstone 1

## Introduction and motivation

AirBnb is a website that allows people to search and reserve short-term and apartment rentals, as well as become a host on the platform by opening up their own space to potential guests. All prices are set by the hosts, and guests/renters can narrow their search by different criteria to find a place to stay within their budget while still meeting their needs. As a host looking to earn supplemental income through AirBnB, it is important to know what the market price for your space is so that you can meet the demand of more consumers and ultimately have more guests book a stay with you.

There are third-party companies out there who provide AirBnB pricing for a fee, but you still aren't told what you should price it at in order to get the most demand. AirBnB also provides hosts with some advice when it comes to pricing, but who knows what attributes they are using to determine those prices, or how successful that value is in attracting guests (as hosts don’t have to go with the suggested price, this would be hard to test!). Within the real estate industry, this would have a big impact for real estate agents and their clients (homebuyers and investors) looking to use a measure like this as part of the bigger picture in describing and analyzing the potential return on investment for a home purchase.

With this project, I hope to create a model that takes in AirBnB listing data and predicts the base price for listings in Los Angeles, CA. I hope to expand this project to other cities and also to use NLP techniques on the text attributes to see if it improves accuracy.

## Conclusions
This model could contribute to the AirBnB host platform by providing more insight into the market and how much a host can expect to make by listing their space. This analysis also provides insight into which features of a listing are most important, and what a host can do to earn more for their listing.
Through modeling the data using a RandomForestRegressor, we know that we can predict what the nightly price of an AirBnB listing in LA should be with 80.87% R^2 accuracy, according to other listings and their features. We see from the feature weights that over 70% of the model is based on the ‘accommodates’, ‘bathrooms’, ‘room_type’ and ‘latitude’/‘longitude’ attributes, which are all fixed numbers a host can easily come up with when going to look up whether or not to AirBnB their space. Because the ‘accommodates’ feature is so important in determining price, and we saw earlier that the list price increased as the number of guests accommodated increased, we could also recommend that hosts optimize their space to accommodate as many guests (comfortably) as possible to optimize revenue. 

I was also interested to see how many predictions fell within 5% of the actual price, within 10%, and above 15%. 
Total # test data: 7770
Within 5% error: 4595
Within 10% error: 6663
More than 15% error: 414

This shows us that only about 5% of the predictions came in with more than 15% error.

