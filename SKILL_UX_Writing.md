---
name: ux-writing
description: >
  Guía de UX writing para interfaces digitales. Usá esta skill siempre que necesites
  escribir o revisar textos de una app o plataforma web: botones, CTAs, labels, títulos,
  subtítulos, mensajes de error, estados vacíos, onboarding, notificaciones, tooltips,
  placeholders, confirmaciones, formularios y FAQs. También activala cuando haya dudas
  sobre tono, capitalización, puntuación, hipervínculos o formato de datos en la interfaz.
  Antes de escribir cualquier texto, consultar la sección "Configuración del producto" para
  adaptar voz, idioma y persona gramatical al proyecto en curso.
---

# UX Writing Skill

Guía de buenas prácticas para escribir textos de interfaz claros, consistentes y centrados
en el usuario. Las reglas son independientes del producto — para aplicarlas correctamente,
completar primero la sección de configuración.

---

## Configuración del producto

Antes de escribir, definir estos parámetros para el proyecto en curso. Si no están definidos,
preguntar al usuario antes de continuar.

| Parámetro | Valor para este proyecto |
|---|---|
| Nombre del producto | — |
| Idioma/s | — |
| Persona gramatical | — (ej: tú, usted, vos, you) |
| Tono general | — (ej: amigable, formal, técnico) |
| Audiencia principal | — |

---

## Principios generales

Todo texto de interfaz debe cumplir estas condiciones:

**Claro** — El usuario entiende qué significa y qué hacer sin tener que pensar.
**Conciso** — Sin palabras innecesarias. Si se puede decir en menos, mejor.
**Útil** — Aporta información relevante en el momento justo.
**Consistente** — Los mismos elementos usan siempre los mismos patrones y términos.
**Centrado en el usuario** — Habla de beneficios para el usuario, no de features del producto.

---

## Voz y tono

La **voz** es constante — define la personalidad del producto.
El **tono** varía según el contexto emocional del usuario en cada momento.

### Qué hace una buena voz de producto
- Habla de igual a igual, sin condescendencia
- Usa verbos de acción directa
- Evita lenguaje corporativo o burocrático
- No culpa al usuario

### Qué NO hace
- No usa jerga técnica sin necesidad
- No usa frases genéricas como "Ha ocurrido un error inesperado"
- No es condescendiente ni sobreexplica
- No usa "haz clic aquí" o "este enlace" para hipervínculos

### Tono según contexto

| Contexto | Tono recomendado |
|---|---|
| Onboarding | Entusiasta, orientado al beneficio |
| Flujo normal (navegación, búsqueda) | Neutral, claro, eficiente |
| Éxito / confirmación | Positivo, breve |
| Error | Empático, orientado a la solución |
| Acción irreversible | Neutro, preciso, sin alarmar |
| Estado vacío | Alentador, con una acción clara |
| Notificación | Directo, relevante para el momento |

---

## Reglas operacionales

### Capitalización
- Títulos y subtítulos: primera letra mayúscula, resto minúscula (salvo nombres propios o siglas)
- Botones y labels: primera letra mayúscula únicamente

| ❌ Evitar | ✅ Usar |
|---|---|
| "Guardar Cambios" | "Guardar cambios" |
| "ver más" | "Ver más" |

### Botones y CTAs
Formato: **verbo + sustantivo**. Máximo 3 palabras. Describir la acción que ocurre al presionar.

| ❌ Evitar | ✅ Usar | Por qué |
|---|---|---|
| "Ir" | "Ver perfil" | Sin verbo claro |
| "Haz clic aquí" | "Descargar informe" | No describe la acción |
| "OK" | "Entendido" | Ambiguo |
| "Continuar" | "Guardar cambios" | No dice qué ocurre |
| "Sí" / "No" | "Eliminar cuenta" / "Cancelar" | Sin contexto |

### Hipervínculos
Insertar el link en texto descriptivo que indique el destino. Nunca en texto genérico.

- **Incorrecto:** "Para más información haz clic aquí."
- **Correcto:** [Ver términos y condiciones] (con link insertado)

### Puntuación
- Sin punto final en labels, botones, títulos y placeholders
- Con punto final en textos de más de una oración (descripciones, tooltips, errores)
- En español: signos de apertura (¡ ¿) obligatorios

### Placeholders en formularios
Mostrar un ejemplo del formato esperado, no repetir el label.

| ❌ Evitar | ✅ Usar |
|---|---|
| Placeholder: "Correo electrónico" (igual al label) | Placeholder: "nombre@ejemplo.com" |
| Placeholder: "Ingresa tu nombre" | Placeholder: "María García" |

---

## Mensajes de error

Estructura siempre: **qué pasó + qué hacer a continuación**. Sin tecnicismos. Sin culpar al usuario.

| ❌ Evitar | ✅ Usar |
|---|---|
| "Error 404" | "No encontramos esa página. Vuelve al inicio." |
| "Ha ocurrido un error inesperado." | "No pudimos guardar los cambios. Intenta de nuevo." |
| "Formulario inválido" | "Falta completar el correo electrónico." |
| "Sin conexión" | "Sin conexión a internet. Revisa tu red e intenta de nuevo." |
| "Contraseña incorrecta" | "El correo o la contraseña no coinciden. Inténtalo de nuevo." |

**Regla adicional:** Los errores de validación deben aparecer cerca del campo que los generó, no al final del formulario.

---

## Estados vacíos

Distinguir siempre entre dos casos, ya que el tono y la acción sugerida son distintos:

**Primera vez (nunca hubo datos):** Explicar qué verá el usuario cuando haya contenido y ofrecer una acción para empezar.
> "Aún no tienes favoritos guardados. Explora el mapa y guarda los lugares que te interesen."

**Sin resultados tras búsqueda o filtro:** Explicar por qué no hay resultados y ofrecer una salida.
> "No encontramos resultados con esos filtros. Prueba con otros criterios o amplía la búsqueda."

---

## Onboarding

- Una idea por pantalla
- Primero el beneficio para el usuario, luego la acción
- Evitar explicar cómo funciona la tecnología; explicar qué gana el usuario
- No pedir permisos sin explicar antes para qué se usan

**Estructura recomendada por pantalla:**
1. Beneficio principal (titular)
2. Explicación breve opcional (1 línea)
3. CTA claro

**Ejemplo genérico:**
> "Encuentra lo que necesitas en segundos."
> Busca por categoría, ubicación o nombre.
> [Empezar a explorar]

---

## Notificaciones

Estructura: **información clave primero + contexto breve + CTA si aplica**.

La información más importante debe aparecer al inicio, por si el mensaje se trunca.

| ❌ Evitar | ✅ Usar |
|---|---|
| "Hola, tenemos novedades para ti en la sección de ofertas disponibles." | "Nueva oferta disponible. Válida hasta el viernes." |
| "Tu pedido está siendo procesado por nuestro equipo." | "Pedido confirmado. Lo recibirás el jueves 12." |

---

## Confirmaciones de acciones destructivas

Cuando la acción no se puede deshacer, el texto debe ser preciso y neutral — sin alarmar, pero sin minimizar.

- El botón de confirmación debe describir exactamente la acción, no decir "Sí" o "Confirmar"
- El botón de cancelar debe ser siempre la opción visualmente menos prominente

**Ejemplo:**
> "¿Eliminar esta cuenta?"
> Esta acción no se puede deshacer. Perderás todos tus datos y configuraciones.
> [Eliminar cuenta] [Cancelar]

---

## Formularios

- Agrupar campos relacionados en secciones con título
- Los labels deben estar siempre visibles (no depender del placeholder como único indicador)
- El helper text previene errores antes de que ocurran; el error text los corrige después
- Indicar los campos opcionales, no los obligatorios (son minoría)

| Elemento | Función | Ejemplo |
|---|---|---|
| Label | Identifica el campo | "Correo electrónico" |
| Placeholder | Muestra el formato esperado | "nombre@ejemplo.com" |
| Helper text | Previene errores | "Usaremos este correo para enviarte el acceso." |
| Error text | Corrige errores | "El correo no tiene un formato válido." |

---

## Tooltips

- Usar solo cuando la información es realmente adicional, no para compensar un label confuso
- Texto breve: una oración máximo
- No repetir lo que ya dice el label o el helper text

---

## Checklist de revisión

Antes de entregar cualquier texto de interfaz:

- [ ] ¿El usuario entiende qué hace este elemento sin contexto adicional?
- [ ] ¿Los botones usan verbo + sustantivo?
- [ ] ¿Los hipervínculos están en texto descriptivo?
- [ ] ¿Los mensajes de error dicen qué pasó y qué hacer?
- [ ] ¿Los estados vacíos tienen una acción clara?
- [ ] ¿Capitalización correcta en todos los elementos?
- [ ] ¿Sin punto final en labels, botones y títulos cortos?
- [ ] ¿El tono es apropiado para el contexto emocional del usuario en ese momento?
- [ ] ¿La terminología es consistente con el resto de la interfaz?
- [ ] ¿Los placeholders muestran formato, no repiten el label?

---

## Adaptación por idioma

Al escribir en múltiples idiomas, mantener los principios pero adaptar las convenciones:

| Aspecto | Español | English | Português (BR) |
|---|---|---|---|
| Persona | Definir por proyecto (tú / usted / vos) | you (informal) | você |
| Signos de apertura | ¡ ¿ obligatorios | No aplica | No aplica |
| Formato de fecha | DD/MM/AAAA | MM/DD/YYYY | DD/MM/AAAA |
| Tono | Cálido, directo | Conversacional, conciso | Amigable, cercano |

Los principios de claridad, concisión y consistencia aplican en todos los idiomas por igual.
