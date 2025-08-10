# WordPress Child Theme with Dummy Products (Storefront)

## 📌 Project Overview
This project is a **WordPress Child Theme** based on the **Storefront** theme, enhanced with:
- Custom pages created via **hooks** in `functions.php`.
- Dummy products added programmatically using WooCommerce functions.
- Template customizations for better structure and semantic markup.
- Proper use of **WordPress coding standards** (hooks, filters, file structure).

---

## 📂 Project Structure

wordpress-child-theme-dummy-products/
│
├── storefront-child/
│ ├── functions.php # Custom hooks, page modifications, and product generation code
│ ├── style.css # Child theme stylesheet (with required Theme Header)
│ ├── templates/ # Template overrides (if any)
│ └── other custom files...
│
├── dummy-product-php.txt # Standalone PHP script to insert dummy products
└── README.md # Project documentation


---

## ⚙️ Features Implemented

### 1. **Child Theme Creation**
- Based on **Storefront** theme.
- Contains `style.css` with required Theme Header for WordPress to recognize it.
- Uses `functions.php` to enqueue parent theme styles and add new functionality.

### 2. **Custom Pages via Hooks**
- Used **WooCommerce & WordPress hooks** to inject custom content into specific locations.
- Example: Adding banners, featured products, or promotional text without editing core files.

### 3. **Dummy Products (Programmatic Creation)**
- Script in `dummy-product-php.txt` contains PHP code to:
  - Create multiple dummy products.
  - Set product titles, descriptions, prices, images, and categories.
  - Support WooCommerce product types (Simple, Variable, etc.).

### 4. **Template Customization**
- Overrode specific WooCommerce templates for improved layout.
- Ensured semantic HTML for better accessibility and SEO.

### 5. **WordPress Standards & Code Quality**
- Followed **WordPress coding standards**.
- Used `add_action` and `add_filter` instead of direct template edits.
- Code is clean, readable, and reusable.

---

## 🛠 Installation & Usage

1. **Upload Child Theme**
   - Copy `storefront-child/` to your WordPress `/wp-content/themes/` folder.
   - Activate it from the WordPress Dashboard → Appearance → Themes.

2. **Install & Activate WooCommerce**
   - Go to Plugins → Add New → Search "WooCommerce" → Install → Activate.

3. **Import Dummy Products**
   - Open `dummy-product-php.txt`.
   - Copy its code into your child theme's `functions.php` (or create a simple plugin).
   - Refresh your site (the code will add products automatically).

---

## 📄 Notes
- This project **does not edit** the parent theme directly — ensuring updates won't break changes.
- Uses **hooks and filters** for maximum flexibility.
- Follows **best practices** for WooCommerce development.

---

## 👨‍💻 Author
- Developed as part of a WordPress/WooCommerce customization task.
- By: *[Ashish Badhwar]*

