# General-Store-Management-System-in-C-using-OOPS

This is a **Store Management System** built in C++ that allows users to manage products, maintain a shopping cart, generate bills, and handle wishlists. It is designed for small-scale retail businesses or educational purposes to demonstrate inventory management and billing functionalities.

---

## Features

### Core Functionality
1. **Product Management**:
   - Load products from a `products.csv` file.
   - View all available products with details like name, price, stock, and category.

2. **Shopping Cart**:
   - Add products to the cart.
   - Remove products from the cart.
   - Save the current cart to a file (`saved_cart.txt`) for later use.
   - Load a previously saved cart.

3. **Wishlist**:
   - Add products to a wishlist.
   - Move all wishlist items to the cart (if stock is available).

4. **Billing System**:
   - Generate detailed bills with subtotal, discount, tax, and total amount.
   - Save the bill as a receipt in `receipt.txt`.
   - Apply custom discounts and tax rates during billing.

5. **Inventory Updates**:
   - Automatically updates product stock when items are added to or removed from the cart.

6. **User-Friendly Menu**:
   - A simple text-based menu system guides users through all available actions.

---

## Installation and Setup

### Prerequisites
- **C++ Compiler**: Ensure you have a C++ compiler installed (e.g., GCC or Clang).
- **Text Editor**: Use any text editor or IDE for viewing and modifying the code (e.g., VS Code, CLion, or Sublime Text).

### Steps to Run the Application
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/store-management-system.git
   ```

2. **Navigate to the Project Directory**:
   ```bash
   cd store-management-system
   ```

3. **Prepare the `products.csv` File**:
   - Create a file named `products.csv` in the project directory.
   - Populate it with product data in the following format:
     ```
     Laptop,1200.50,10,Electronics
     Smartphone,699.99,25,Electronics
     Headphones,149.99,50,Accessories
     Notebook,12.99,100,Stationery
     Pen,1.99,500,Stationery
     ```

4. **Compile the Code**:
   Open a terminal and compile the program using:
   ```bash
   g++ -o store_management main.cpp
   ```

5. **Run the Application**:
   Execute the compiled binary:
   ```bash
   ./store_management
   ```

6. **Interact with the System**:
   - Follow the on-screen instructions to navigate the menu and perform actions.

---

## Usage Instructions

### 1. View All Products
- Select option `1` from the menu to view all available products along with their prices, stock levels, and categories.

### 2. Add Product to Cart
- Select option `2`, enter the product name, and specify the quantity to add it to your cart.

### 3. Remove Product from Cart
- Select option `3`, enter the product name, and remove it from your cart. The stock will be updated accordingly.

### 4. View Cart
- Select option `4` to view the contents of your cart. If the cart is empty, you'll receive a notification.

### 5. Save and Load Cart
- Use options `5` and `6` to save the current cart to `saved_cart.txt` or load a previously saved cart.

### 6. Wishlist Management
- Add products to your wishlist using option `7`.
- View your wishlist using option `8`.
- Move all wishlist items to the cart using option `9` (if stock is available).

### 7. Generate Bill
- Select option `10` to generate a detailed bill. You can apply custom discounts and tax rates during this process.
- The bill will be displayed on the console and saved as `receipt.txt`.

### 8. Exit
- Select option `11` to exit the application.

---

## Example Workflow

1. Start the application:
   ```bash
   ./store_management
   ```

2. View available products:
   ```
   --- Available Products ---
   Laptop - Rs.1200.50 (Electronics) Stock: 10
   Smartphone - Rs.699.99 (Electronics) Stock: 25
   Headphones - Rs.149.99 (Accessories) Stock: 50
   Notebook - Rs.12.99 (Stationery) Stock: 100
   Pen - Rs.1.99 (Stationery) Stock: 500
   ```

3. Add a product to the cart:
   ```
   Enter product name to add to cart: Laptop
   Enter quantity: 1
   Laptop added to cart.
   ```

4. Generate a bill:
   ```
   Enter discount percentage: 10
   Enter tax rate percentage: 5

   --- Current Bill ---
   Laptop            x1  Rs.1200.50

   Subtotal: Rs.1200.50
   Discount (10%): Rs.120.05
   Tax (5%): Rs.54.02
   Total: Rs.1134.47
   ```

5. Save the receipt:
   ```
   Detailed receipt saved to receipt.txt
   ```

---

## File Structure

### Input Files
- **`products.csv`**:
  - Contains product details in the format: `Name,Price,Stock,Category`.
  - Example:
    ```
    Laptop,1200.50,10,Electronics
    Smartphone,699.99,25,Electronics
    ```

### Output Files
- **`receipt.txt`**:
  - Generated bill with subtotal, discount, tax, and total amount.
  - Example:
    ```
    ============================================
               ASHISH STORE RECEIPT          
    ============================================
    Date: Mon Mar 11 03:10:00 2025
    --------------------------------------------
    Item                     Qty      Price     Total
    Laptop                   x1       Rs.1200.50 Rs.1200.50
    --------------------------------------------
    Subtotal:                Rs.1200.50
    Discount (10%):          Rs.120.05
    Tax (5%):                Rs.54.02
    TOTAL:                   Rs.1134.47
    ============================================
    ```

- **`saved_cart.txt`**:
  - Saves the current cart state for later use.
  - Example:
    ```
    Laptop,1
    Smartphone,2
    ```

---

## Customization

### Adding New Products
To add more products:
1. Open the `products.csv` file.
2. Add new entries in the format:
   ```
   ProductName,Price,Stock,Category
   ```

### Modifying Discounts and Taxes
- During billing, you can specify custom discount percentages and tax rates.

### Enhancements
- Extend the system to support user accounts and multiple stores.
- Add a graphical user interface (GUI) using libraries like Qt or SFML.

---

## Screenshots

### Main Menu
![Main Menu](screenshots/main_menu.png)

### Bill Generation
![Bill Generation](screenshots/bill_generation.png)

*(Replace the above image paths with actual screenshots of your application.)*

---

## Contributing

Contributions are welcome! If you'd like to improve this project, please follow these steps:
1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Submit a pull request with a detailed description of your changes.

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## Acknowledgments

- Inspired by real-world store management systems.
- Built using C++ for efficient and lightweight performance.

---

Feel free to reach out with any questions or suggestions! Enjoy managing your store! 🛒
