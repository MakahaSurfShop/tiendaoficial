# Makaha Surf Shop

Tienda online de surf ubicada en Barranco, Lima, Perú.
Especializada en tablas de surf, wetsuits, accesorios y equipamiento para surfistas.

## Tecnologías utilizadas

* HTML
* JavaScript
* TailwindCSS
* Culqi Checkout
* Integración backend para procesamiento de pagos

## Métodos de pago disponibles

* Tarjetas de crédito y débito (Culqi)
* Yape
* Plin
* Transferencia bancaria
* Pago coordinado vía WhatsApp

## Flujo de pago con Culqi

1. El usuario agrega productos al carrito de compras.
2. Se abre Culqi Checkout desde el frontend.
3. Culqi genera un **token seguro de pago**.
4. El token se envía al backend mediante una solicitud `POST`.
5. El backend procesa el pago usando la API de Culqi.
6. Si el pago es aprobado (`status: captured`), se confirma el pedido y se envía el detalle por WhatsApp.

## Web publicada

https://makahasurfshop.github.io/tiendaoficial/

## Repositorio del proyecto

https://github.com/MakahaSurfShop/tiendaoficial
