sriram kumar

import datetime

# Input date in the format 'YYYY-MM-DD'
date_str = input("Enter a date (YYYY-MM-DD): ")

try:
    # Parse the input date string into a datetime object
    date_obj = datetime.datetime.strptime(date_str, '%Y-%m-%d')
    
    # Get the day of the week as an integer (0 = Monday, 6 = Sunday)
    day_of_week = date_obj.weekday()
    
    # Define a list of day names
    days = ["Monday", "Tuesday", "Wednesday", "Thursday", "Friday", "Saturday", "Sunday"]
    
    # Print the day of the week
    print(f"The day of the week for {date_str} is {days[day_of_week]}.")
except ValueError:
    print("Invalid date format. Please use YYYY-MM-DD format.")

