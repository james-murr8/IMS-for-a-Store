An inentory management system for a general retail store 

Project 1: IMS for Convience Store 


This program provides a basic framework for managing products, inventory, and transactions in a retail or convenience store. It consists of several classes to handle different aspects of the store's operations:

    Product Class:
        Represents a product in the store.
        Attributes: product_id, name, category, price, quantity_in_stock.

    Inventory Class:
        Manages the store's inventory.
        Methods:
            add_product(self, product): Adds a product to the inventory.
            update_stock(self, product_id, quantity): Updates the stock quantity of a product.
            get_product_info(self, product_id): Retrieves information about a product based on its ID.

    Transaction Class:
        Represents a transaction made in the store.
        Attributes: transaction_id, products (a dictionary of products and quantities), total_amount.

    Store Class:
        Represents the store itself, containing an inventory and transaction history.
        Methods:
            process_transaction(self, products): Processes a transaction, updating inventory and generating a transaction record.

Usage:

    Initialization:
        Creates a store instance.
        Adds products (e.g., Water, Soda, Tea, Chips, Gummy bears) to the inventory.

    CLI (Command-Line Interface):

        Offers three options:
            View Product Info (Choice 1): Allows users to view product information by entering a product ID. If the ID is invalid, it prints "Im sorry, we do not have that here."
            Process Transaction (Choice 2): Enables users to add products to a transaction until they enter 0. It calculates the total amount and generates a transaction record.
            Exit (Choice 3): Exits the program.

        Handles invalid user choices with a message: "Sorry, I'm not sure what you are looking for."

Note: This system does not handle edge cases, such as negative quantities or incorrect user inputs. It provides a basic structure that can be extended for more complex store management scenarios.
