# Threat Modeling with the PASTA Framework

## Descripción

Este proyecto documenta la aplicación del framework **PASTA (Process for Attack Simulation and Threat Analysis)** para realizar el modelado de amenazas de una aplicación móvil de compra y venta de zapatillas.

El objetivo es identificar amenazas, vulnerabilidades y riesgos antes del despliegue de la aplicación, permitiendo implementar controles de seguridad que reduzcan la superficie de ataque y fortalezcan la protección de los activos críticos.

---

# Objetivos del Proyecto

- Comprender el funcionamiento del framework PASTA.
- Analizar una aplicación desde la perspectiva de un analista de seguridad.
- Identificar los activos críticos del sistema.
- Analizar amenazas internas y externas.
- Detectar vulnerabilidades potenciales.
- Modelar posibles rutas de ataque.
- Proponer controles de seguridad para mitigar los riesgos.

---

# Escenario

Una empresa dedicada a la compra y venta de zapatillas desarrolló una aplicación móvil que permite:

- Registro de usuarios.
- Inicio de sesión.
- Compra y venta de productos.
- Mensajería entre compradores y vendedores.
- Calificación de vendedores.
- Procesamiento de pagos electrónicos.

Antes del lanzamiento de la aplicación, el equipo de seguridad realiza un proceso de **Threat Modeling** utilizando el framework **PASTA** para identificar riesgos de seguridad y fortalecer la aplicación antes de ponerla en producción.

---

# Tecnologías Analizadas

Durante el análisis se evaluaron las siguientes tecnologías:

- API (Application Programming Interface)
- Public Key Infrastructure (PKI)
- SHA-256
- Base de datos SQL

---

# Framework PASTA

El análisis sigue las siete etapas del framework:

1. Definir los objetivos del negocio.
2. Definir el alcance tecnológico.
3. Analizar el flujo de datos.
4. Identificar amenazas.
5. Analizar vulnerabilidades.
6. Modelar posibles ataques.
7. Analizar riesgos e implementar controles de seguridad.

---

# Principales Hallazgos

- La base de datos SQL representa uno de los activos más críticos de la aplicación.
- El flujo de datos permite identificar puntos donde un atacante podría interceptar o manipular información.
- Vulnerabilidades como SQL Injection pueden comprometer la confidencialidad, integridad y disponibilidad de los datos.
- El modelado de amenazas permite descubrir riesgos antes del despliegue de la aplicación.
- La implementación de controles preventivos reduce significativamente la superficie de ataque.

---

# Controles de Seguridad Recomendados

- Firewall correctamente configurado.
- Autenticación Multifactor (MFA).
- Validación de entradas.
- Prepared Statements para consultas SQL.
- IDS / IPS.
- Monitoreo continuo.
- Gestión de parches.
- Principio de mínimo privilegio.
- Cifrado de datos sensibles.
- Gestión segura de credenciales.

---

# Estructura del Proyecto

```text
threat-modeling-pasta-framework/
│
├── README.md
├── pasta-threat-model.md
├── risk-analysis.md
│
└── assets/
    ├── 01-project-overview.png
    ├── 02-data-flow.png
    ├── 03-attack-tree.png
    ├── 04-pasta-framework.png
    └── 05-executive-dashboard.png
```

---

# Recursos Visuales

## 1. Panorama General del Proyecto

![Project Overview](assets/01-project-overview.png)

---

## 2. Flujo de Datos de la Aplicación

![Data Flow](assets/02-data-flow.png)

---

## 3. Árbol de Ataque

![Attack Tree](assets/03-attack-tree.png)

---

## 4. Framework PASTA

![PASTA Framework](assets/04-pasta-framework.png)

---

## 5. Dashboard Ejecutivo del Análisis de Riesgos

![Executive Dashboard](assets/05-executive-dashboard.png)

---

# Conclusiones

El framework PASTA proporciona una metodología estructurada para identificar amenazas, analizar vulnerabilidades y evaluar riesgos durante el desarrollo de una aplicación.

Aplicar este proceso antes del despliegue permite fortalecer la seguridad desde el diseño, proteger los activos críticos de la organización y reducir significativamente la probabilidad de incidentes de ciberseguridad.

---

# Autor

Proyecto desarrollado como parte del estudio de **Threat Modeling** y **Application Security**, aplicando el framework **PASTA (Process for Attack Simulation and Threat Analysis)** sobre un caso práctico de análisis de riesgos en una aplicación móvil.
