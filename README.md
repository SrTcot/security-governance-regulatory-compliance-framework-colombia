Security Governance & Regulatory Compliance Framework – Colombia

📌 Descripción General

Este repositorio consolida un marco integral de seguridad de la información, ciberseguridad, riesgo operativo, continuidad del negocio y cumplimiento normativo aplicable al sector financiero colombiano.
Está diseñado como referencia técnica para equipos de ingeniería, ciberseguridad, riesgo, cumplimiento y auditoría.

El contenido se alinea con lineamientos de la Superintendencia Financiera de Colombia (SFC), los estándares internacionales ISO, NIST, CIS, y principios de seguridad por diseño.




🎯 Objetivos del Repositorio

Establecer lineamientos formales para garantizar la Confidencialidad, Integridad y Disponibilidad (CIA) de la información.

Documentar las políticas y procedimientos internos exigidos por la regulación colombiana.

Guiar el diseño técnico de controles avanzados de ciberseguridad.

Proveer plantillas, matrices y artefactos necesarios para auditorías, certificaciones y operación continua.

Facilitar el cumplimiento con la normatividad vigente del sector financiero.





📚 Alcance

Este repositorio cubre:

Políticas de seguridad obligatorias y recomendadas.

Normatividad colombiana vigente para entidades vigiladas.

Arquitectura de seguridad, monitoreo, IAM y SSDLC.

Playbooks de respuesta a incidentes.

Riesgo operativo, continuidad del negocio y tercerización.

Integración entre estándares globales y regulación local.





🏛 Marco Regulatorio Colombiano

📘 Circular Externa 007 de 2018 – Seguridad de la Información y Ciberseguridad

Lineamientos para un Programa Integral de Ciberseguridad

Controles mínimos:

Gestión de identidades y accesos (IAM), MFA, privilegios mínimos.

Gestión de vulnerabilidades, SAST/DAST, pruebas de penetración.

Arquitectura segura: segmentación de red, hardening, cifrado.

Monitoreo continuo con SOC/SIEM, EDR/XDR.

Gestión de parches y configuración segura.

Seguridad en la nube bajo responsabilidad compartida.

Indicadores e informes a la Alta Dirección.


Obligaciones de reporte:

Reporte de incidentes al CSIRT Financiero.

Notificación a usuarios afectados cuando corresponda.

Participación en ejercicios de ciberseguridad coordinados por la SFC.





📘 SARLAFT 4.0 – Lavado de Activos y Financiación del Terrorismo

Incluye directrices sobre:

Gestión del riesgo LA/FT y perfilamiento del cliente.

Monitoreo transaccional en tiempo real.

Señales de alerta y analítica de comportamiento.

Reporte ROS.

Integración con controles antifraude y ciberseguridad.





📘 SARO – Riesgo Operativo

Requisitos:

Identificación, medición y control de riesgos operativos y tecnológicos.

Inclusión de ciberataques como escenarios de riesgo.

Matrices alineadas a ISO 31000 y COSO III.

Planes de continuidad basados en impacto.



---

📘 SARAS – Riesgos Ambientales y Sociales

(Obligatorio según Circular Externa 015 de 2025)

Identificación de riesgos ambientales, sociales y climáticos.

Análisis de materialidad.

Monitoreo y reporte a la SFC.

Integración en gobierno corporativo y modelos de riesgo.





📘 Protección al Consumidor Financiero

Requisitos:

Controles antifraude para canales digitales.

Mecanismos de autenticación robusta.

Monitorización transaccional avanzada.

Atención y respuesta ágil a incidentes que afecten a clientes.



---

🔐 Políticas Internas del Programa de Seguridad

1. Política de Seguridad de la Información (PSI)

Incluye gobierno corporativo, roles, clasificación de activos, CIA, cifrado, accesos, inventarios y retención.

2. Gestión de Identidades y Accesos (IAM)

Requisitos:

MFA obligatorio.

Principio de mínimo privilegio.

Rotación de credenciales.

Segregación de funciones (SoD).

Accesos privilegiados (PAM).


3. Seguridad en el Ciclo de Vida del Desarrollo (SSDLC)

Incluye:

SAST, DAST, SCA.

Controles en CI/CD.

Modelado de amenazas (STRIDE).

Revisión de código segura.

Vaults para secretos.


4. Continuidad del Negocio y Recuperación (BCP/DRP)

Elementos:

BIA.

RTO/RPO críticos.

Continuidad para incidentes cibernéticos.

Redundancia geográfica.

Planes de comunicación.


5. Monitoreo, Auditoría y Operación del SOC

SIEM con correlación avanzada.

Integración con EDR/XDR.

Alarmas obligatorias CE 007.

Reportes ejecutivos.

Retención de logs ≥ 12 meses.


6. Gestión de Proveedores y Tercerización

Evaluación de riesgo de terceros.

SLA y cláusulas de seguridad.

Auditorías continuas.

Cumplimiento de prácticas cloud seguras.


7. Gestión de Incidentes de Seguridad (CSIRT)

Incluye:

Procesos NIST 800-61.

Playbooks: ransomware, DDoS, phishing, fuga de datos, fraude.

Reporte al CSIRT Financiero.





🗂 Arquitectura del Repositorio

/docs
   /01-politicas
      seguridad-informacion.md
      iam.md
      continuidad-negocio.md
      sdlc-seguro.md
      terceros.md
      monitoreo-soc.md
      gestion-incidentes.md
      sarlaft.md
      saras.md

   /02-regulacion-colombia
      circular-007-2018.md
      circular-015-2025.md
      sarlaft-capitulo-iv.md
      saro-lineamientos.md
      proteccion-consumidor.md

   /03-procedimientos
      onboarding-seguridad.md
      playbooks/
         ransomware.md
         phishing.md
         fuga-datos.md
         ddos.md
         fraude-digital.md

   /04-plantillas
      risk-assessment.md
      incident-report.md
      bcp-template.md
      sdlc-checklist.md
      proveedores-checklist.md

README.md




⚙️ Crosswalk Técnico – Estándares vs Normativa SFC

Área	Estándar	Regulación SFC	Alineación

Seguridad	ISO 27001	Circular 007	Alta
Ciberseguridad	NIST CSF	Circular 007	Alta
Desarrollo Seguro	OWASP, NIST 800-218	Circular 007	Alta
Continuidad	ISO 22301	Requerimientos BCP SFC	Alta
Riesgo Operativo	ISO 31000	SARO	Alta
Riesgo LA/FT	–	SARLAFT 4.0	Obligatoria
ESG/Clima	TCFD	SARAS (CE 015/2025)	Alta





🛠 Requerimientos Técnicos Mínimos

Infraestructura

Zero Trust Architecture.

Segmentación de red.

Hardening basado en CIS.

WAF obligatorio.

TLS 1.3 en todos los canales.


Desarrollo

Firmas digitales en commits.

Pipelines con escaneo automático.

Vault para secretos.


Operación

EDR/XDR en endpoints críticos.

Logs centralizados.

Respuesta automatizada a alertas críticas.





🤝 Contribuciones

Las contribuciones deben cumplir con:

Normatividad colombiana aplicable.

Buenas prácticas de ingeniería.

Estándares internacionales de seguridad.

Validación técnica antes de aprobación.





📄 Licencia

MIT License
