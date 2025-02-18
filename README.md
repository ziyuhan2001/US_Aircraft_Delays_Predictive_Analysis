# Predicting Arrival and Departure Delays for U.S. Domestic Flights through Regression Modeling

Regardless of domestic or international flights, the reduction of flight departure and arrival delays is crucial for maintaining passenger satisfaction and ensuring optimal inbound and outbound flight coordination and aircraft scheduling for airlines. As such, this project analyzes the combined dataset of 2022 US domestic flight data from the Bureau of Transportation Statistics and daily airport weather data from the National Centers for Environmental Information. Utilizing the R programming language, we develop predictive regression models to forecast aircraft delay times in the United States and identify future trends. This involves conducting Exploratory Data Analysis to gain insights and employing regression methods for effective model selection, aiming to optimize predictions of future delay times. The results indicate satisfactory predictive accuracy, with PLS emerging as the most effective model.

## INTRODUCTION

Ensuring optimal passenger satisfaction and maintaining efficient aircraft coordination are paramount objectives in the airline industry. Our project, with a central focus on in-depth analysis of both flight and weather data, is dedicated to the development of advanced regression models. The primary aim is to accurately predict delay times for US domestic flights, contributing to enhanced scheduling precision and an improved overall passenger experience.

## Background

Since the relaxation of public health measures for controlling the coronavirus disease, the demand for air travel has been recovering and steadily increasing, with a global air traffic passenger demand growth rate of approximately 64% in 2022 compared to the previous year. As a result, the consequences of flight delays have been subsequently increasing, impacting both customers and airlines. According to the Federal Aviation Administration (FAA), aircraft delays in the United States contributed to an estimated $32.9 billion in direct costs to airlines, airports, and passengers in 2019 [1]. Variables including constrained airspace and airport resources, the extensive volume of aircraft, air traffic controllers, and weather disruptions add further complexity to airline operational processes and cause delays to be inevitable. The inherent complexities and overall scale of the system make delay prediction a challenging problem.

## Literature Review

Several attempts to predict aircraft delay using predictive modeling and simulation have been conducted in advance. In one study, Juan Jose Rebollo and Hamsa Balakrishnan developed various classification and regression models according to 100 origin-destination pairs, discovering that the random forest method yielded the most superior performance [2]. In another study, Yiyang Xu et al. team developed a multiple linear regression model to forecast aircraft delay based on flight delay data published by the Chinese Air Traffic Control Authority, considering temperature, previous delay rate, month, and weekday as influential factors [3]. Apart from a multiple linear regression model, the team also established and employed alternative machine learning models to forecast aircraft delay, including Gradient Boosting, Logistic Regression, K-Near Neighborhood, Gaussian Naive Bayes, Support Vector Machine, Decision Tree, and Random Forest, and observed the corresponding predictive accuracy. In another attempt to analyze aircraft delay, Q. L. Qin and H. Yu used the Fast Fourier Transform method and ANOVA to develop the Fourier Fit Model for predicting delay trends with high precision [4]. However, the predictive analysis was only conducted on a single airport (John F. Kennedy International Airport) and may not be suitable for forecasting aircraft delay in a multiple airport study.

## Objectives

The prediction of aircraft delays has the potential to immediately improve operation performance by enabling Air Traffic Control to take proactive preventive measures and by assisting airlines in organizing recovery procedures at a quicker and more efficient pace. As such, it becomes imperative to identify significant factors responsible for delays and develop a predictive model to forecast flight delays. This paper collects and analyzes extensive flight data, coupled with weather data from arrival and departure airports. The regression models presented in this paper attempt to predict future aircraft delays for domestic flights of the top 30 busiest airports and top 10 airlines with the highest revenue earned in the United States by considering past delays in the network.

The definitions of significant key terms are described below:

- **Departure Delay of Flight**: This quantity is defined as the difference between the actual time that an aircraft pushes away from the terminal gate and its scheduled gate departure time. The departure delay is assumed to be nonnegative. If a flight departs ahead of schedule, the corresponding departure delay is set to 0.
- **Arrival Delay of Flight**: This quantity is defined as the difference between the actual time an aircraft arrives at its terminal gate and its scheduled gate arrival time. The arrival delay is assumed to be nonnegative. If a flight arrives ahead of schedule, the corresponding arrival delay is set to 0.

## Results Summary

Through thorough exploratory data analysis to understand data trends and employing advanced model selection techniques, we achieve a low amount of prediction error compared to the original ordinary least squares method. Utilizing BIC, PLS, and other model selection strategies, our approach results in a decrease in the root mean square error (RMSE) to around 17 for predicting both arrival and departure delay times. This translates to an average difference of 17 minutes between our predicted and actual delay times, showcasing the effectiveness of our regression models.

## References

1. Anupkumar, A. (2023, May). Investigating the costs and economic impact of flight delays in the aviation industry and the potential strategies for reduction https://scholarworks.lib.csusb.edu/cgi/viewcontent.cgi?article=2885&context=etd 
2. Rebollo, J., & Balakrishnan, H. (n.d.). Characterization and Prediction of Air Traffic Delays. MIT - Massachusetts Institute of Technology. https://www.mit.edu/~hamsa/pubs/RebolloBalakrishnanTRC2014.pdf
3. Xu, Y., Liu, L., Gao, X., & Zeng, F. (2019, January). Analysis of Factors in Flight Delay. ResearchGate. https://www.researchgate.net/publication/337952687_Analysis_of_Factors_in_Flight_Delay
4. Qin, Q., & Yu, H. (2015, November 29). A Statistic Analysis of Flight Delays of Major US Airports: Illustrated by the Example of the JFK Airport. SpringerLink. https://link.springer.com/chapter/10.1007/978-3-662-43871-8_68
