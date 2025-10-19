# DISEÑO DE BASE DE DATOS - OLIMPIA STORE

## Tablas Principales

### users
- id, name, email, password, role_id, email_verified_at, remember_token, created_at, updated_at

### roles
- id, name, permissions, created_at, updated_at

### products
- id, name, description, sku, barcode, price, stock, category_id, images, status, created_at, updated_at

### categories
- id, name, description, parent_id, slug, created_at, updated_at

### orders
- id, user_id, order_number, status, total_amount, shipping_cost, tax_amount, payment_method, shipping_address, created_at, updated_at

### order_items
- id, order_id, product_id, quantity, unit_price, total_price

### inventories
- id, product_id, stock_quantity, minimum_stock, status, created_at, updated_at

### payments
- id, order_id, payment_method, transaction_id, amount, status, payment_details, created_at, updated_at

### invoices
- id, order_id, invoice_number, electronic_data, pdf_path, xml_path, status, created_at, updated_at