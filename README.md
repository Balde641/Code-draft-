# Code-draft- from Google
Asking the user for input until they give a valid response
while True:
    try:
        age = int(input("Please enter your age: "))
    except ValueError:
        print("Sorry, I didn't understand that.")
        continue
    except NameError:
        print('No letters. Write numbers(combination between 0..9')
        continue
    if age < 0:
        print("Sorry, your response must not be negative.")
        continue
    else:
        #age was successfully parsed, and we're happy with its value.
        #we're ready to exit the loop.
        break
if age >= 18:
    print("You are able to vote in the United States!")
else:
    print("You are not able to vote in the United States.")
    
    
 While Loops and Input   
## Start with a list containing several names.
names = ['guido', 'jesse', 'jessica', 'tim']

# Start with an empty list. You can 'seed' the list with
#  some predefined values if you like.
#names = []


# Set new_name to something other than 'quit'.
new_name = ''

# Start a loop that will run until the user enters 'quit'.
while new_name != 'tim':
    # Ask the user for a name.
    new_name = input("Please tell me someone I should know, or enter 'quit': ")

    # Add the new name to our list.
    if new_name != 'tim':
        names.append(new_name)

# Show that the name has been added to the list.
print(names)    
