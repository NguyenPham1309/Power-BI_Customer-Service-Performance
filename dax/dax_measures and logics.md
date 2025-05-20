// This file contains the DAX logic for key measures and calculated columns
// It serves as a reference and documentation for the DAX code.
// -----------------------------------------------------------------------------
// Create the date table handling the time analysis
Date = CALENDAR(date(2021,01,01),DATE(2021,03,31))

//Format into the different unit of time

//Month column (from Jan-Mar)
Month = FORMAT('Date'[Date],"mmmm")

//Month in number (from 1-12)
Monthnum = MONTH('Date'[Date])

//Day of week (from Mon-Sun)
DayofWeek = FORMAT('Date'[Date],"dddd")

//Day of week in number (from 1-7)
Dayofweek_num = FORMAT('Date'[Date],"w")

//Week in number (from 1-52)
Weeknum = FORMAT('Date'[Date],"ww")

//Extract the day number from the date (from 1-31)
Datenum = FORMAT('Date'[Date],"dd")

//Create a month column using to sort the month (not by alphabetical order but by number 1-2-3)
SortMonth = SWITCH('Date'[Month],"January",1,"February",2,"March",3)

