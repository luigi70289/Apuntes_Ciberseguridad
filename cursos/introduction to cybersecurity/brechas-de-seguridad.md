# Brechas de seguridad: casos reales

Resumen de cuatro incidentes con su ataque, su impacto y cómo se podían prevenir. Consultado el 6 de noviembre de 2026.

| Incidente / fecha | Organización afectada | Qué se llevó o qué pasó | Ataque utilizado | Cómo prevenirlo | Fuentes |
|---|---|---|---|---|---|
| **Equifax**, mayo-julio de 2017 | Equifax, agencia de crédito de EE. UU. | Nombres, números de la Seguridad Social, fechas de nacimiento y direcciones de unos 147 millones de personas. También números de carné y de tarjeta. | Explotaron un fallo conocido de Apache Struts. Apache dijo que Equifax no había instalado la actualización a tiempo. | Aplicar los parches de seguridad pronto y vigilar la red para detectar intrusiones. | [1], [2] |
| **Target**, noviembre-diciembre de 2013 | Target, cadena de tiendas de EE. UU. | Unos 40 millones de números de tarjetas de pago. | Phishing a un contratista de aire acondicionado. Con sus credenciales entraron en la red y metieron malware en los terminales de pago. | Separar la red de proveedores de la de pagos (segmentación) y limitar el acceso de terceros. | [3], [4] |
| **Colonial Pipeline**, mayo de 2021 | Colonial Pipeline, oleoducto de EE. UU. | El oleoducto estuvo parado unos cinco días. Pagaron 4,4 millones de dólares de rescate y se recuperaron unos 2,3 millones. | Ransomware. Entraron con la contraseña filtrada de una cuenta VPN antigua que seguía activa y no tenía autenticación multifactor. | Activar MFA, cerrar las cuentas que ya no se usan y no reutilizar contraseñas. | [5], [6] |
| **MOVEit Transfer**, mayo de 2023 | Organizaciones que usaban MOVEit Transfer, de Progress Software. | Datos guardados en las bases de datos del programa. | El grupo CL0P explotó una inyección SQL (CVE-2023-34362) e instaló una web shell para sacar los datos. | Actualizar a la versión corregida, limitar las conexiones a IPs de confianza, activar MFA y revisar cuentas no autorizadas. | [7], [8], [9] |

## Fuentes

1. CNBC, 14 sep 2017: Equifax y la investigación de la FTC. https://www.cnbc.com/2017/09/14/equifax-tumbles-as-ftc-confirms-investigation-into-breach.html
2. Verus, 2022: acuerdo final de la FTC sobre la brecha de Equifax. https://verusllc.com/litigation-update-ftc-announces-settlement-finalization-on-2017-equifax-data-breach-claims
3. Bad Technology: Target, 40 millones de tarjetas a través de un contratista. https://bad.technology/articles/target-breach-40-million-cards-stolen-via-third-party-hvac-contractor.html
4. CEI: Cyber Security, Target's 2013 Data Breach. https://cei.com/about-cei/media-room/blog/cyber-security-targets-2013-data-breach
5. ManageEngine: The Colonial Pipeline hack uncovered. https://www.manageengine.com/blog/general/the-colonial-pipeline-hack-uncovered-fbi-and-cisa-recommended-security-measures.html
6. Bad Technology: Colonial Pipeline, cinco días sin combustible. https://bad.technology/articles/colonial-pipeline-ransomware-shuts-down-us-east-coast-fuel-supply-for-five-days.html
7. Industrial Cyber: aviso de CISA y el FBI sobre CL0P y MOVEit. https://industrialcyber.co/cisa/cisa-fbi-warn-organizations-that-cl0p-ransomware-group-exploits-moveit-transfer-vulnerability/
8. HealthITSecurity: Clop Ransomware Gang Exploiting MOVEit. https://healthitsecurity.com/news/clop-ransomware-gang-exploiting-moveit-cybersecurity-vulnerability
9. Fidelis Security: MOVEit, detalles y mitigaciones. https://fidelissecurity.com/?p=563
