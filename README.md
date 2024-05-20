Contains analysis and results from Practical Application 1 Assignment
Problems
1-3. Data Cleaning and Identify Nans.
The following was done to clean the data being analyzed.
Car column presented very little information (mostly missing NAN values) so it was decided to drop that column as the data was not usefull.
The rest of the columns are object types, the rows that indicate a nan are minimal so those rows were dropped. The passenger column was renamed to correct spelling.
Lastly, the age entries titled below21 and plus50 were transformed to greater than and less than notations.

4. What proportion of the total observations chose to accept the coupon?
num_accept = sum(data_rm['Y'] == 1)/len(data_rm)*100
print(num_accept)
~57% of total observations accepted a coupon

5. Use a bar plot to visualize the `coupon` column.
![image](https://github.com/JJcancan/Practical-Application-1/assets/165223563/56b46c34-a09d-472b-a6da-62ffe5ed4742)

6. Use a histogram to visualize the temperature column.
![image](https://github.com/JJcancan/Practical-Application-1/assets/165223563/793de41b-bb4c-4089-a0cd-d0996a7fa86b)

Bar Coupon Questions
2. What proportion of bar coupons were accepted?
num_accept_bar = sum(Bar_data['Y'] == 1)/len(Bar_data)*100
print(num_accept_bar)
~41% of Bar Coupons were accepted

3. Compare the acceptance rate between those who went to a bar 3 or fewer times a month to those who went more.
As expected those that declared that they went three or fewer times a month vs three or more denied the Coupon at a higher rate.
![BarQ3](https://github.com/JJcancan/Practical-Application-1/assets/165223563/202c6c01-03b9-4041-8f12-2f8b8918917e)

4. Compare the acceptance rate between drivers who go to a bar more than once a month and are over the age of 25 to the all others.  Is there a difference?
The group going one or more times a month and are greater than the Age of 25 denied the Bar Coupon more than the rest of participants <= 25 years old who went less than once a month.
![BarQ4](https://github.com/JJcancan/Practical-Application-1/assets/165223563/a1db4a5d-9403-4ffb-807e-397d6a9a8533)


5. Use the same process to compare the acceptance rate between drivers who go to bars more than once a month and had passengers that were not a kid and had occupations other than farming, fishing, or forestry.
![BarQ5](https://github.com/JJcancan/Practical-Application-1/assets/165223563/bd9b2ef4-172a-4a2d-b2f9-3039b6387408)

6. Compare the acceptance rates between those drivers who:

- go to bars more than once a month, had passengers that were not a kid, and were not widowed *OR*
- go to bars more than once a month and are under the age of 30 *OR*
- go to cheap restaurants more than 4 times a month and income is less than 50K.

![image](https://github.com/JJcancan/Practical-Application-1/assets/165223563/60d830fe-f1d4-45c9-9948-995437c528d6)

7.  Based on these observations, what do you hypothesize about drivers who accepted the bar coupons?
Age and the number of visits I think is the main predictors that determine drivers who accept bar coupons.
An additonal countplot provided below shows how much of the drivers are concentrated at 21 years old.
It was observed that in the first figure those who declared they went three or more times were more likely to accept the coupon.
Overall the income does not seem to show a specific range of drivers that accepted the bar coupon based on their income.

![BarQ7_1](https://github.com/JJcancan/Practical-Application-1/assets/165223563/b89e8d75-7c14-48e8-8fb3-60899766f253)
![BarQ7_2](https://github.com/JJcancan/Practical-Application-1/assets/165223563/c7fde92c-1aff-4a53-8612-e9f5f18a8660)
![BarQ7_3](https://github.com/JJcancan/Practical-Application-1/assets/165223563/e26c5848-68b4-4b88-a2e1-ef02a17dfaa7)

Independent Investigation

Using the bar coupon example as motivation, you are to explore one of the other coupon groups and try to determine the characteristics of passengers who accept the coupons.  

1. For the independent investigation, the drivers that accepted a coffee house coupon were analyzed

2. Wanted to see the distribution of occupations within the coffee house data. It was observed that drivers under a student, unemployed, or Computer & Math occupation accepted a majority of the coffee house coupons.
![image](https://github.com/JJcancan/Practical-Application-1/assets/165223563/36c44b32-aca1-4c67-afd1-593e71c22e68)

3. The data was filtered for drivers that declared a student, unemployed, or Computer & Math occupation to see the acceptance rate compared to the rest of the data. Overall the acceptance rate for this pool of drivers is slightly greater than the rest of the other occupations combined.
![image](https://github.com/JJcancan/Practical-Application-1/assets/165223563/c2bc08e7-fc4d-4741-b086-1b6c98437a3f)

4. Next wanted to observe if there was a specific time range and destination. It was observed that the hours 10AM and 2PM were when the majority of the coffee coupon were accepted. It was also observed that "the no urgent" destination was the majority for destinations given. Drivers offered a coffee house coupon at 10AM and 2PM with no urgent destination given had a slightly greater acceptance rate compared to those who were offered outside those hours and with a different destination designated.

![Independent_Q3](https://github.com/JJcancan/Practical-Application-1/assets/165223563/4ad1a5ed-b7bb-4473-b799-7a6e29363dbf)
![Independent_Q4](https://github.com/JJcancan/Practical-Application-1/assets/165223563/91f6efc6-f211-47f7-a4a9-6cc8b6eee1f8)
![Independent_Q5](https://github.com/JJcancan/Practical-Application-1/assets/165223563/f4fec52f-f788-4c24-aee5-853a8c273cc7)

5. Using a count plot it was obsevered that drivers younger than 26 years old were more likely to accept the Coffee House Coupon.
![Independent_Q6](https://github.com/JJcancan/Practical-Application-1/assets/165223563/7ed6f4ce-b936-4104-a499-d8824b8fd26d)
The acceptance rate of those younger than 26 years old is slightly greater than those of other ages.
![image](https://github.com/JJcancan/Practical-Application-1/assets/165223563/03393446-9532-4b6c-81ae-904bc499e8ce)

6.Conclusion
It was observed that the following characteristics could indicate that someone is more inclined to accept the coffee house coupon:
If a driver declares 'Student/Unemployed/Comp & Math' as an occupation, if the driver has no urgent place to go and is given between
'10AM'-'2PM', and if the driver is younger than 26 years old.








   






