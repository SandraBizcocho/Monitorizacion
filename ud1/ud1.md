🧠 Comandos de Monitorización de Procesos en Linux
# 🖥️ Procesos

![Linux Badge](https://img.shields.io/badge/Linux-Terminal-black?logo=linux&logoColor=white)
![Bash Badge](https://img.shields.io/badge/Shell-Bash-blue?logo=gnu-bash)
![Monitoring Badge](https://img.shields.io/badge/Category-Monitoring-green)

🧭 Introducción

Estos comandos permiten ver y controlar los procesos activos en Linux, ayudando a conocer el uso de CPU, memoria y usuarios que los ejecutan. Son esenciales para monitorizar el sistema.

## Lista de comandos:

🔗 [ps au](#-1-ps-au)

🔗 [ps aux](#-2-ps-aux)

🔗 [ps -u](#3-ps--u-alumno)

🔗 [top](#-4-top)

🔗 [top -b -n 3](#-5-top--b--n-3--topinfo)

🔗 [htop](#%EF%B8%8F-6-htop)

🔗 [ps -eo user](#-7-ps--eo-userpidcommcpu---sort-cpu--head--n-6)

---

## 📋 1. `ps au`
Muestra los **procesos activos** del usuario actual en un formato más detallado (sin procesos de otros usuarios).  

🔍 Opciones:  
a → Muestra los procesos de todos los usuarios que tienen una terminal activa.  
u → Usa un formato “user-oriented”, mostrando columnas como USER, PID, %CPU, %MEM, TTY, TIME y COMMAND.

💡 Es ideal para ver qué programas tienes en ejecución en tu sesión actual.

📸 **Captura:**  

![Ver imagen](img/psau.png)

[⬆️ Volver a la lista de comandos](#lista-de-comandos)

---

## 👥 2. `ps aux`
Lista **todos los procesos del sistema** incluyendo los de otros usuarios y los que no están asociados a una terminal (daemon o servicio).   

🔍 Opciones:  
a → Procesos de todos los usuarios.  
u → Muestra los procesos con formato detallado.  
x → Incluye procesos sin terminal asociada.

💡 Ideal para administradores que necesitan una visión completa del sistema.

📸 **Captura:**  

![Ver imagen](img/psaux.png)

[⬆️ Volver a la lista de comandos](#lista-de-comandos)

---

## 👩‍💻 3. `ps -u alumno`
Muestra solo los procesos que pertenecen al usuario **alumno** 👤.  

🔍 Opciones:  
-u [usuario] → Muestra únicamente los procesos del usuario indicado.

💡 Muy útil cuando hay varios usuarios en el sistema y quieres filtrar los procesos de un usuario específico.

📸 **Captura:**  

![Ver imagen](img/ps-u.png)

[⬆️ Volver a la lista de comandos](#lista-de-comandos)

---

## ⚡ 4. `top`
Muestra en **tiempo real** los procesos activos, el uso de CPU, memoria, carga del sistema y el tiempo que lleva encendido el equipo.  

📊 Características principales:  
Se actualiza automáticamente cada pocos segundos.  
Ordena los procesos por consumo de CPU o memoria.  
Permite finalizar procesos desde la propia interfaz (tecla k).  
Muestra estadísticas del sistema en la parte superior (load average, uptime, etc.).

💡 Es una de las herramientas más comunes para **monitorizar el rendimiento**.

📸 **Captura:**   

![Ver imagen](img/top.png)

[⬆️ Volver a la lista de comandos](#lista-de-comandos)

---

## 🧾 5. `top -b -n 3 > top.info`
Ejecuta `top` en **modo batch** (sin interfaz interactiva) y guarda **3 iteraciones** en el archivo `top.info`  

🔍 Opciones:  
-b → “Batch mode”: produce salida estándar, ideal para guardar en archivos o scripts.  
-n 3 → Indica que tome 3 actualizaciones y luego termine.  
'>' Redirige la salida al archivo top.info.

💡 Perfecto para registrar el rendimiento del sistema y analizarlo más tarde con cat o less.

📸 **Captura:**   

![Ver imagen](img/top-b.png)

[⬆️ Volver a la lista de comandos](#lista-de-comandos)

---

## 🖥️ 6. `htop`
Versión mejorada e interactiva de `top`, con una **interfaz gráfica en terminal más visual, colorida y fácil de usar** 🎨.  

✨ Ventajas sobre top:  
Muestra barras de colores para CPU, RAM y swap.  
Permite desplazarse con el teclado por la lista de procesos.  
Facilita matar procesos (F9) o cambiar su prioridad (F7/F8).  
Agrupa procesos en forma de árbol jerárquico.  

💡 Permite navegar, ordenar y finalizar procesos fácilmente con el teclado.

📸 **Captura:**  

![Ver imagen](img/htop.png)

[⬆️ Volver a la lista de comandos](#lista-de-comandos)

---

## 🔝 7. `ps -eo user,pid,comm,%cpu --sort=-%cpu | head -n 6`
Muestra los **5 procesos que más CPU consumen**, ordenados de mayor a menor 🔥.  

🔍 Opciones:  
-e → Muestra todos los procesos del sistema.  
-o → Permite definir qué columnas mostrar (user, pid, comm, %cpu).  
--sort=-%cpu → Ordena la salida por uso de CPU (el signo “-” indica orden descendente).  
| head -n 6 → Muestra solo las primeras 6 líneas (una de cabecera + 5 procesos).

💡 Ideal para detectar procesos que saturan la CPU y sobrecargan el sistema.

📸 **Captura:** 

![Ver imagen](img/ps-eo.png)

[⬆️ Volver a la lista de comandos](#lista-de-comandos)

## 🔗 [Documentación](../ud1/documentos/documento.md)
## 🔗 [Unidad 2. Memoria, espacio y rendimiento del disco](../ud2/ud2.md)
