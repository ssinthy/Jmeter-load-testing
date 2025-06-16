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
```bash
jmeter -n -t .\booking.jmx -l .\booking.jtl -e -o Reports
