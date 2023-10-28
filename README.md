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

    store == Store()
    this portion of the code initializes a new store, creates several products, and adds them to the store's inventory. These products are now available for transactions within this store management system.

    CLI Boolean type for interacting witht the store:
    #Example 
    while True:
    print("\nOptions:")
    print("1. View Product Info")
    print("2. Process Transaction")
    print("3. Exit")
    choice = input("Enter your choice: ")
    Users can select options 1, 2, or 3, with the system providing appropriate responses based on the chosen action.


Sample Usage:

The code provides a sample usage of the classes and a command-line interface to interact with the store. It allows you to:

![Screenshot (164)](https://github.com/Enigma-design/IMS-for-a-Store/assets/53714668/895d4dfa-2f4f-4bb4-bbee-3a6d290d5088)

If an invalid choice is entered in the CLI, it will print "Sorry, I'm not sure what you are looking for."

![Screenshot (165)](https://github.com/Enigma-design/IMS-for-a-Store/assets/53714668/06ddc8bc-195e-40a5-8999-37dfb47d1a80)


    Handles invalid user choices with a message: "Sorry, I'm not sure what you are looking for."


Note: This system does not handle negative quantities
