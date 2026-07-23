# 🤖 UX Writing Prompt System

Sistema modular de **UX writing basado en prompts** diseñado para integrarse con LLMs (ChatGPT, Claude, etc.) y automatizar la generación de textos de interfaz de forma consistente.

---

## 📦 Arquitectura
.
├── ux-writing.md # Prompt workflow (entry point)
└── SKILL_generica.md # Knowledge base (rules + constraints)


---

## 🧠 Concepto

Este repo implementa un patrón de diseño común en sistemas con IA:

> **Workflow (orquestación) + Skill (contexto + reglas)**

- **Workflow →** controla la ejecución del prompt  
- **Skill →** define el comportamiento, tono y restricciones  

---

## 🔁 Flujo de ejecución
<img width="1024" height="1536" alt="ChatGPT Image 5 may 2026, 12_28_45 a m" src="https://github.com/user-attachments/assets/09b61eef-2332-4dc4-93f2-521f7330bc4c" />




## ⚙️ Uso
Entrada (prompt)
/ux-writing [elemento] [contexto]

# Ejemplos

/ux-writing botón para eliminar cuenta
/ux-writing error cuando falla el pago
/ux-writing onboarding app de finanzas


## 🧩 Diseño del sistema

# 1. Workflow Layer (ux-writing.md)

Responsabilidades:

- Parsear input
- Validar contexto mínimo
- Orquestar ejecución
- Aplicar lógica conversacional (preguntar si falta info)
- Esto funciona como un controller de prompts.

# 2. Skill Layer (SKILL_generica.md)

Responsabilidades:

- Definir reglas lingüísticas
- Establecer constraints
- Normalizar output
- Reducir variabilidad del modelo

Esto funciona como:

- System prompt persistente + guideline engine



## 🧱 Prompt Pattern

El sistema sigue este patrón:

- [INSTRUCTION]
Activar skill de UX writing

- [CONTEXT]
Elemento + situación del usuario

- [CONSTRAINTS]
Reglas de UX writing (claridad, tono, etc.)

- [OUTPUT]
Texto de interfaz


## 📏 Reglas clave (enforced constraints)

El modelo debe cumplir:

- CTAs → verbo + sustantivo
- Errores → qué pasó + qué hacer
- Máxima concisión
- Sin ambigüedad
- Sin lenguaje técnico innecesario
- Evitar "OK", "Click aquí", etc.

Esto reduce:

- Alucinaciones
- Verbosidad innecesaria
- Inconsistencias de tono

## 🧪 Ejemplo end-to-end

# Input
/ux-writing error login

# Resolución interna
- Elemento: error
- Contexto: login
- Skill: UX writing rules

" Output
El correo o la contraseña no coinciden. Inténtalo de nuevo.


## 🧬 Extensibilidad

Este sistema está pensado para escalar:

# Nuevas skills
/skills/
├── ux-writing
├── legal-writing
├── marketing-copy

# Multi-language support

La skill ya contempla:

- Español
- English
- Português

Se puede extender con:

- Localización automática
- Variantes regionales

# Integración con agentes

Este patrón funciona bien con:

- AI agents
- Chatbots
- Copilots de diseño
- Plugins de Figma / IDEs

## 🔌 Integración (ejemplo conceptual)
const runUxWriting = async (input) => {
  const skill = load("SKILL_generica.md")
  const workflow = load("ux-writing.md")

  return llm({
    system: skill,
    instruction: workflow,
    user: input
  })
}

## ✅ Ventajas

- Consistencia de copy a escala
- Reutilización de prompts
- Reducción de dependencia manual
- Mejora en calidad de UX writing
- Fácil de integrar en pipelines

⚠️ Consideraciones
- Requiere configuración de producto para mejores resultados. En este caso, se usó como base el Framework Baraldi -> https://github.com/leobaraldi96/fwbaraldi
- No reemplaza validación humana en casos críticos
- Depende de la calidad del contexto de entrada

## 🚀 Roadmap sugerido
 - Output estructurado (JSON para UI automation)
 - Testing de prompts (evals)
 - Versionado de skills
 - Integración con design tokens
 - Plugin para Figma

## 🧑‍💻 Autoría
Denisse Peduzzi
Content Designer - AI Product Designer
