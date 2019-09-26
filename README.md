# Technical Task for a position of Machine Learning Engineer @ About You

Dear candidate

As part of the recruitment process, we would like to ask you to accomplish the following assessment task which should take not more than a couple of evenings of your time. Please do your best and aim for an end-to-end MVP solution.

As <em>result</em> of the exercise, it is expected to receive a link to the <em>github/gitlab/bitbucket repo</em> with working executable code base and instruction on how to run it, and with the detailed report (as <em>jupyter notebook</em>, or <em>markdown</em> file) containing description of your model, assumptions you made and justification of your tech choices.

## Description

We would like to propose you to familiarise yourself with the housing market in Hamburg, hence to suggest you to build a service to forecast price for the flats available for rent in Hamburg. 

In order to complete that exercise, we would like to formulate the following task for you:

1. Given the data sample <strong>ml_eng_ay_data.csv.gz</strong> (see [data dictionary](#data-dictionary) for columns description), build a model to forecast <strong>total rent price</strong> for <strong>up to 6 months</strong> in the future. The model should perform <em>better than</em> the seasonal naïve model in terms of RMSE. Use as many available <em>features</em> as <em>it would make sense</em> (based on the features importance) for the model accuracy and stability.
2. Deploy your <em>model as a service</em> (e.g. as a dockerized web server) so it is capable to run a batch-prediction.
3. (<em>Optional</em>) Build a dockerized stateless service to re-train your model.

### Data dictionary

|column|type|comment|
|:-|:-|:-|
|date|date|date when the ad was published|
|cnt_rooms|int|number of rooms in the flat|
|flat_area|float|living area of the flat (in square meters)|
|rent_base|float|base monthly rent for the flat (in euro)|
|rent_total|float|total (inlucing utilities) monthly rent for the flat (in euro)|
|flat_type|string|type of the property, e.g. appartment, roof_storey, etc.|
|flat_interior_quality|string|quily of the flat interior|
|flat_condition|string|flat condition, e.g. normal, good, etc.|
|flat_age|string|category of the flat's age (in years), e.g. <5, <10, ..., <50 etc.|
|flat_thermal_characteristic|float|energy consumption for the flat (in kWh per square meter per year)|
|has_elevator|boolean|indicates if the house has an elevator|
|has_balcony|boolean|indicates if the flat has a balcony|
|has_garden|boolean|indicates if a garden can be accessed from the flat|
|has_kitchen|boolean|indicates if the flat has built-in kitchen|
|has_guesttoilet|boolean|indicates if the flat has guest toilet|
|geo_city|string|city location of the flat|
|geo_city_part|string|city district location of the flat|

<br>

<em>Note</em>: we would recommend you to consider employing tools/services and languages we use:
- DSL/Programming language: <strong>Python (ver. >= 3.7.4)</strong>
- ML Frameworks/libraries: <strong>TensorFlow 2.0</strong>, <strong>GluonTS (ver. >= 0.3.4)</strong>
- <strong>Docker</strong> (ver. >= 19)

Good luck and hopefully see you soon in our headquarters for onsite interview.
<br>
<br>Best regards

<strong>ABOUT YOU GmbH</strong>
<br>Amtsgericht Hamburg HR B 120869
<br>Geschäftsführer: Sebastian Betz, Tarek Müller, Hannes Wiese