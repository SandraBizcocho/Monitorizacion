🧠 Comandos de Monitorización de Tráfico de Red en Linux
# Tráfico de la red.

![Linux Badge](https://img.shields.io/badge/Linux-Terminal-black?logo=linux&logoColor=white)
![Bash Badge](https://img.shields.io/badge/Shell-Bash-blue?logo=gnu-bash)
![Monitoring Badge](https://img.shields.io/badge/Category-Monitoring-green)

🧭 Introducción

**Estos comandos permiten monitorizar el tráfico de red, ver la actividad de las interfaces, analizar paquetes y diagnosticar problemas de conectividad. Son herramientas fundamentales para administradores de sistemas y técnicos de redes.**

# 📋 1. `bmon`

Muestra el uso de **ancho de banda** en tiempo real por cada interfaz de red.  
🔍 Es muy visual y útil para detectar rápidamente picos de tráfico o interfaces con mayor carga.

📸 Captura:

![Ver imagen](img/bmon1.png)

---

# 📋 2. `iptraf`

Herramienta interactiva en modo texto para **monitorizar conexiones, tráfico por protocolo y estadísticas de red.**  
🔍 Permite observar la actividad en tiempo real de interfaces y puertos, mostrando bytes, paquetes y dirección origen/destino.

📸 Captura:

![Ver imagen](img/iptraf1.png)

---

# 📋 3. `tcpdump`

Analiza y captura **paquetes** que circulan por la red.  
🔍 Es ideal para diagnosticar problemas de red, verificar tráfico sospechoso o analizar protocolos.  
Se usa con permisos de superusuario y admite filtros potentes (por IP, puerto, protocolo, etc.).

📸 Captura:

![Ver imagen](img/tcpdump.png)

---

# 📋 4. `tcptrack`

Muestra las **conexiones TCP activas** en tiempo real junto con su velocidad de transferencia.  
🔍 Es muy útil para observar qué IPs están conectadas y cuántos datos están enviando o recibiendo.  

📸 Captura:

![Ver imagen](img/tcptrack1.png)
