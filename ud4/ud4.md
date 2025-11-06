🧠 Comandos de Monitorización de Puertos en Linux
# Conexiones, puertos abiertos y resolución ARP

![Linux Badge](https://img.shields.io/badge/Linux-Terminal-black?logo=linux&logoColor=white)
![Bash Badge](https://img.shields.io/badge/Shell-Bash-blue?logo=gnu-bash)
![Monitoring Badge](https://img.shields.io/badge/Category-Monitoring-green)

🧭 Introducción

**Estos comandos permiten ver los puertos y conexiones activas, así como identificar equipos conectados en la red mediante tablas ARP o escaneos de puertos. Son muy útiles para la administración, auditoría y diagnóstico de redes.**

## 📋 1. `arp -a`

Muestra la **tabla ARP del sistema**, indicando las direcciones IP y MAC de los equipos conectados.  
🔍 Es útil para saber qué dispositivos están en la misma red local y si hay comunicación activa.

📸 Captura:

![Ver imagen](img/arp-a.png)

---

## 📋 2. `arp -n`

Muestra la tabla ARP sin resolver los nombres de host, es decir, mostrando directamente las IPs y direcciones MAC.  
🔍 Es más rápido que arp -a y se usa cuando no se desea realizar consultas DNS.

📸 Captura:

![Ver imagen](img/arp-n.png)

---

# 📋 3. `nmap`

Escanea los puertos abiertos de un equipo o red.  
🔍 Es una herramienta muy potente para auditar la seguridad, verificar servicios activos o comprobar el estado de un servidor.  
*Ejemplo:*
`sudo nmap -sS 192.168.1.0/24`

📸 Captura:

![Ver imagen](img/nmap.png)

---

# 📋 4. `ss -ntnp`

Muestra las conexiones TCP en escucha (LISTEN) con sus puertos, PID y procesos asociados.  
🔍 Es el reemplazo moderno de netstat, más rápido y preciso.

📸 Captura:

![Ver imagen](img/ss-ntnp.png)

---

# 📋 5. `ss -plunt`

Muestra todas las conexiones TCP y UDP, tanto en escucha como activas.  
🔍 Muy útil para obtener una visión completa de la actividad de red del sistema.

📸 Captura:

![Ver imagen](img/ss-plunt.png)
