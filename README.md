#  Bug Reports - Swag Labs (SauceDemo)

This document contains all identified bugs and defect reports found during testing the Swag Labs application using the `problem_user` credentials.

---

## Bug List Overview

| ID | Bug Title | Severity | Priority |
|---|---|---|---|
| BUG-01 | Home Page - All products display the same image | Medium | Medium |
| BUG-02 | Product Details Page - Item price changes upon clicking item | High | High |
| BUG-03 | Home Page - "Remove" button fails to function | High | High |
| BUG-04 | Product Details Page - "Add to cart" button fails to function | Critical | High |
| BUG-05 | Sidebar Menu - "About" link redirects to a 404 Page Not Found error | Medium | Medium |
| BUG-06 | Products Page - All sorting filter options fail to reorder products | Medium | Medium |
| BUG-07 | Checkout Step One - Typing Last Name clears and truncates First Name field | Critical | High |

---

## Detailed Bug Reports

### BUG-01: Home Page - All products display the same image
* **Description:** Every product listed on the inventory page displays the exact same image (dog photo) regardless of the product type.
* **Environment:** Microsoft Edge | Windows 11
* **Steps to Reproduce:**
  1. Login as `problem_user`.
  2. Navigate to the products inventory page.
* **Expected Result:** Each product displays its unique corresponding image.
* **Actual Result:** All products render with the same dog picture.

---

### BUG-02: Product Details Page - Item price changes upon clicking item
* **Description:** Opening a product's details page displays a price different from the price shown on the inventory listing page.
* **Environment:** Microsoft Edge | Windows 11
* **Steps to Reproduce:**
  1. Login as `problem_user`.
  2. Note the price of any item on the home page (e.g., $29.99).
  3. Click on the item to open its details page.
* **Expected Result:** The price on the details page matches the inventory listing price.
* **Actual Result:** The price changes dynamically to an incorrect value on the details page.

---

### BUG-03: Home Page - "Remove" button fails to function
* **Description:** Clicking the "Remove" button on the home page for an added item does not remove it from the shopping cart.
* **Environment:** Microsoft Edge | Windows 11
* **Steps to Reproduce:**
  1. Add an item to the cart from the main inventory page.
  2. Click the **Remove** button on the same item page.
* **Expected Result:** The item is removed, and the button changes back to "Add to cart".
* **Actual Result:** The button stays as "Remove" and the cart count does not update.

---

### BUG-04: Product Details Page - "Add to cart" button fails to function
* **Description:** Clicking "Add to cart" inside any product's details page fails to add the product to the shopping cart.
* **Environment:** Microsoft Edge | Windows 11
* **Steps to Reproduce:**
  1. Login as `problem_user`.
  2. Click on any product to open its details page.
  3. Click the **Add to cart** button.
* **Expected Result:** The product is added to the cart and the counter increments.
* **Actual Result:** Clicking the button does nothing.

---

### BUG-05: Sidebar Menu - "About" link redirects to a 404 Page Not Found error
* **Description:** The "About" navigation link in the side menu points to an invalid/broken URL resulting in a 404 error.
* **Environment:** Microsoft Edge | Windows 11
* **Steps to Reproduce:**
  1. Open the burger menu at the top left.
  2. Click on the **About** link.
* **Expected Result:** Redirection to `https://saucelabs.com/`.
* **Actual Result:** Redirection to a broken page displaying **404 - Page Not Found**.

---

### BUG-06: Products Page - All sorting filter options fail to reorder products
* **Description:** Selecting any option from the product sorting dropdown (A-Z, Z-A, Price low-high, Price high-low) fails to change the order of the product list.
* **Environment:** Microsoft Edge | Windows 11
* **Steps to Reproduce:**
  1. Select any sorting option from the top-right filter dropdown.
* **Expected Result:** Product list re-orders according to the selected option.
* **Actual Result:** The product list order remains static.

---

### BUG-07: Checkout Step One - Typing Last Name clears and truncates First Name field
* **Description:** Entering text into the "Last Name" field automatically clears/truncates the input in the "First Name" field down to a single character.
* **Environment:** Microsoft Edge | Windows 11
* **Steps to Reproduce:**
  1. Proceed to Checkout Step One.
  2. Enter a full name in **First Name** (e.g., `mariam`).
  3. Click and type in **Last Name** (e.g., `123`).
* **Expected Result:** Both input fields retain their original entered text.
* **Actual Result:** The First Name input is truncated to a single character (e.g., `a`).
## Trello Board Screenshots

![Trello Board Overview](./Bug%20Report%20screen%20shots/your_image_name.png)
