🧠 Comandos de Monitorización de Recursos en Linux
# 💾 Memoria, espacio y rendimiento del disco.

![Linux Badge](https://img.shields.io/badge/Linux-Terminal-black?logo=linux&logoColor=white)
![Bash Badge](https://img.shields.io/badge/Shell-Bash-blue?logo=gnu-bash)
![Monitoring Badge](https://img.shields.io/badge/Category-Monitoring-green)

🧭 Introducción

**Estos comandos permiten analizar y monitorizar el tráfico de red en tiempo real, detectar cuellos de botella y observar la actividad de las interfaces de red. Son muy útiles para la administración y diagnóstico del sistema Linux. 🐧**

## 📋 1. `atop`

Muestra **información detallada** sobre procesos, uso de CPU, memoria, disco, red y más en tiempo real.  
🔍 Es más completo que top y htop, e incluso permite registro histórico, lo que facilita analizar problemas ocurridos en el pasado.

💡 Muy usado en servidores críticos.

📸 Captura:  

![Ver imagen](img/atop1.png)

---

## 📋 2. `df`
Muestra el **espacio en disco disponible y usado** en cada sistema de archivos montado.  
🔍 Opciones:

df -h → Muestra el tamaño de las particiones en formato legible (GB, MB, etc.).
✔ Hace que los valores se entiendan mejor.

df -hT → Igual que -h pero además muestra el tipo de sistema de archivos (ext4, xfs, tmpfs, etc.).
✔ Muy útil para identificar qué tipo de partición estás analizando.

💡 Es perfecto para comprobar si el disco se está llenando y evitar fallos del sistema.

📸 Captura:  

![Ver imagen](img/df.png)

---

## 📋 3. `du`
Informa sobre el uso de espacio en disco por archivos y directorios.  
🔍 Opciones más frecuentes:

du -hs → Muestra el tamaño TOTAL de la carpeta donde estás.  
-h → Muestra los tamaños en formato legible (KB, MB, GB).  
-s → Resume, muestra solo el total del directorio actual, sin listar subdirectorios. 

du -hs /home → Muestra solo el tamaño total de la carpeta /home.

du -hs /home/* → Muestra el tamaño de cada subcarpeta dentro de /home.  
✔ Ideal para saber qué usuario o carpeta está ocupando más espacio.

💡 Ideal para localizar carpetas grandes y liberar espacio rápidamente.

📸 Captura:  

![Ver imagen](img/du.png)

---

## 📋 4. `free`
Muestra la memoria RAM y swap disponible y utilizada del sistema.  Ayuda a analizar el consumo de memoria y detectar si el sistema necesita más recursos.

🔍 Opciones:  
-h → “Human readable”, muestra los valores en MB y GB, mucho más fácil de leer. 💡 Es la opción más usada en administración de sistemas.  
-s 3 → "s" de seconds (segundos). 💡 Ideal para monitorear cómo cambia la RAM durante una instalación, copia de archivos, ejecución de programas, etc.  
-c 3 → “count”, número de actualizaciones. 💡 Perfecto para obtener una pequeña muestra automática sin usar un bucle.

📸 Captura:  

![Ver imagen](img/free.png)

---

## 📋 5. `iostat`
Permite ver estadísticas de:  
📀 Discos y dispositivos de almacenamiento  
⚙️ Operaciones de entrada/salida (I/O)  
🧠 Carga de CPU
🔍 Es muy útil para detectar cuellos de botella en discos o rendimiento de CPU.

💡 Ideal para una consulta rápida del rendimiento general.

📸 Captura:  

![Ver imagen](img/iostat.png)


## [Unidad 3. Tráfico de la red](../ud3/ud3.md)
