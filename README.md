# Car-Price-Prediction
Problem Statement –
----------------
An AutoMobile Company has collected data for 2018 years sales but unfortunate due to power failure their server crashed and the data they collected got corrupted. In some features values became missing and for some car sale entries price features, details are lost. Now this company needs your help and has hired you to predict their missing entering and find the lost car prices value.
They have also asked you to tell the car price-category [Low, Medium, High].

Data Description –
--------------------
Each Car (has an id number) has feature inputs of fuel type in car(petrol/diesel), ABS-compatibility, support of parking sensors(parking-sensor), its assigned insurance risk rating (symbolling), average loss payment per insured vehicle(normalized loss), number of doors in car, body-type(sedan/hatchback/wagon/etc.), manufacturer brand name(manufacturer), condition of car(condition: new/old), wheel-base details, length, breadth, height, car-weight in pounds, engine-type, number of persons capacity in car, engine-size, battery-type, diameter of each cylinder (bore), amount of movement of piston can move up & down(stroke), compression-ratio, horsepower in hp, peak-rpm, mileage within the city(city-mpg) and highway(highway-mpg) and price.

The lost corrupted values are marked with a ‘?’.

File Descriptions –
-----------------------
·        train.csv – the training dataset

·        test.csv – the testing dataset

·        sample.csv – a sample submission file in the correct format

Data Fields –
-----------------
·       id: car_id (unique for every entry)

·       fuel: car fuel-type (petrol or diesel)

·       ABS-compatibility: support or not

·       parking-sensor: tells about compatibility

·       symboling: its assigned insurance risk rating

·       normalized-losses: average loss payment per insured vehicle year

·       num-of-doors: two or fours doors car

·       body-style: car body style (hatchback/sedan/wagon/etc.)

·       manufacturer: car brand name

·       condition: car sold was new or old

·       wheel-base: distance between centers of front and rear wheels

·       length: length of car [continuous from 141.1 to 208.1]

·       width: width of car  [continuous from 60.3 to 72.3]

·       height: height of car [continuous from 47.8 to 59.8]

·       car-weight: weight of car without occupants or baggage(in pounds)

·       engine-type: [dohc, dohcv, l, ohc, ohcf, ohcv, rotor]

·       num-of-persons: [eight, five, four, six, three, twelve, two]

·       engine-size: [continuous from 61 to 326]

·       batter-type: [sli, li-ion, wetcell, dc, vrla, ssli, msli, agm]

·       bore: diameter of car cylinder

·       stroke: amount of movement of piston can move up & down

·       compression-ratio: [continuous from 7 to 23]

·       horsepower: value in hp [continuous from 48 to 288]

·       peak-rpm: power band of electric motor

·       city-mpg: city mileage of car

·       highway-mpg: highway mileage of car

·       price: price of car



SOLUTION APPROACH
-------------------
I have used KNN- Imputation to impute the missing value.
Used only those attribute which is highly influence the price attribute (having high corelation value with price)
Applied Logistic regression to predict the prixe.

RUN the code
------------
First run train.ipynb file.
Model generated after training is finalized_model.sav
Then run Test.py which save the predicted price in file output file.
























