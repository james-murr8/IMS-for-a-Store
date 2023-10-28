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

Sample Usage:

The code provides a sample usage of the classes and a command-line interface to interact with the store. It allows you to:

    View product information by providing the product ID.
    Process a transaction by selecting products and quantities, and it prints out the transaction details.
    Exit the application.

If an invalid choice is entered in the CLI, it will print "Sorry, I'm not sure what you are looking for."

        Handles invalid user choices with a message: "Sorry, I'm not sure what you are looking for."

Note: This system does not handle negative quantities
