# Análisis de Riesgos de la Aplicación

## Resumen

Como parte del proceso de modelado de amenazas utilizando el framework PASTA, se realizó un análisis de riesgos para identificar los activos críticos de la aplicación, las amenazas potenciales, las vulnerabilidades existentes y los controles de seguridad recomendados.

El objetivo es reducir la probabilidad de incidentes de seguridad antes del lanzamiento de la aplicación móvil.

---

# Activos Críticos

Los activos identificados durante el análisis son:

- Información de los usuarios.
- Credenciales de acceso.
- Base de datos SQL.
- Información de pagos.
- API de la aplicación.
- Sistema de mensajería.
- Inventario de productos.
- Infraestructura de la aplicación.

---

# Amenazas Identificadas

## Amenazas Externas

- Atacantes que buscan acceder a información confidencial.
- Bots automatizados.
- Ataques de fuerza bruta.
- SQL Injection.
- Robo de credenciales.
- Denegación de servicio (DoS).

---

## Amenazas Internas

- Uso indebido de privilegios.
- Acceso no autorizado por empleados.
- Divulgación de información confidencial.
- Errores humanos durante la administración del sistema.

---

# Vulnerabilidades Detectadas

Durante el análisis se identificaron las siguientes vulnerabilidades potenciales:

- Consultas SQL vulnerables.
- Validación insuficiente de entradas.
- Configuración incorrecta de permisos.
- APIs con controles de autenticación insuficientes.
- Contraseñas débiles.
- Configuración insegura del servidor.

---

# Evaluación del Riesgo

| Riesgo | Impacto | Probabilidad | Nivel |
|---------|---------|--------------|-------|
| SQL Injection | Alto | Alto | Crítico |
| Robo de credenciales | Alto | Medio | Alto |
| Acceso indebido a la API | Alto | Medio | Alto |
| Exposición de datos personales | Muy Alto | Medio | Crítico |
| Errores de configuración | Medio | Alto | Alto |

---

# Controles de Seguridad Recomendados

Se recomienda implementar los siguientes controles:

- Firewall correctamente configurado.
- Autenticación Multifactor (MFA).
- Validación de entradas.
- Prepared Statements para consultas SQL.
- IDS/IPS.
- Monitoreo continuo.
- Cifrado mediante AES y RSA.
- Hash seguro mediante SHA-256.
- Gestión de parches.
- Principio de mínimo privilegio.
- Registro y monitoreo de eventos.
- Auditorías periódicas de seguridad.

---

# Prioridad de Implementación

## Prioridad Alta

- Protección de la base de datos.
- Seguridad de la API.
- Implementación de MFA.
- Validación de entradas.

---

## Prioridad Media

- Monitoreo continuo.
- Revisión de configuraciones.
- Capacitación del personal.

---

## Prioridad Baja

- Optimización de procesos internos.
- Revisión periódica de documentación.
- Mejoras continuas.

---

# Recomendaciones

Para reducir la superficie de ataque de la aplicación se recomienda:

- Implementar controles de seguridad desde las primeras etapas del desarrollo.
- Aplicar el principio de mínimo privilegio.
- Realizar pruebas periódicas de seguridad.
- Mantener actualizados los componentes de software.
- Supervisar continuamente la infraestructura.
- Revisar regularmente las configuraciones del firewall y de la base de datos.

---

# Conclusiones

El análisis de riesgos permitió identificar que la base de datos y la información de los usuarios representan los activos más valiosos de la aplicación.

La aplicación del framework PASTA facilitó la identificación de amenazas, vulnerabilidades y controles preventivos antes del despliegue del sistema, reduciendo significativamente el riesgo de incidentes de seguridad.
