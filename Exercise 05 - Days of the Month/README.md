## Exercise 5: Days of the Month - 30 Marks

Write a program that tells a user how many days there are in a specific month. Use a dictionary to map the month numbers (1-12) to the number of days in each month.

### Instructions:
1. Create a Dictionary: Define a dictionary where the keys are month numbers and the values are the number of days in those months.
2. Input Handling: Ask the user to input the month number.
3. Check and Output: Use an if-else statement to check if the input is valid and print the number of days in the corresponding month.

### Advanced Requirement:
Leap Year Adjustment: Modify the program to account for leap years. For February, ask the user if the year is a leap year and adjust the number of days accordingly.
def days_in_month():
 month_days = {1: 31, 2: 28, 3: 31,  4: 30, 5: 31, 6: 30,7: 31, 8: 31,9: 30,10: 31 11: 30,12: 31 }
 month = int(input("Enter the month number (1-12): "))
      if month in month_days:
         if month == 2:
            leap_year = input("Is it a leap year? (yes/no): ").strip().lower()
            if leap_year == "yes":
                print("February has 29 days in a leap year.")
            else:
                print("February has 28 days.")
            else:
                print(f"Month {month} has {month_days[month]} days.")
            else:
                  print("Invalid month number. Please enter a number between 1 and 12.")
           if __name__ == "__main__":
                      days_in_month()







       

