# Inventory Management CLI Project

## Overview
This is a command-line inventory management system written in Python, utilizing SQLAlchemy for database operations and SQLite as the database engine. The system allows users to interact with product data, manufacturers, categories, transactions, and user information.

## Setup
1. **Database Configuration:**
   - The SQLite database is configured using SQLAlchemy. The database file is named `Inventory.db`. 
   
2. **Dependencies:**
   - Ensure you have the necessary dependencies installed. You can install them using the following command:
     ``pip install sqlalchemy`` 

## Project Structure
- **`main.py`:** The main script that contains the classes for products, manufacturers, categories, transactions, and users. It also includes the CLI interface for interacting with the inventory system. 

- **`Inventory.db`:** SQLite database file where the data is stored.

## Classes
1. **Product:**
   - Represents a product with attributes such as `productName`, `description`, and `QuantityInStock`.
   - Belongs to a manufacturer and a category.
   - Has a relationship with transactions.

2. **Manufacturer:**
   - Represents a manufacturer with attributes like `Title` and `contactPerson`.
   - Has a relationship with products.

3. **Category:**
   - Represents a category with attributes like `categoryName` and `description`.
   - Has a relationship with products.

4. **Transaction:**
   - Represents a transaction with attributes like `transactionType`.
   - Relates to a specific product.

5. **User:**
   - Represents a user with attributes like `userName`, `firstName`, `lastName`, and `phoneNo`.

## Usage
1. **Run the Script:**
   - Execute the script using the following command:
     ``python main.py``

   - This will start the CLI interface for interacting with the inventory system.

2. **Main Menu Options:**
   - Choose options from the main menu to perform various operations, including viewing products, checking low stock items, calculating average quantity, searching transactions, and quitting the system.

## Contributing
Feel free to contribute to the improvement of this inventory management system. Fork the repository, make your changes, and submit a pull request.
## Link to Entity Relationship Diagram
https://dbdiagram.io/d/65a08d03ac844320aec0ddeb

## Author
- **Diko Mohamed**

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
