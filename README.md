5th homework

Work Day Scheduler

First I get the browser Moment.js by downloading a JS file and linking it to my HTML file.

once linked I include as text in #CurrentId a date from moment().format('dddd, MMMM Do YYYY')

then to host the info from 8 to 5pm I created an Array named workTime, with Subarrays as follows
        var workTime = [
            ["8 AM", ""],
            ["9 AM", ""],
            ["10 AM", ""],
            ["11 AM", ""],
            ["12 PM", ""],
            ["1 PM", ""],
            ["2 PM", ""],
            ["3 PM", ""],
            ["4 PM", ""],
            ["5 PM", ""],
            ];

I created a variable where i get only the first 2 digits of the hour and if it is PM or AM to get convert to a 2 hrs format value. this will be used again to define the classes of each row/hour.

then to create the divs to display the timeslots i use a For loop were from 0 to my array length i append the rowas and columns adding the right attributes of class specifically as stated in the css file
an if applies the class correcponding to each row if the hour is less, equal or higher than the hour the row repreents.

after the timeslots are created, an On Click event saves the input in the specific row to the index in the array and at the same time in local storage.