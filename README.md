# foodtrack-db
Plataforma para gestionar operaciones de foodtrucks en distintos puntos de una ciudad
# FoodTrack DB

## 📌 Descripción

FoodTrack es una plataforma para gestionar operaciones de foodtrucks en distintos puntos de una ciudad.

Este proyecto implementa el esquema relacional inicial utilizando SQL Server, con control de versiones mediante Git y GitHub.

---

## 🧱 Modelo de Datos

El sistema incluye las siguientes entidades:

* foodtrucks
* products
* orders
* order_items
* locations

### Relaciones principales:

* Un foodtruck tiene múltiples productos, pedidos y ubicaciones
* Un pedido contiene múltiples ítems (order_items)
* Cada ítem referencia un producto

---

## 📂 Estructura del Proyecto

```
/data/      → archivos CSV
/scripts/   → scripts SQL
README.md   → documentación
```

---

## ⚙️ Cómo ejecutar

1. Crear base de datos en SQL Server
2. Ejecutar:

   * `scripts/01_create_schema.sql`
   * `scripts/02_alter_orders.sql`
3. (Opcional) importar datos desde `/data/`

---

## 🚀 Tecnologías utilizadas

* SQL Server
* DBeaver
* Git / GitHub

---

## 📈 Posibles mejoras

* Automatización de carga de datos con Python
* Validación de integridad avanzada
* Implementación de stored procedures
