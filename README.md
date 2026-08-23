# 🐛 Bug Reports - Swag Labs (SauceDemo)

## 📌 Project Description
This repository contains comprehensive Quality Assurance (QA) documentation and defect reports for the **Swag Labs (SauceDemo)** e-commerce application under `problem_user` scenarios.

---

## 📋 Trello Board Overview

![Trello List 1](./Bug-Report-Screenshots/Listscreenshot1.png)
![Trello List 2](./Bug-Report-Screenshots/Listscreenshot2.png)
![Trello List 3](./Bug-Report-Screenshots/Listscreenshot3.png)
![Trello List 4](./Bug-Report-Screenshots/Listscreenshot4.png)
![Trello List 5](./Bug-Report-Screenshots/Listscreenshot5.png)
![Trello List 6](./Bug-Report-Screenshots/Listscreenshot6.png)
![Trello List 7](./Bug-Report-Screenshots/Listscreenshot7.png)

---

## 📑 Bug List Summary

| ID | Bug Title | Severity | Priority |
|---|---|---|---|
| BUG-01 | Home Page - All products display the same image | Medium | Medium |
| BUG-02 | Product Details Page - Item price changes upon clicking item | High | High |
| BUG-03 | Home Page - "Remove" button fails to function | High | High |
| BUG-04 | Product Details Page - "Add to cart" button fails for all products | Critical | High |
| BUG-05 | Sidebar Menu - "About" link redirects to 404 Page Not Found | Medium | Medium |
| BUG-06 | Products Page - All sorting filter options fail to reorder products | Medium | Medium |
| BUG-07 | Checkout Step One - Typing Last Name clears First Name field | Critical | High |

---

## 🔍 Detailed Bug Reports

### BUG-01: Home Page - All products display the same image
* **Description:** Every product listed on the inventory page displays the exact same image (dog photo) regardless of the product type.
* **Environment:** Microsoft Edge | Windows 11
* **Steps to Reproduce:**
  1. Login as `problem_user` with password `secret_sauce`.
  2. Navigate to the main inventory page (`/inventory.html`).
* **Expected Result:** Each product should display its unique corresponding item image.
* **Actual Result:** All products render with the same dog picture (`sl-404.jpg`).

**Screenshots:**
![BUG-01 Image 1](./Bug-Report-Screenshots/bug-01-same-images.png.png)
![BUG-01 Image 2](./Bug-Report-Screenshots/bug-01-same-images.png2.png)
![BUG-01 Image 3](./Bug-Report-Screenshots/bug-01-same-images.png3.png)

---

### BUG-02: Product Details Page - Item price changes upon clicking item
* **Description:** Opening a product's details page displays a price different from the price shown on the main inventory listing page.
* **Environment:** Microsoft Edge | Windows 11
* **Steps to Reproduce:**
  1. Login as `problem_user`.
  2. Note the price of any item on the home page (e.g., $29.99).
  3. Click on the product title to open its details page.
* **Expected Result:** The price on the details page must match the inventory listing price.
* **Actual Result:** The price changes dynamically to an incorrect value on the details page.

**Screenshots:**
![BUG-02 Image 1](./Bug-Report-Screenshots/bug-02-price-change.png1.png)
![BUG-02 Image 2](./Bug-Report-Screenshots/bug-02-price-change.png2.png)
![BUG-02 Image 3](./Bug-Report-Screenshots/bug-02-price-change.png3.png)
![BUG-02 Image 4](./Bug-Report-Screenshots/bug-02-price-change.png4.png)
![BUG-02 Image 5](./Bug-Report-Screenshots/bug-02-price-change.png5.png)
![BUG-02 Image 6](./Bug-Report-Screenshots/bug-02-price-change.png6.png)

---

### BUG-03: Home Page - "Remove" button fails to function
* **Description:** Clicking the "Remove" button on the main inventory page for an added item fails to remove it from the cart.
* **Environment:** Microsoft Edge | Windows 11
* **Steps to Reproduce:**
  1. Login as `problem_user`.
  2. Click **Add to cart** on any item on the home page.
  3. Click the newly appeared **Remove** button on the same item card.
* **Expected Result:** The item is removed, the cart count decreases, and the button changes back to "Add to cart".
* **Actual Result:** The button stays as "Remove" and the item remains in the cart.

**Screenshots:**
![BUG-03 Image 1](./Bug-Report-Screenshots/bug-03-remove-button.png1.png)
![BUG-03 Image 2](./Bug-Report-Screenshots/bug-03-remove-button.png2.png)
![BUG-03 Image 3](./Bug-Report-Screenshots/bug-03-remove-button.png3.png)

---

### BUG-04: Product Details Page - "Add to cart" button fails for all products
* **Description:** Clicking the "Add to cart" button inside any individual product details page does nothing.
* **Environment:** Microsoft Edge | Windows 11
* **Steps to Reproduce:**
  1. Login as `problem_user`.
  2. Click on any product title to open its product details page.
  3. Click the **Add to cart** button.
* **Expected Result:** Button text changes to "Remove" and the cart count badge increments by 1.
* **Actual Result:** The button remains stuck as "Add to cart" and no action occurs.

**Screenshots:**
![BUG-04 Image 1](./Bug-Report-Screenshots/bug-04-add-to-cart.png.png)
![BUG-04 Image 2](./Bug-Report-Screenshots/bug-04-add-to-cart.png2.png)
![BUG-04 Image 3](./Bug-Report-Screenshots/bug-04-add-to-cart.png3.png)

---

### BUG-05: Sidebar Menu - "About" link redirects to 404 Page Not Found
* **Description:** The "About" navigation link in the side drawer menu points to a broken URL resulting in a 404 error.
* **Environment:** Microsoft Edge | Windows 11
* **Steps to Reproduce:**
  1. Login as `problem_user`.
  2. Open the burger menu at the top left corner.
  3. Click on the **About** menu item.
* **Expected Result:** User is redirected to `https://saucelabs.com/`.
* **Actual Result:** User lands on a page displaying **404 - Page Not Found**.

**Screenshots:**
![BUG-05 Image 1](./Bug-Report-Screenshots/bug-05-about-404.png.png)
![BUG-05 Image 2](./Bug-Report-Screenshots/bug-05-about-404.png2.png)
![BUG-05 Image 3](./Bug-Report-Screenshots/bug-05-about-404.png3.png)
![BUG-05 Image 4](./Bug-Report-Screenshots/bug-05-about-404.png4.png)

---

### BUG-06: Products Page - All sorting filter options fail to reorder products
* **Description:** Selecting any sorting option from the top-right dropdown filter fails to reorder the product list.
* **Environment:** Microsoft Edge | Windows 11
* **Steps to Reproduce:**
  1. Login as `problem_user`.
  2. Select any filter option from the dropdown (A-Z, Z-A, Price Low-High, Price High-Low).
* **Expected Result:** The product list reorders according to the selected option.
* **Actual Result:** The list remains static and no reordering takes place.

**Screenshots:**
![BUG-06 Image 1](./Bug-Report-Screenshots/bug-06-sorting-filter.png.png)
![BUG-06 Image 2](./Bug-Report-Screenshots/bug-06-sorting-filter.png2.png)
![BUG-06 Image 3](./Bug-Report-Screenshots/bug-06-sorting-filter.png3.png)
![BUG-06 Image 4](./Bug-Report-Screenshots/bug-06-sorting-filter.png4.png)

---

### BUG-07: Checkout Step One - Typing Last Name clears First Name field
* **Description:** Entering input in the Last Name field automatically clears and truncates the previously entered First Name text down to a single character.
* **Environment:** Microsoft Edge | Windows 11
* **Steps to Reproduce:**
  1. Add any item to cart and navigate to Checkout Step One.
  2. Type a full name in **First Name** (e.g., `mariam`).
  3. Click and type text in **Last Name** (e.g., `123`).
* **Expected Result:** Both input fields retain their complete entered values.
* **Actual Result:** First Name input is truncated down to a single character (e.g., `a`).

**Screenshots:**
![BUG-07 Image 1](./Bug-Report-Screenshots/bug-07-lastname-clears-firstname.png.png)
![BUG-07 Image 2](./Bug-Report-Screenshots/bug-07-lastname-clears-firstname.png%202.png)
![BUG-07 Image 3](./Bug-Report-Screenshots/bug-07-lastname-clears-firstname.png3.png)
