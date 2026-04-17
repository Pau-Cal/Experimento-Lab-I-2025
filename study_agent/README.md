# Study Agent

Base inicial para construir un agente de estudio orientado a una maestría en ciencia de datos.

## Objetivo

Definir una estructura reutilizable para que el agente:

- explique teoría
- proponga ejercicios
- corrija respuestas
- resuma lecturas
- prepare exámenes
- recomiende rutas de estudio

## Estructura

- `prompts/system_prompt.md`: prompt base del tutor
- `config/agent_spec.json`: objetivo, alcance, roles y perfil pedagógico
- `config/curriculum_template.json`: plan curricular editable por materia
- `config/knowledge_and_logic.json`: capas de conocimiento y lógica de interacción
- `materials/glossary.md`: glosario inicial
- `materials/question_bank.json`: banco semilla de preguntas
- `materials/study_routes.json`: rutas de estudio por objetivo
- `memory/student_progress_template.json`: memoria del estudiante
- `evaluation/test_scenarios.json`: escenarios para probar e iterar el agente

## Cómo usar esta base

1. Editar `config/curriculum_template.json` con las materias reales de la maestría.
2. Cargar materiales propios del estudiante en la capa correspondiente.
3. Usar `prompts/system_prompt.md` como prompt del agente.
4. Persistir el estado del estudiante siguiendo `memory/student_progress_template.json`.
5. Ejecutar pruebas con los casos definidos en `evaluation/test_scenarios.json`.

## Alcance inicial

La implementación actual no reemplaza los notebooks existentes. Funciona como una base de contenidos y configuración para un tutor académico separado y extensible.
