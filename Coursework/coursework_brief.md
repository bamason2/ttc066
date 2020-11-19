
# TTC066 Vehicle Dynamics and Simulation

# MIRA Coursework

## Background

Development of models for the use of predicting powertrain performance is an important process in the design of a modern vehicle. Once a model has been developed it is also necessary to validate it against experimental data. Over the last few weeks you have developed a MATLAB Simulink vehicle/powertrain simulation model that can be used to estimate the straight-line performance of a passenger vehicle, this model will be used in the coursework. Empirical data will be collected from test track experiments at MIRA and this will be used to both tune and assess the validity of the model as well as illustrate factors affecting performance.

## Coursework assignment

The objective of the coursework assignment is to obtain real-world experience of straight-line vehicle performance characteristics and the use of a vehicle/powertrain simulation model to predict the vehicle motion under such conditions. This will involve;

* Measurement of empirical data from the vehicle CANBUS.
* Graphical examination and discussion of the measured data.
* Tuning of key simulation model parameters.
* Comparing the model predictions and measured data.

A report will be written and handed in at the end of Week 11.

## Test vehicle

The test vehicle is a Ford Focus ST.  Information about the speed of the vehicle is obtained from the vehicle's CANBUS. The driver's inputs,  of clutch and throttle pedal position are measured and these are used as inputs to the powertrain model. All variables are recorded on a laptop.

## Test procedure

The coastdown tests will be conducted on parallel straights. These consist of two dual carriageways, one mile long straights, linked with banked turns. The straight sections have zero gradients. Prior to testing the vehicle is weighed. The vehicle and tyres are warmed up by driving a couple of laps and the testing can then be started.

A typical test plan would be as follows. At least two pairs of coastdown data will normally be collected and used to cancel out the effect of wind.

* A speed of approximately 100kph is reached on the turn and the vehicle quickly accelerated up to approximately 115kph once on the straight.
* The gearbox is put into neutral and the vehicle coasts.
* Immediately after neutral is selected the data collection is started.
* At the end of the straight, the data collection is stopped and the test is then repeated in the opposite direction.

After completion of the coastdown tests, standing start acceleration tests are carried out. Two of these (one in each direction) can be used to try to achieve a minimum acceleration time.

## Model tuning

 ***Coastdown tests.*** These act as a precursor to the acceleration tests, allowing appropriate tuning of the drag parameters. You should compare simulated and measured vehicle speeds, and tune the $A_d$, $B_d$ and $C_d$ values to get the best match. It is also possible to change drivetrain friction parameters and vehicle frontal area (provided it remains physically realistic)

***Acceleration tests.*** You should aim to get the best correlation between vehicle/wheel speed in the simulation and measured wheel speed from the MIRA tests – also aim for good correlation between measured and simulated engine speeds. The most likely discrepancies between the results will probably relate to the tyre adhesion characteristics and clutch biting point. Adjust these parameters in the simulation model to match the measured data as accurately as possible. Other sources of error for example could be;

* Non-linearity of the clutch and/or throttle pedal inputs
* Engine torque scaling

These parameters can also be tuned to achieve a better match – but the tuned parameters must remain meaningful. Always try to understand and be prepared to explain the reason for changes.

## Preparation for test data

Before the test data becomes available, you should attempt a model tuning ‘dry run’. Tune the model parameters to obtain a single model that gives best performance on average for the calibrated test files provided for the lab exercise. Note that the actual MIRA tests results may vary significantly from the sample data and as such the tuned values will differ (i.e. you will need to tune the model to the actual measured data), the main purpose of the lab exercise is to gain familiarity with the software and parameter names.

Think about the report structure in advance so that number of graphs and information needed from the tests and analysis are known in advance. Parts of the report (such as the introduction) can be written in advance (and modified as necessary during MIRA week) to save time.

## Report

The report must be written in a formal, technical style. The first page should include an executive summary containing a maximum of 250 words. The maximum length of the report is 9 pages of A4, including the title page, all graphs (excluding appendices). Describe your results as concisely as possible – including plots of simulated and measured data on the same axes. Fully describe your measurements and examine/discuss the empirical data before moving on to the MATLAB analysis. Illustrate and discuss your findings for both the coastdown and acceleration sections of the test. Tabulate your tuned parameter settings and briefly discuss these settings in terms of feasibility and effect. Comment (but don’t dwell) on the major discrepancies between your tuned model and the vehicle results. In the further work section comment on additional instrumentation and tests that you would undertake to improve accuracy if you were to repeat the experiment and subsequent analysis.

Your report will be assessed in terms of:

* Your description of the vehicle testing. [20%]
* Your analysis and discussion of the measured data.  [20%]
* Your approach to, and comparative success in tuning the model parameters. [20%]
* Your discussions and commentary on the model/testing methods and errors noted. [20%]
* Clear and concise reporting style and general quality and completeness of the report. [20%]