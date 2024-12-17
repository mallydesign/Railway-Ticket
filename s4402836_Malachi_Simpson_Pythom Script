# Prices for destinations
prices = {
    "London": 10.15,
    "Manchester": 22.50,
    "Birmingham": 21.40
}

# Function to print receipt
def print_receipt(name, destination, num_tickets, total_cost):
    print("\n--- Receipt ---")
    print(f"Name: {name}")
    print(f"Destination: {destination}")
    print(f"Number of Tickets: {num_tickets}")
    print(f"Total Cost: £{total_cost:.2f}")
    print("Thank you for your purchase!")
    print("----------------\n")

# Main Program
while True:
    # Get user's name
    name = input("What is your name? ").strip()
    
    # Select destination
    print("\nAvailable Destinations:")
    for destination in prices.keys():
        print(f"- {destination}")
    
    destination = input("\nPlease select your destination: ").strip()
    if destination not in prices:
        print("Invalid destination selected. Please try again.\n")
        continue
    
    # Get number of tickets
    try:
        num_tickets = int(input("How many tickets would you like to purchase? "))
        if num_tickets <= 0:
            print("Please enter a valid number of tickets.\n")
            continue
    except ValueError:
        print("Invalid input. Please enter a number.\n")
        continue
    
    # Calculate total cost
    total_cost = prices[destination] * num_tickets
    
    # Display transaction summary
    print(f"\n--- Transaction Summary ---")
    print(f"Name: {name}")
    print(f"Destination: {destination}")
    print(f"Number of Tickets: {num_tickets}")
    print(f"Total Cost: £{total_cost:.2f}")
    print("---------------------------\n")
    
    # Ask if they want a receipt
    print_receipt_option = input("Would you like to print a receipt? (yes/no): ").strip().lower()
    if print_receipt_option == "yes":
        print_receipt(name, destination, num_tickets, total_cost)
    
    # Ask if they want to make another purchase
    another_purchase = input("Would you like to make another purchase? (yes/no): ").strip().lower()
    if another_purchase != "yes":
        print("Thank you for using the system. Goodbye!")
        break
