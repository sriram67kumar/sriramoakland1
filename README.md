
NOTE: THIS IS A COPY OF Day-Identifier, Arunangsh



sriram kumar

import datetime
date_str = input("Enter a date (YYYY-MM-DD): ")
try:
    date_obj = datetime.datetime.strptime(date_str, '%Y-%m-%d')
    day_of_week = date_obj.weekday()
        days = ["Monday", "Tuesday", "Wednesday", "Thursday", "Friday", "Saturday", "Sunday"]
        print(f"The day of the week for {date_str} is {days[day_of_week]}.")
except ValueError:
    print("Invalid date format. Please use YYYY-MM-DD format.")

