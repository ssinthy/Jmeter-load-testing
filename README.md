# JMeter Performance Testing

## Project Summary:
This project performs load and stress testing on the [Restful Booker API](https://restful-booker.herokuapp.com) using Apache JMeter. The simulated scenario involves:

- Logging in via API
- Creating a booking with randomized data
- Searching for the created booking

The test simulates 120,000 users over a 12-hour period (downscaled in 3 test stages for practical purposes).

## Technology:
- Apache JMeter

## Prerequisite:
- Install Java JDK 8+
- Install Apache JMeter 5.5+

## How to run?
### 1. Run Test from GUI (for debugging)
- Open Apache JMeter
- Load `booking.jmx`
- Click **Start**

### 2. Run Load Test (Headless)
- jmeter -n -t .\booking.jmx -l .\booking.jtl -e -o Reports

## Request summary
### Load testing
![image](https://github.com/user-attachments/assets/d02c9b33-9412-459e-a52b-073523ada097)

## Generated HTML reports
### Load testing
- Load testing Iteration 1
![image](https://github.com/user-attachments/assets/ba182b12-239b-4c89-96f0-5a10c996a21a)

- Load testing Iteration 2
![image](https://github.com/user-attachments/assets/4e87b552-c5e2-4b85-9d9c-7bc87befcc74)

- Load testing Iteration 3
![image](https://github.com/user-attachments/assets/c45d57d5-b17c-4ac3-bd9d-5ebb963948a7)

