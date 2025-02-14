# Math_While_Loop
# Python WHILE - Do Math On User Input Lab

'''
Coding Challenge:
WHILE - Do Math On User Input Lab

- Ask user for an integer number greater than 20
- Test the <user_number> to see if it's an integer
- Set our initial <count> variable to 0
- While our <User_number> is greater than 1
- Divide the <user_number> by 2
- Increase our <count> by 1
- end

Expected Output:
If the user_number was 20:
  Starting Code Challenge
  Enter an integer number 20 or greater > 20
  Your number 20 is a valid Integer 20 or greater. Thanks
  Starting While Loop - Print Count Variable
  The user input started as  20
  The current value of the user input after some math is 10.0
  The while loop has looped 1 time
  The current value of the user input after some math is 5.0
  The while loop has looped 2 time
  The current value of the user input after some math is 2.5
  The while loop has looped 3 time
  The current value of the user input after some math is 1.25
  The while loop has looped 4 time
  The current value of the user input after some math is 0.625
  The while loop has looped 5 time
  Ending While Loop
  The While Loop, looped a total of 5 times
  Ending Code Challenge
'''

# Your Code Starts Here:

# Include any Libraries
# Declare Any Global Variables

def main():
    print("Starting Code Challenge")
    
    # Ask user for an integer greater than 20 and validate input
    while True:
        try:
            user_number = int(input("Enter an integer number 20 or greater > "))
            if user_number >= 20:
                print(f"Your number {user_number} is a valid Integer 20 or greater. Thanks")
                break
            else:
                print("Please enter a number greater than or equal to 20.")
        except ValueError:
            print("That's not an integer. Please enter a valid integer.")
    
    # Initialize the count variable to 0
    count = 0

    # Starting the while loop to divide the user number by 2
    print("Starting While Loop - Print Count Variable")
    original_number = user_number  # Save the original number for reference
    while user_number > 1:
        user_number /= 2  # Divide the number by 2
        count += 1  # Increment the count
        
        # Print current state after each division
        print(f"The current value of the user input after some math is {user_number}")
        print(f"The while loop has looped {count} time{'s' if count > 1 else ''}")
    
    # Ending the while loop
    print("Ending While Loop")
    print(f"The While Loop, looped a total of {count} times")

    # Ending Code Challenge
    print("Ending Code Challenge")

main()

