# SIMAF

Sistema Integrado Municipal de Administración Financiera

## Descripción del Sistema

SIMAF es una plataforma web diseñada para municipalidades que
centraliza la gestión de ingresos, egresos y presupuesto en un solo
sistema. Permite mejorar la transparencia, trazabilidad y control
financiero mediante roles definidos y registros auditables.

## Problema que Resuelve

Las municipalidades suelen manejar procesos financieros en sistemas
separados o manualmente, lo que genera inconsistencias, retrasos en
reportes y poca trazabilidad. El sistema busca centralizar la
información financiera y facilitar la supervisión y auditoría.

## Usuarios y Stakeholders

-   Director Financiero Municipal
-   Encargado de Presupuesto
-   Contador Municipal
-   Auditor Municipal
-   Concejo Municipal

## Objetivos

-   Reducir errores contables.
-   Mejorar tiempos de generación de reportes.
-   Garantizar trazabilidad de transacciones.
-   Fortalecer la transparencia financiera.

## Alcance

-   Registro de ingresos municipales.
-   Registro de egresos.
-   Control de presupuesto por partidas.
-   Flujo de aprobación de egresos.
-   Reportes financieros.
-   Bitácora de auditoría.
-   Panel de control con ejecución presupuestaria.

## Fuera de Alcance

-   Cobro en línea para ciudadanos.
-   Gestión de nómina.
-   Sistema de compras públicas.
-   Integración bancaria en tiempo real.
-   Portal público de transparencia.

## Requerimientos Funcionales

-   FR-01: Registro de ingresos con detalles completos.
-   FR-02: Registro de solicitudes de egreso.
-   FR-03: Aprobación o rechazo de egresos.
-   FR-04: Visualización de saldo por partida.
-   FR-05: Consulta histórica para auditoría.
-   FR-06: Generación de reportes financieros.
-   FR-07: Registro de bitácora de acciones.

## Requerimientos No Funcionales

-   NFR-01: Soporte para múltiples usuarios concurrentes.
-   NFR-02: Tiempo de respuesta menor a 3 segundos.
-   NFR-03: Disponibilidad mensual del 99%.
-   NFR-04: Cifrado de datos en base de datos.
-   NFR-05: Respaldos automáticos diarios.

## Diagrama de Contexto

```mermaid
graph TD
    Director[Director Financiero Municipal]
    Presupuesto[Encargado de Presupuesto]
    Contador[Contador Municipal]
    Auditor[Auditor Municipal]
    
    Sistema[SIMAF-MUNI]
    
    Director -->|Aprueba egresos| Sistema
    Presupuesto -->|Gestiona partidas| Sistema
    Contador -->|Registra ingresos y egresos| Sistema
    Auditor -->|Consulta y audita| Sistema