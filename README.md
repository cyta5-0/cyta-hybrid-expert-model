# Modelo CyTA de Sistemas Expertos Híbridos  
### Inferencia determinística con generación de conocimiento asistida por IA

## Descripción general

El **Modelo CyTA de Sistemas Expertos Híbridos** es una arquitectura modular orientada al análisis formal de dominios específicos mediante reglas explícitas e inferencia determinística, integrando modelos de IA generativa exclusivamente para la redacción, contextualización y expresión del conocimiento previamente calculado.

El modelo ha sido desarrollado en el marco del proyecto **CyberCyTA** y está diseñado para garantizar:

- trazabilidad lógica,
- auditabilidad,
- reproducibilidad,
- separación epistemológica entre cálculo e interpretación,
- independencia tecnológica.

---

## Principios fundamentales

El modelo se apoya en los siguientes principios:

1. **Separación estricta de responsabilidades**
   - Entrada de datos
   - Inferencia lógica
   - Presentación de resultados
   - Generación discursiva asistida por IA

2. **Inferencia determinística**
   - Todos los cálculos, indicadores y reglas se resuelven fuera de la IA.
   - La IA no calcula, no decide ni introduce reglas.

3. **IA como sistema expresivo**
   - La IA recibe hechos, resultados y lógica aplicada.
   - Su rol es exclusivamente narrativo y contextual.

4. **Compatibilidad y sustentabilidad**
   - Compatible con PHP 5.6
   - Sin dependencias externas
   - Portable y reutilizable

---

## Arquitectura general

```text
Entrada de datos
        ↓
Normalización
        ↓
Inferencia lógica (motor de reglas)
        ↓
Resultados calculados
        ↓
Construcción de prompt estructurado
        ↓
IA generativa (redacción profesional)

## Organización del proyecto
/config
  ├── model_config.php     ← Conocimiento del dominio
  └── labels.php           ← Textos y etiquetas

/engine
  ├── input_loader.php     ← Normalización de datos
  ├── logic_engine.php     ← Inferencia y cálculos
  ├── prompt_builder.php   ← Construcción del prompt
  └── schema_metadata.php  ← Metadatos JSON-LD

/ui
  ├── form_view.php        ← Formulario de entrada
  ├── results_view.php     ← Visualización de resultados
  └── prompt_view.php      ← Prompt + acciones

index.php                  ← Orquestador del sistema

**Rol del archivo index.php**

* El archivo index.php actúa como orquestador del sistema, coordinando:  
* el flujo de ejecución,  
* la activación condicional del motor,  
* la integración entre UI, inferencia y generación asistida por IA.  
* No implementa lógica de dominio ni inferencia, sino control sistémico.

**Rol de la IA generativa**

La IA recibe un prompt estructurado que contiene:

* datos de entrada,  
* resultados calculados,  
* lógica aplicada,  
* contexto del análisis.  
* Su función es generar una redacción profesional, coherente y contextualizada.

**Ventajas del modelo**

* Transparencia lógica  
* Auditabilidad completa  
* Reproducibilidad del análisis  
* Escalabilidad por dominio  
* Integración semántica (Schema.org / RDFa)

**Uso responsable de IA generativa**

* Casos de uso  
* Análisis financiero y contable  
* Evaluación de indicadores  
* Diagnósticos basados en reglas  
* Sistemas de apoyo a la decisión  
* Curación académica asistida por IA

**Licencia**

Este proyecto se distribuye bajo una licencia abierta, acorde a los principios de acceso libre de CyTA
