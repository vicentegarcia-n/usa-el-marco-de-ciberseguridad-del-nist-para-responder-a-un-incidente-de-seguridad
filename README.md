# usa-el-marco-de-ciberseguridad-del-nist-para-responder-a-un-incidente-de-seguridad
Proyecto hecho en el curso #3 "Conexión y protección: Redes y seguridad de redes" del Certificado de Ciberseguridad de Google

### 🛡️ Usa el Marco de Ciberseguridad del NIST para responder a un incidente de seguridad

**Descripción:**  
Este proyecto consistió en la gestión y análisis de un ataque **DDoS de inundación ICMP** en una organización ficticia, aplicando el **Marco de Ciberseguridad del NIST (CSF)**. A través de sus cinco funciones clave (**Identificar, Proteger, Detectar, Responder y Recuperar**), se documentó la respuesta ante el incidente y se establecieron medidas preventivas para mitigar futuros ataques.

**📌 Escenario del incidente:**

- Un ataque DDoS basado en paquetes ICMP dejó **fuera de servicio** los recursos de red durante dos horas.
- El tráfico de red legítimo quedó bloqueado, afectando la operatividad de la empresa.
- Se activó un protocolo de respuesta de incidentes para restablecer los servicios críticos.

**🛠️ Aplicación del NIST CSF:**

1. **🔎 Identificar:**
   - Se reconoció que el ataque fue una inundación ICMP, afectando todos los servicios críticos.

2. **🛡️ Proteger:**
   - Se implementó una regla en el **firewall** para limitar la tasa de paquetes ICMP.
   - Se desplegó un **IDS/IPS** para filtrar tráfico sospechoso.

3. **📡 Detectar:**
   - Se habilitó la **verificación de IPs de origen** para detectar direcciones falsas en los paquetes ICMP.
   - Se utilizó software de **monitoreo de red** para identificar patrones de tráfico anómalos.

4. **🚨 Responder:**
   - Se aisló el tráfico malicioso en lugar de interrumpir toda la red.
   - Se analizaron registros de red para determinar el origen del ataque.
   - Se estableció un procedimiento de notificación a autoridades y partes interesadas.

5. **🔄 Recuperar:**
   - Se restauraron progresivamente los servicios críticos.
   - Se detuvieron servicios no esenciales para optimizar el rendimiento de la red.
   - Se establecieron nuevas políticas de mitigación contra DDoS.

**🛠️ Herramientas utilizadas:**

- **Firewall (iptables, Cisco ACLs, pfSense)**
- **Sistemas de detección y prevención de intrusos (IDS/IPS)**
- **Software de monitoreo de red (Wireshark, Snort, Zeek)**
- **Registros de eventos y logs de tráfico de red**

**📌 Aprendizajes clave:**

- La importancia de contar con un **plan de respuesta a incidentes** bien estructurado.
- Cómo aplicar el **NIST CSF** para gestionar ataques DDoS en tiempo real.
- La necesidad de **automatizar la detección de tráfico malicioso** con reglas de firewall y sistemas IDS/IPS.
