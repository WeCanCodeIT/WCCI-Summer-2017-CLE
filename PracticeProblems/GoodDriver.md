# Good Driver
You work for a car insurance company that is running a special deal for good drivers. In order for a customer to be given "Good Driver" status, the driver must install a Good Driver Device in their car that will track their driving. Your job is to develop the software that will run calculations based on their trips and output a report.

### Good Driver Input
The Good Driver Device reports driving data in a text file called `DrivingRecord.txt`. The file contains the following information:
```
Driver Lauren
Driver Jarryd
Driver Daniel
Driver Jordan
Trip Lauren 07:15 07:45 17.3
Trip Lauren 06:12 06:32 21.8
Trip Jarryd 12:01 13:16 42.0
Trip Jordan 06:06 12:26 80.2
Trip Jarryd 15:00 15:49 11.4
```
The lines that start with `Driver` have the names of the drivers on the insurance account.
The lines that start with `Trip` have the name of the driver for that trip, the start time of the trip, end time of the trip, and number of miles traveled for that trip.

**NOTE: All times are based on a 24-hour clock, so you can assume the end time will always be greater than the start time. Drivers will never drive past midnight.

### Good Driver Output
You are required to output a summary report to the console window. Based on the input in the file, output should be the following:
```
Jordan: 80 miles @ 13 mph
Jarryd: 53 miles @ 26 mph
Lauren: 39 miles @ 47 mph
Daniel: 0 miles
```
The record should include every driver listed on the account, the total number of miles driven and their average speed.
Any trips that have a speed that is less than 5 mph or greater than 100 mph, do not include them in the calculations.
Lastly, the report should be sorted from greatest number of miles to fewest number of miles.

### Getting Started
Clone the [Good Driver repository](https://github.com/WeCanCodeIT/GoodDriverProblem). You will be creating your program as a console application using the cloned project. The text file, called `DrivingRecord.txt`, with the driving record information is already included in the solution. You will need to use [StreamReader](https://www.dotnetperls.com/streamreader) to read the information from the file. You should output your calculations as a record to the console window.

### Expectations
- Your code should be clean and well-organized. 
- You should take an Object Oriented Programming approach to this exercise. 
- Have fun with this!
