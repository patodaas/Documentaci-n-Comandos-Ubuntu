## Patricio Dávila Assad 2089263
# Documentación Personal de Comandos en Terminal (Linux + Git)

Este documento resume mi recorrido personal aprendiendo comandos esenciales de la terminal de Ubuntu y Git. Están organizados de lo más básico a lo más avanzado dentro de mi propio nivel de uso.

---

##  **1. Comandos básicos de navegación y sistema**

### **`pwd`**
Muestra la ruta completa del directorio en el que estoy.
- **Ejemplo:** `pwd`

### **`cd`**
Sirve para moverme entre carpetas.
- **Ejemplo:** `cd Documentos`

### **`ls`**
Lista los archivos y carpetas en el directorio actual.
- **Ejemplo:** `ls`

### **`clear`**
Limpia la terminal para mantenerla ordenada.
- **Ejemplo:** `clear`

### **`whoami`**
Muestra el nombre del usuario actual.
- **Ejemplo:** `whoami`

---

##  **2. Comandos para crear, editar y gestionar archivos**

### **`echo`**
Imprime texto en la terminal o lo guarda en un archivo.
- **Ejemplo:** `echo "Hola"`

### **`nano`**
Editor de texto dentro de la terminal.
- **Ejemplo:** `nano archivo.txt`

### **`touch`** *(escrito antes como "rouch")*
Crea un archivo vacío.
- **Ejemplo:** `touch notas.txt`

### **`cat`**
Muestra el contenido de un archivo.
- **Ejemplo:** `cat archivo.txt`

### **`grep`**
Busca texto dentro de un archivo o salida.
- **Ejemplo:** `grep "error" log.txt`

### **`tree`**
Muestra la estructura de directorios en forma de árbol.
- **Ejemplo:** `tree`

---

##  **3. Comandos de manipulación de archivos y directorios**

### **`mkdir`**
Crea un directorio.
- **Ejemplo:** `mkdir proyectos`

### **`mv`**
Mueve o renombra archivos.
- **Ejemplo:** `mv archivo.txt carpeta/`

### **`rm`**
Elimina archivos.
- **Ejemplo:** `rm archivo.txt`

### **`chmod`**
Cambia los permisos de un archivo.
- **Ejemplo:** `chmod +x script.sh`

### **`./`** (Ejecutar un archivo)
Sirve para ejecutar archivos con permisos de ejecución.
- **Ejemplo:** `./script.sh`

---

##  **4. Comandos de administración del sistema**

### **`sudo`**
Ejecuta un comando con permisos de administrador.
- **Ejemplo:** `sudo nano /etc/hosts`

### **`apt install`**
Instala paquetes desde los repositorios.
- **Ejemplo:** `sudo apt install git`

### **`apt update`**
Actualiza la lista de paquetes disponibles.
- **Ejemplo:** `sudo apt update`

### **`apt upgrade`**
Actualiza los paquetes instalados a su última versión.
- **Ejemplo:** `sudo apt upgrade`

### **`ps`**
Muestra procesos activos.
- **Ejemplo:** `ps`

### **`kill`**
Termina un proceso usando su PID.
- **Ejemplo:** `kill 1234`

### **`man`**
Muestra el manual de un comando.
- **Ejemplo:** `man ls`

---

##  **5. Comandos esenciales de Git**

### **`git config --global user.name`**
Configura el nombre de usuario global de Git.
- **Ejemplo:** `git config --global user.name "Mi Nombre"`

### **`git config --global user.email`**
Configura el correo global de Git.
- **Ejemplo:** `git config --global user.email "correo@example.com"`

### **`git init`**
Inicializa un repositorio Git en una carpeta.
- **Ejemplo:** `git init`

### **`git add`**
Agrega archivos al área de *staging*.
- **Ejemplo:** `git add archivo.txt`
- **Todos los archivos:** `git add .`

### **`git commit -m "mensaje"`**
Guarda los cambios en el historial.
- **Ejemplo:** `git commit -m "Añadí el archivo inicial"`

### **`git push`**
Sube los commits a un repositorio remoto.
- **Ejemplo:** `git push`

### **`git push -u origin <rama>`**
Conecta la rama local con el remoto la primera vez.
- **Ejemplo:** `git push -u origin main`

### **`git pull`**
Descarga y aplica cambios del remoto.
- **Ejemplo:** `git pull`

---

##  **Conclusión personal**
Estos comandos representan mi recorrido aprendiendo a usar la terminal y Git. Empecé con tareas muy simples como navegar directorios y mostrar archivos, y poco a poco fui usando comandos más técnicos como `chmod`, procesos, paquetes del sistema y versiones con Git. Esta documentación refleja justo los que realmente he usado y entendido hasta ahora.

