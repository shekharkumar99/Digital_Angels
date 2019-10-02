
## Start Application 
	1. Open Terminal
	2.  Type npm i 
	3.  Then node .'

#### Description:
	Generate 12 x 40 minute timeslots between 9am and 6pm
 Appointments have a 5 minute break between
 Returns an object with the start and end time of each appointment
 <br>

 Appointment times are:
 0900 - 0940, 0945 - 1025, 1030 - 1110, 1115 - 1155
 1200 - 1240, 1245 - 1325, 1330 - 1410, 1415 - 1455
 1500 - 1540, 1545 - 1625, 1630 - 1710, 1715 - 1755 
 <br>

#### `Once the server is running:`

#### `GET http://localhost:3000/timeslots?year=yyyy&month=mm&day=dd`
Displays all available timeslots for the day
eg. http://localhost:3000/timeslots?year=2019&month=10&day=12
<br>

#### `GET http://localhost:3000/days?year=yyyy&month=mm`
Displays weather or not all days of the month currently have available timeslots
eg. http://localhost:3000/days?year=2019&month=10
<br>

#### `POST http://localhost:3000/book?year=yyyy&month=mm&day=dd&hour=hh&minute=mm`
Books an appointment by creating an event in the calendar, provided that the timeslot is available.
eg. http://localhost:3000/days?year=2019&month=10&day=12&hour=9&minute=00
