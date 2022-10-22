# Current Classes

[Return to cover letter](https://github.com/SJTapia/resume/tree/main)

I like to think of my schooling as an investment I've made into any future company I may work for, so I thought it might be interesting for you to see what classes I'm currently taking. If you're curious about any classes I've taken previously, definitely feel free to ask!

- Introduction to Information Technology
- Introduction to Problem Solving and Programming
- Intermediate Algebra 
- Elementary Spanish 1

As a bit of fun, here's the most recent (as of 10/21/22) program I wrote for my programming class:

 # Samuel J. Tapia
# October 14, 2022
# INFOTC 1040, Challenge: Number Stats in Dictionary

  numbers_list = []

  def numbers_dictionary():
      # requests necessary file, opens file, and creates a list out of the values 
      input_file = input("Enter the name of the file containing the necessary values: ")


      if input_file == "numbers.txt":
          numbers_file = open("numbers.txt", "r")
      else:
          print("It appears the requested file does not exist.")
      for value in numbers_file:
          extract = float(value)
          numbers_list.append(extract)
      numbers_file.close()

      # returns the name of the file


      # returns the sum of the numbers in the file list
      file_sum = sum(numbers_list)
      # counts how many numbers are in the file list
      file_count = len(numbers_list)
      # averages the numbers in the file list
      file_average = file_sum / file_count
      # returns the maximum value in the file list
      value_max = max(numbers_list)
      # returns the minimum value in the list list
      value_min = min(numbers_list)
      # provides a range of the values
      values_range = value_max - value_min

      #stores the information into a dictionary 
      numbers = {
          #"Name" : file_name,
          "Sum" : file_sum,
          "Count" : file_count,
          "Average" : file_average,
          "Max Value" : value_max,
          "Min Value" : value_min,
          "Range" : values_range
      }

      # Asks the user what information they would like to know, then provides the result
      print()
      print("Available options are as follows: name, sum, count, average, max, min, range")
      print()
      user_input = input("What information would you like to know about the file?: ")
      #if user_input == "name":
      if user_input == "sum":
          result = "The sum of the numbers is: {}"
          print(result.format(numbers.get("Sum")))
      if user_input == "count":
          result = "The count of the numbers is: {}"
          print(result.format(numbers.get("Count")))
      if user_input == "average":
          result = "The average of the numbers is: {}"
          print(result.format(numbers.get("Average")))
      if user_input == "max":
          result = "The largest valued number is: {}"
          print(result.format(numbers.get("Max Value")))
      if user_input == "min":
          result = "The smallest valued number is: {}"
          print(result.format(numbers.get("Min Value")))
      if user_input == "range":
          result = "The range of the numbers is: {}"
          print(result.format(numbers.get("Range")))


  #calls the function
  numbers_dictionary()


[Return to cover letter](https://github.com/SJTapia/resume/tree/main)
