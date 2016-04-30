## [GOT a Flight](http://www.delay.ml/) - [Live demo](http://www.delay.ml/demo/)
> ***Flight delay prediction system*** - **Clear for Take Off** Project - Nasa Space App 2016

### About GOT a Flight

The potential and complexity of the solution is that the prediction is not based on old statistics, but it is **based on the future and current forecasts** combined with **aviation reports** and multiple factors that influence the weather-related delays, such as the **position of the runways at the airport**, **the number of runways**, **the aircraft specifications**, the **conditions for emergency landings** at the departure airport and the International Aviation Standards and Regulations. 
This information is public; the key point is to combine the correct factors and to generate the most precise rules, and that is why GOT a Flight is being created!

In addition, GOT a Flight introduces the new concept of ***“insurance”*** in the aviation sector by offering flight insurance policies to **cover extra expenses** incurred due to the delay. As part of the project, we also present a roadmap with additional features aimed to improve the accuracy of the prediction.

### Proposed Solution

The complex work of predicting a flight delay was resolved by merging data from diverse sources: weather conditions, aircraft specs, airport design and International Standards and Regulations.
***The result is an application that predicts the probability of a flight being delayed because of the weather conditions***. Moreover, it offers the possibility to take out an insurance policy to cover the expenditures incurred due to the delay, thus proposing an innovative business model to the aviation market. 

### Prediction - How it works 

GOT a Flight predicts the weather conditions by analyzing parameters within different categories and by combining all the variables involved in a flight delay:

- **Aircraft specifications**: the range of acceptable crosswinds, the certification to operate in icy conditions operations and runway limitations are all parameters given by the manufacturer. 

- **International Aviation Standards and Regulations**: FAA and NOAA dispositions and Manual of All-Weather Operations, DOC 9365, from the International Civil Aviation Organization (ICAO).

- **Weather forecast and pre-flight reports**: The application combines long term forecasts taken from forcaset.io and aviation reports from the National Oceanic and Atmospheric Administration (NOAA) and the Aviation Weather Center (AWC), which are used by pilots to plan the flights. These aviation reports include **METAR**, **TAF**, **SIGMET** and **AIRMET**, and the variables are *temperature*, *wind speed and direction*, *humidity*, *precipitations*, *visibility* and *ceiling*.

- **The position of the runways in the airport and crosswind**: The orientation is needed to calculate the crosswind, the orthogonal component of the wind toward the runway. The maximum crosswind component is limited by the aircraft model and is given by the manufacturer. 

- **Visibility**: Even if the international and national standards and regulations allow take-off and landing with almost no visibility and ceilings as low as 200ft, the delays start as soon as the pilot needs to take off or land with *IFR*. What’s more, in the most crowded airports delays could start with MVFR procedures.

- **Icy conditions**: Most of the commercial aircraft are certificated to fly up to moderately icy conditions, but is highly recommendable to *avoid flying in severe icing conditions*. Even if the plane can take-off in such conditions, it is plausible that after a long taxing, the aircraft might be de-iced, resulting in delays.

- **Ceiling**: The *thickness and height of clouds* covering the sky, within the limits of the different flight categories: Visual Flight Rules (**VFR**), Marginal Visual Flight rules (**MVFR**), Instrument Flight Rules (**IFR**) and Low Instrument Flight Rules (**LIFR**).

- **The number of runways available in the airport**: If any of the runways cannot be used because of the weather conditions, then the same number of departures and arrivals has to be distributed between the remaining number of available runways. This situation will also generate a delay.

- **Departure and arriving airports**: The departure of an aircraft could be delayed by weather conditions at the departure airport, but it could also be delayed due to the bad conditions at the arriving airport.

- **Emergency landing at the departure airport**: For flight initiation, departure weather minima at an airport should not be less than the applicable minima for landing at that airport unless a suitable take-off alternate aerodrome is available.

### Improvements (coming soon...)

- **Implement Supervised machine learning techniques** to gain even more accuracy upon each delayed flight predicted. Currently the application is hosted in IBM Bluemix, so a potential candidate could be the Watson service.
- Add **more forecast sources and validate estimates**: detect if the weather prediction of a particular source is not reliable at a particular time.
- Include **historical statistics** and compare them with each prediction to test the results and adjust the estimate if found beneficial.
- Check and **analyze non-weather data** to cover more delay factors, apart from weather conditions.
- Load **more aircraft models and airports** with the corresponding specifications.
- Insert the **flight number instead** of the itinerary.

