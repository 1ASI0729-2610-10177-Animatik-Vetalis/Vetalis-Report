﻿# Capítulo II: Requirements Elicitation & Analysis

---

## 2.1. Competidores

---
**GVET**<br> GVET es una plataforma integral "todo en uno" diseñada para la gestión clínica y administrativa de centros veterinarios en Latinoamérica. Su fortaleza radica en la **sincronización en tiempo real** entre el área médica y la administrativa: permite a los veterinarios gestionar historias clínicas detalladas mientras el sistema automatiza el control de stock y las comisiones por médico. Sin embargo, aunque es muy robusto en la gestión operativa, su interfaz puede resultar compleja para usuarios nuevos y la profundidad de sus reportes financieros avanzados suele estar reservada para planes de alto costo, lo que limita el acceso a analítica de datos en clínicas pequeñas.

**QVET**<br> QVET es uno de los softwares de gestión veterinaria más consolidados a nivel global, enfocado en la **estandarización de procesos y contabilidad**. Se destaca por su potente módulo de ERP, que permite una gestión exhaustiva de ingresos y egresos, auditorías de inventario y facturación electrónica integrada. Su principal ventaja es la solidez en la administración de grandes centros hospitalarios; no obstante, su arquitectura se siente menos ágil que las soluciones nativas en la nube más modernas, y su enfoque está tan volcado a la administración que la experiencia de usuario para el médico veterinario en consulta suele ser menos intuitiva.

**Wakyma Vets**<br> Wakyma es una solución *cloud-native* moderna que pone el foco en la **experiencia de usuario (UX) y la fidelización del cliente**. Su fortaleza reside en un dashboard administrativo simplificado que prioriza la visibilidad de la rentabilidad diaria y la automatización de recordatorios de pago y citas mediante canales digitales. Es ideal para clínicas que buscan digitalización rápida con una curva de aprendizaje mínima. Por el contrario, su capacidad de personalización en el control de inventarios críticos (insumos médicos específicos) es menor comparada con sistemas más robustos, y su enfoque es más comercial que puramente médico-hospitalario.
### 2.1.1. Análisis competitivo
#### Competitive Analysis Landscape

| **Título del Análisis** | **Competitive Analysis Landscape**                                                                                                                                                                                                                                                           |
| :--- |:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **¿Por qué llevar a cabo este análisis?** | Identificar brechas operativas y financieras en las soluciones actuales para posicionar a Vetalis como el ERP/EHR líder en trazabilidad de insumos y gestión de rentabilidad real en el mercado peruano. <br><br> Comparación por criterios estratégicos, operativos y de modelo de negocio. |
<br>

| **Categoría** | **Criterio** | <div align="center"><img src="../assets/vetalis_logo.png" alt="Vetalis" width="60"><br>**Nuestra Startup:<br>Vetalis**</div> | <div align="center"><img src="../assets/gvet_logo.png" alt="GVET" width="60"><br>**Competidor 1:<br>Gvet**</div> | <div align="center"><img src="../assets/qvet_logo.jpg" alt="QVET" width="60"><br>**Competidor 2:<br>qvet**</div> | <div align="center"><img src="../assets/wakyma_logo.png" alt="Wakyma" width="60"><br>**Competidor 3:<br>Wakyma Vets**</div> |
| :--- | :--- |:-----------------------------------------------------------------------------------------------------------------------------| :--- | :--- | :--- |
| **Perfil** | Overview | Plataforma SaaS integral (ERP/EHR) con enfoque en control de utilidades.                                                     | Ecosistema digital centrado en la experiencia de usuario y movilidad. | Software de larga trayectoria especializado en administración contable. | Solución cloud-native moderna enfocada en marketing y fidelización. |
| | Ventaja Competitiva | Trazabilidad exacta de insumos (gasto por cita) y dashboards de utilidad neta real.                                          | Integración fluida entre la app del dueño de mascota y el historial clínico. | Robustez contable absoluta y cumplimiento de normativas de auditoría complejas. | Automatización de la comunicación con el cliente y facilidad de uso (UX/UI). |
| **Perfil de <br> Marketing** | Mercado Objetivo | Clínicas veterinarias en crecimiento en Perú (Admin + Médicos).                                                              | Clínicas veterinarias medianas y grandes en Latinoamérica. | Hospitales veterinarios y cadenas con alta carga administrativa. | Veterinarias jóvenes que buscan digitalización rápida y comercial. |
| | Estrategias de <br> Marketing | Inbound marketing enfocado en eficiencia operativa y gestión financiera.                                                     | Presencia fuerte en redes sociales y alianzas con facultades de veterinaria. | Venta directa corporativa y presencia en congresos internacionales. | Marketing digital agresivo y periodos de prueba gratuitos (Freemium). |
| **Perfil de <br> Producto** | Productos & <br> Servicios | Gestión clínica (EHR), ERP financiero, inventario automático y pagos integrados.                                             | Gestión de citas, historia clínica, tienda online y app para propietarios. | ERP contable, facturación SUNAT, laboratorios y hospitalización. | Agenda digital, recordatorios automáticos, ficha médica y analítica. |
| | Precios & Costos | Modelo de suscripción mensual (SaaS) escalable por transacciones.                                                            | Suscripción por módulos con costos adicionales por usuarios/sedes. | Licenciamiento inicial más costo de mantenimiento anual elevado. | Suscripción mensual competitiva basada en pacientes activos. |
| | Canales de <br> Distribución | Plataforma Web (SaaS) responsiva.                                                                                            | Web y aplicación móvil nativa. | Software local con servicios en la nube e interfaz web. | Multiplataforma: Web, Android e iOS. |

<br>

### Análisis SWOT (FODA)

| Categoría | <div align="center"><img src="../assets/vetalis_logo.png" alt="Vetalis" width="40"><br>Vetalis</div> | <div align="center"><img src="../assets/gvet_logo.png" alt="GVET" width="40"><br>Gvet</div> | <div align="center"><img src="../assets/qvet_logo.jpg" alt="QVET" width="40"><br>qVet</div> | <div align="center"><img src="../assets/wakyma_logo.png" alt="Wakyma" width="40"><br>Wakyma Vets</div> |
| :--- |:-----------------------------------------------------------------------------------------------------| :--- | :--- | :--- |
| **Fortalezas** | Trazabilidad exacta de insumos y dashboards financieros simplificados.                               | Comunidad activa y excelente integración móvil. | Alta confiabilidad contable y cumplimiento legal. | Interfaz moderna y procesos de comunicación automatizados. |
| **Debilidades** | Producto nuevo en fase de desarrollo (menor historial de marca).                                     | Curva de aprendizaje técnica para el personal administrativo. | Interfaz antigua y procesos de configuración complejos. | Funcionalidades de inventario médico menos profundas. |
| **Oportunidades** | Crecimiento de la demanda de digitalización en veterinarias peruanas.                                | Expansión a servicios de telemedicina integrados. | Migración de clientes antiguos a sus nuevas versiones cloud. | Liderar el mercado de pequeñas clínicas con modelos low-cost. |
| **Amenazas** | Competidores establecidos con mayores presupuestos de marketing.                                     | Entrada de softwares genéricos de citas que bajen precios. | Nuevas normativas gubernamentales que exijan cambios. | Consolidación de otras plataformas de pagos competidoras. |
### 2.1.2. Estrategias y Tácticas frente a Competidores

| **Categoría** | **Estrategia** | **Táctica**                                                                                                                                                                                |
| :--- | :--- |:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Estrategias Ofensivas** | Diferenciación por precisión financiera (vs. GVET/Wakyma) | Implementar el módulo **"Gasto por Procedimiento"** para descontar insumos exactos (ml, unidades) en cada cita, calculando la utilidad neta real al instante.                              |
| | Modernización de la experiencia clínica (vs. QVET) | Diseñar una interfaz **"Single Page"** que permita al médico registrar la atención y el consumo de stock en una sola pantalla, eliminando la lentitud de los sistemas antiguos.            |
| **Estrategias Defensivas** | Localización y cumplimiento normativo (vs. Softwares Globales) | Integración nativa con **SUNAT** y pasarelas de pago locales (**Izipay/Niubiz**) para ofrecer una solución lista para el mercado peruano sin configuraciones externas.                     |
| | Reducción de barreras de entrada (vs. QVET) | Aplicar un modelo de **suscripción SaaS escalable** sin costo de licencia inicial, facilitando que clínicas pequeñas adopten la tecnología sin descapitalizarse.                           |
| **Estrategias de Crecimiento** | Marketing de autoridad financiera | Ejecutar una estrategia de **Inbound Marketing** basada en la rentabilidad, usando los Dashboards de Vetalis como gancho para atraer administradores preocupados por el control de costos. |
| | Retención por ecosistema integrado | Centralizar la facturación y los pagos dentro de la plataforma para generar una dependencia positiva basada en la **eficiencia operativa**, dificultando la migración a otros sistemas.    |
## 2.2. Entrevistas
***
### 2.2.1. Diseño de entrevistas

### 2.2.2. Registro de entrevistas
### 2.2.3. Análisis de entrevistas
## 2.3. Needfinding
***
### 2.3.1. User Personas
### 2.3.2. User Task Matrix
### 2.3.3. User Journey Mapping
### 2.3.4. Empathy Mapping
## 2.4. Big Picture EventStorming
***
## 2.5. Ubiquitous Language
***
