# ARQUITECTURA DEL SISTEMA - OLIMPIA STORE

## Stack Tecnológico
- **Backend:** Laravel 10 + PHP 8.2+
- **Frontend:** Blade + TailwindCSS + Alpine.js
- **Base de datos:** MySQL 8.0
- **Cache:** Redis
- **Queue:** Laravel Horizon
- **Search:** Laravel Scout + Algolia

## Estructura de Módulos

app/
├── Modules/
│ ├── Auth/ # Autenticación y usuarios
│ ├── Products/ # Catálogo de productos
│ ├── Orders/ # Gestión de pedidos
│ ├── Inventory/ # Control de inventario
│ ├── Payments/ # Pasarelas de pago
│ ├── Invoicing/ # Facturación electrónica
│ └── Integrations/ # Shopify, Mercado Libre, etc.

## Patrones de Diseño
- Repository Pattern
- Service Classes
- API Resources
- Event Listeners
- Job Queues