# Modelado de Amenazas utilizando el Framework PASTA

## Introducción

El modelado de amenazas es una técnica utilizada para identificar riesgos de seguridad durante el desarrollo de una aplicación. Su objetivo es descubrir amenazas y vulnerabilidades antes de que la aplicación sea puesta en producción, permitiendo implementar controles de seguridad de forma preventiva.

En este proyecto se aplica el framework **PASTA (Process for Attack Simulation and Threat Analysis)** sobre una aplicación móvil destinada a la compra y venta de zapatillas deportivas.

---

# Escenario

La empresa desarrolló una aplicación móvil que permite:

- Registro de usuarios.
- Inicio de sesión.
- Compra y venta de zapatillas.
- Mensajería entre compradores y vendedores.
- Calificación de vendedores.
- Procesamiento de pagos electrónicos.

Debido a que la aplicación almacenará información personal y financiera, la organización decidió realizar un proceso de modelado de amenazas antes de su lanzamiento.

---

# Etapa I - Definir los Objetivos del Negocio

## Objetivos identificados

- Facilitar la compra y venta de zapatillas mediante una aplicación intuitiva.
- Proteger la información personal y financiera de los usuarios.
- Procesar pagos de forma segura cumpliendo los requisitos legales.

### Resultado

Se identificó que la disponibilidad del servicio, la privacidad de los datos y la seguridad de los pagos representan los objetivos más importantes para el negocio.

---

# Etapa II - Definir el Alcance Tecnológico

## Tecnologías utilizadas

- API
- PKI
- SHA-256
- SQL

### Tecnología priorizada

La base de datos SQL fue considerada el activo tecnológico más crítico porque almacena información confidencial como usuarios, productos, inventario, mensajes y registros de transacciones.

Una vulnerabilidad como SQL Injection podría comprometer la confidencialidad, integridad y disponibilidad de toda la información almacenada.

---

# Etapa III - Descomposición de la Aplicación

## Flujo de datos

Usuario

↓

Aplicación móvil

↓

API

↓

Base de datos SQL

↓

Resultados

↓

Usuario

### Análisis

El flujo de datos permitió identificar los puntos donde la información puede ser interceptada, modificada o consultada de forma no autorizada.

---

# Etapa IV - Análisis de Amenazas

## Amenazas externas

- Atacantes que buscan robar información personal y financiera.
- Bots automatizados que intentan explotar vulnerabilidades de la aplicación.

## Amenazas internas

- Empleados con privilegios que podrían abusar de su acceso.
- Uso indebido de información confidencial por parte de personal autorizado.

---

# Etapa V - Análisis de Vulnerabilidades

## Vulnerabilidades identificadas

- Consultas SQL vulnerables a ataques de SQL Injection.
- Validación insuficiente de las entradas proporcionadas por los usuarios.

### Riesgo

Estas debilidades podrían permitir el acceso, modificación o eliminación de información crítica almacenada en la base de datos.

---

# Etapa VI - Modelado del Ataque

## Objetivo del atacante

Obtener acceso no autorizado a la información de los usuarios.

## Posibles rutas de ataque

- Explotar una vulnerabilidad de SQL Injection.
- Comprometer cuentas mediante credenciales débiles.
- Aprovechar errores de validación de entradas.
- Acceder a información sensible utilizando permisos mal configurados.

---

# Etapa VII - Análisis de Riesgos y Controles

## Controles recomendados

- Firewall correctamente configurado.
- Autenticación Multifactor (MFA).
- Uso de Prepared Statements.
- Validación de entradas.
- IDS/IPS.
- Monitoreo continuo.
- Cifrado de datos sensibles.
- Gestión segura de credenciales.

---

# Conclusiones

El framework PASTA permitió identificar los activos críticos, comprender el flujo de datos de la aplicación, detectar amenazas y vulnerabilidades potenciales y proponer controles preventivos antes del despliegue de la aplicación.

Aplicar el modelado de amenazas durante el desarrollo fortalece la seguridad desde el diseño y reduce significativamente el riesgo de incidentes de ciberseguridad.
