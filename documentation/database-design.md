# DISEÑO DE BASE DE DATOS

## Tablas Principales
- users (id, name, email, password, role_id, ...)
- roles (id, name, permissions)
- products (id, name, sku, price, stock, ...)
- categories (id, name, parent_id, ...)
- orders (id, user_id, status, total, ...)
- order_items (id, order_id, product_id, quantity, price)
- inventories (id, product_id, stock, alerts)
- payments (id, order_id, method, status, ...)
- invoices (id, order_id, electronic_data, ...)