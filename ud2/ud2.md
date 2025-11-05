🧠 Comandos de Monitorización de Recursos en Linux
# Memoria, espacio y rendimiento del disco.

![Linux Badge](https://img.shields.io/badge/Linux-Terminal-black?logo=linux&logoColor=white)
![Bash Badge](https://img.shields.io/badge/Shell-Bash-blue?logo=gnu-bash)
![Monitoring Badge](https://img.shields.io/badge/Category-Monitoring-green)




🧭 Introducción

Estos comandos permiten conocer el uso de recursos del sistema como CPU, memoria, disco y rendimiento general. Son muy útiles para la administración y diagnóstico del sistema Linux.

📋 1. atop

Muestra información detallada sobre procesos, uso de CPU, memoria, disco, red y más en tiempo real.
🔍 Es una herramienta avanzada de monitorización, similar a top pero con datos más completos y registro histórico.

📸 Captura:  

![Ver imagen](img/atop1.png)

---

📋 2. df

Muestra el espacio en disco disponible y usado en cada sistema de archivos montado.
🔍 Es ideal para comprobar cuánto espacio queda en las particiones o unidades montadas.

📸 Captura:  

![Ver imagen](img/df.png)

---

📋 3. du

Informa sobre el uso de espacio en disco por archivos y directorios.
🔍 Se usa frecuentemente con opciones como -h para mostrar tamaños en formato legible (KB, MB, GB).

📸 Captura:  

![Ver imagen](img/du.png)

---

📋 4. free

Muestra la memoria RAM y swap disponible y utilizada del sistema.
🔍 Ayuda a analizar el consumo de memoria y detectar si el sistema necesita más recursos.

📸 Captura:  

![Ver imagen](img/free.png)

---

📋 5. iostat

Permite ver estadísticas de entrada/salida de dispositivos, CPU y almacenamiento.
🔍 Es muy útil para detectar cuellos de botella en discos o rendimiento de CPU.

📸 Captura:  

![Ver imagen](img/iostat.png)
