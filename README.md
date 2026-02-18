# Vacasa Group — Website de Venta Directa

Sitio web de reservas directas para **Vacasa Group**, empresa de alojamientos en Guatemala con propiedades en Antigua Guatemala y Ciudad de Guatemala.

## Propiedades

| Propiedad | Ubicación | Precio/noche |
|-----------|-----------|-------------|
| El Búcaro A | Antigua Guatemala | $85 USD |
| El Búcaro B | Antigua Guatemala | $85 USD |
| El Búcaro C | Antigua Guatemala | $85 USD |
| El Búcaro D | Antigua Guatemala | $85 USD |
| Recolección | Ciudad de Guatemala, Zona 14 | $70 USD |
| EON | Ciudad de Guatemala, Zona 10 | $55 USD |

## Tecnología

- HTML5 + CSS3 vanilla (sin frameworks)
- JavaScript puro
- [Stripe.js](https://stripe.com/docs/js) para pagos con tarjeta
- Google Fonts: Cormorant Garamond, DM Sans, DM Mono

## Configuración antes de publicar

1. **Stripe**: Reemplaza `pk_test_REEMPLAZA_CON_TU_KEY_AQUI` en el script con tu Publishable Key real desde [stripe.com → Developers → API Keys](https://dashboard.stripe.com/apikeys).
2. **WhatsApp**: Actualiza el número `50212345678` con el número real de contacto.
3. **Email**: Actualiza la dirección de correo de contacto.
4. **Backend de pagos**: El flujo actual de Stripe crea un `paymentMethod` en el frontend pero requiere un backend (ej. función serverless) para completar el cobro real con `PaymentIntents`.

## Estructura

```
vacasa/
└── index.html   # Todo el sitio en un solo archivo (HTML + CSS + JS)
```

## Contacto

Para reservas directas: [vacasagroup.com](https://vacasagroup.com)
