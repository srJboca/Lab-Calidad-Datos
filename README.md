# Taller: Auditoría de Calidad y Gobierno de Datos en el Ecosistema SECOP

Este taller práctico tiene como objetivo aplicar conceptos de **Gobierno de Datos** y **Calidad de Información** utilizando datos reales de contratación pública en Colombia (SECOP II y SECOP Integrado). Los estudiantes asumirán el rol de auditores en la Agencia Nacional de Contratación Pública - Colombia Compra Eficiente.

## Objetivos de Aprendizaje
* Implementar el **Ciclo de Gestión de Calidad de Datos (PDCA)**: Planear, Hacer, Verificar y Actuar.
* Evaluar dimensiones críticas de calidad: Completitud, Exactitud, Consistencia, Actualidad y Trazabilidad.
* Utilizar modelos de auditoría forense como la **Ley de Benford** y el **Principio de Pareto** para detectar anomalías.
* Proponer políticas de **Gestión de Datos Maestros (MDM)** y roles de gobierno.

## Herramientas Requeridas
* **Databricks Community Edition**: Plataforma para el procesamiento de datos a escala.
* **PySpark / Spark SQL**: Motor de procesamiento distribuido para grandes volúmenes de datos.
* **Datasets de Datos Abiertos Colombia**:
    * SECOP II - Ofertas por Proceso
    * SECOP Integrado

## Conceptos Clave
El taller se fundamenta en las siguientes dimensiones de calidad de datos:
1. **Completitud (Comprehensiveness)**: ¿La información es suficiente?
2. **Exactitud (Accuracy)**: ¿Los datos reflejan la realidad correctamente?
3. **Consistencia (Consistency)**: ¿Los datos no se contradicen entre sistemas? (Auditado mediante el cruce de SECOP II e Integrado).
4. **Actualidad (Currency)**: ¿Los datos están vigentes y actualizados?
5. **Trazabilidad (Traceability)**: ¿Se puede conocer el origen de los datos?
6. **Corrección (Correctness)**: ¿Los datos están libres de errores de formato (ej. NITs con letras)?

## Estructura del Taller
El laboratorio está dividido en 5 fases críticas:
* **Fase 1: Ingestión y Perfilamiento**: Carga de datos reales mediante API y análisis de nulos.
* **Fase 2: Validez y Reglas de Negocio**: Aplicación de expresiones regulares (Regex) para validar identificadores (NIT).
* **Fase 3: Auditoría de Consistencia**: Cruce de fuentes para detectar discrepancias en nombres de proveedores y valores contractuales.
* **Fase 4: Modelos Estadísticos**: Aplicación de la Ley de Benford (primer dígito) y Pareto (concentración de gasto).
* **Fase 5: Informe de Gobierno**: Sustentación de decisiones estratégicas y asignación de roles.

## Instrucciones de Ejecución
1. Crear un nuevo Notebook en Databricks y copiar el código proporcionado celda a celda.
2. Configurar un clúster activo (Runtime recomendado 13.x o superior).
3. Ejecutar las celdas de forma secuencial.
4. Responder a los **Puntos de Decisión Estratégica** dentro de las celdas Markdown correspondientes.
5. Exportar el resultado final en formato HTML para su entrega.