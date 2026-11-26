# Hiperpharma: backoffice AdonisJS de la droguería (archivo histórico)

![Estado: archivo histórico](https://img.shields.io/badge/Estado-archivo%20hist%C3%B3rico-lightgrey) ![AdonisJS 4.1](https://img.shields.io/badge/AdonisJS%204.1-5A45FF) ![Node.js](https://img.shields.io/badge/Node.js-339933) ![MySQL](https://img.shields.io/badge/MySQL-4479A1)

> [!NOTE]
> Código original del panel administrativo de Hiperpharma, droguería con venta en línea (2020). El producto continúa en **[pharmacy-ecommerce-platform](https://github.com/KevinAndrey96/pharmacy-ecommerce-platform)**, que reúne todos sus componentes con documentación actualizada.

## Qué contiene

- Autenticación por sesión y recuperación de contraseña.
- CRUD de productos con variantes (producto padre), categorías y clientes.
- Modelo de pedidos con detalle de productos y pasarela de pago (`OrderController` y migraciones).
- Migraciones para cupones de descuento y suscriptores del newsletter.
- Tablero con estadísticas de ventas y vistas Edge sobre una plantilla Bootstrap.

## Stack original

| Componente | Tecnología |
| :--- | :--- |
| Framework | AdonisJS 4.1 (Lucid ORM, Shield, Auth) |
| Vistas | Edge |
| Base de datos | MySQL |
| Frontend | Plantilla Bootstrap con librerías Bower incluidas en `public/vendors` |

## Ejecutarlo localmente

```bash
cp .env.example .env    # completa DB_* con una base MySQL local
npm ci                  # node_modules no se versiona
npx adonis key:generate
npx adonis migration:run
npm start               # http://localhost:3333
```

Requiere Node.js 14 y MySQL 5.7 u 8. AdonisJS 4.1 ya no recibe soporte, así que conviene ejecutarlo solo como referencia.

## Estado del repositorio

- Se conserva sin cambios funcionales como referencia del código original (2020).
- No recibe actualizaciones de dependencias; el mantenimiento ocurre en [pharmacy-ecommerce-platform](https://github.com/KevinAndrey96/pharmacy-ecommerce-platform).
- En noviembre de 2026 se depuró el historial completo: se retiraron `node_modules/` (7.588 archivos), el `.env` con credenciales y 19 ramas de Dependabot. Todos los commits conservan su fecha original.

## Autoría

Kevin Andrey Herrera Silva ([@KevinAndrey96](https://github.com/KevinAndrey96)).

## Licencia

Código desarrollado para un cliente y publicado como muestra de portafolio. No incluye licencia de código abierto: todos los derechos reservados.
