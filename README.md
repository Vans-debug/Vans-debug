# Function to print a heart shape
def print_heart():
    # Define the size of the heart
    size = 6
    
    # Loop through each row
    for i in range(size):
        # Loop through each column
        for j in range(size * 2):
            # Calculate the condition to print the heart shape
            if ((i == 0 and (j % size == 1 or j % size == 4)) or
                (i == 1 and (j % size == 0 or j % size == 2 or j % size == 3 or j % size == 5)) or
                (i == 2 and (j % size == 0 or j % size == 5)) or
                (i == 3 and (j % size == 1 or j % size == 4)) or
                (i == 4 and (j % size == 2 or j % size == 3)) or
                (i == 5 and j % size == 3)):
                print('*', end='')
            else:
                print(' ', end='')
        print()

# Call the function to print the heart
print_heart()
