---
name: ux-writing
description: Escribe o revisa textos de interfaz siguiendo buenas prácticas de UX writing, adaptado al producto en curso.
---

# Workflow: /ux-writing

Usa este comando cuando necesites escribir o revisar cualquier texto de interfaz en cualquier producto.

## Cómo invocarlo

```
/ux-writing [elemento] [descripción o contexto]
```

**Ejemplos:**
```
/ux-writing botón para confirmar una compra
/ux-writing mensaje de error cuando el pago falla
/ux-writing estado vacío lista de favoritos primera vez
/ux-writing notificación recordatorio de tarea pendiente
/ux-writing onboarding pantalla de bienvenida app de finanzas
/ux-writing tooltip explicar qué es el CVV en un formulario de pago
```

## Qué hace este workflow

1. Carga la skill `ux-writing` con las buenas prácticas generales
2. Consulta la sección "Configuración del producto" — si no está completa, pregunta los datos necesarios antes de escribir
3. Escribe el texto solicitado aplicando las reglas correspondientes al elemento
4. Si el elemento no está especificado, pregunta antes de continuar

## Parámetros útiles para dar contexto

- **Elemento:** botón, error, estado vacío, notificación, onboarding, título, label, placeholder, tooltip, confirmación destructiva, FAQ
- **Idioma:** especificar si no está definido en la configuración del producto
- **Contexto:** situación del usuario en ese momento del flujo
