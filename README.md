# OOP-Coffee-Dispensing-Machine

This is a Python-based coffee-making simulation program. It models a coffee machine's operations, including managing resources, processing orders, handling payments, and preparing drinks. 

## Features
- **Resource Management:** Tracks the availability of water, milk, and coffee.
- **Menu Options:** Offers three drink options - latte, espresso, and cappuccino.
- **Payment System:** Handles coin-based payment and calculates change.
- **Dynamic Interaction:** Takes user input to order drinks or check machine status.

## How It Works
1. The program runs in a loop, prompting the user to:
   - Choose a drink.
   - View the machine's resource report.
   - Turn off the machine.
2. If a drink is selected:
   - The program checks if enough resources are available.
   - Processes the payment by simulating coin insertion.
   - Deducts the required ingredients and serves the drink.
3. Users can also type `report` to view the available resources and profit or `off` to shut down the machine.

## Menu Options
The coffee machine offers the following drinks:
- **Latte**: Requires 200ml water, 150ml milk, 24g coffee, and costs $2.50.
- **Espresso**: Requires 50ml water, 0ml milk, 18g coffee, and costs $1.50.
- **Cappuccino**: Requires 250ml water, 50ml milk, 24g coffee, and costs $3.00.

## Code Structure
The program is organized into several classes:

1. **`CoffeeMaker`**:
   - Manages resources like water, milk, and coffee.
   - Checks if resources are sufficient to make a drink.
   - Updates resources after making a drink.

2. **`Menu`**:
   - Provides available drink options.
   - Retrieves drink details based on user input.

3. **`MenuItem`**:
   - Models individual drinks with their ingredients and cost.

4. **`MoneyMachine`**:
   - Handles coin-based payments.
   - Tracks total profit and calculates change.

## How to Use
1. Clone this repository to your local machine.
2. Ensure you have Python installed.
3. Run the script:
   ```bash
   python coffee_machine.py
