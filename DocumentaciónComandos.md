## Patricio Dávila Assad 2089263
# Documentación Personal de Comandos en Terminal (Linux + Git)

A continuación presento cada comando con **entrada y salida realista simulada**, como si estuviera usándolo directamente en la terminal.

---

## 1. Navegación y sistema

### **pwd**
Muestra la ruta completa del directorio donde estoy.

**Entrada:**
```
$ pwd
```
**Salida:**
```
/home/usuario/proyectos
```

---
### **cd**
Sirve para moverme entre carpetas.

**Entrada:**
```
$ pwd
/home/usuario/proyectos/carpeta1
$ cd ..
$ pwd
```
**Salida:**
```
/home/usuario/proyectos
```

---
### **ls**
Lista archivos y carpetas.

**Entrada:**
```
$ ls
```
**Salida:**
```
archivo.txt  carpeta2  notas.md
```

---
### **clear**
Limpia la pantalla.

**Entrada:**
```
$ clear
```
**Salida:** *(la terminal se limpia)*

---
### **whoami**
Muestra el usuario actual.

**Entrada:**
```
$ whoami
```
**Salida:**
```
usuario
```

---

## 2. Creación, lectura y búsqueda de archivos

### **echo**
Imprime texto o lo manda a un archivo.

**Entrada:**
```
$ echo "Hola mundo"
```
**Salida:**
```
Hola mundo
```

---
### **nano**
Abre el editor de texto.

**Entrada:**
```
$ nano notas.txt
```
**Salida:** *(se abre la interfaz de nano)*

---
### **touch**
Crea un archivo vacío.

**Entrada:**
```
$ touch nuevo.txt
$ ls
```
**Salida:**
```
archivo.txt  carpeta2  nuevo.txt  notas.md
```

---
### **cat**
Muestra contenido de un archivo.

**Entrada:**
```
$ cat notas.txt
```
**Salida:**
```
Recordatorio:
- Estudiar para el examen
- Practicar comandos de terminal
```

---
### **grep**
Busca coincidencias dentro de texto.

**Entrada:**
```
$ grep "error" log.txt
```
**Salida:**
```
13: error: archivo no encontrado
42: fatal error: permiso denegado
```

---
### **tree**
Muestra estructura de carpetas.

**Entrada:**
```
$ tree
```
**Salida:**
```
.
├── carpeta1
│   └── datos.txt
├── carpeta2
└── notas.md
```

---

## 3. Manipulación de archivos y permisos

### **mkdir**
Crea un directorio.

**Entrada:**
```
$ mkdir nuevo_proyecto
$ ls
```
**Salida:**
```
archivo.txt  carpeta1  carpeta2  nuevo_proyecto  notas.md
```

---
### **mv**
Mueve o renombra archivos.

**Entrada:**
```
$ mv archivo.txt carpeta2/
$ ls carpeta2
```
**Salida:**
```
archivo.txt
```

---
### **rm**
Elimina archivos.

**Entrada:**
```
$ rm nuevo.txt
$ ls
```
**Salida:**
```
archivo.txt  carpeta1  carpeta2  notas.md
```

---
### **chmod**
Cambia permisos.

**Entrada:**
```
$ chmod +x script.sh
$ ls -l script.sh
```
**Salida:**
```
-rwxr-xr-x 1 usuario usuario 120 feb  2 12:00 script.sh
```

---
### **./** (ejecutar archivo)

**Entrada:**
```
$ ./script.sh
```
**Salida:**
```
Script ejecutado correctamente
```

---

## 4. Administración del sistema

### **sudo**
Ejecuta comandos como administrador.

**Entrada:**
```
$ sudo nano /etc/hosts
```
**Salida:**
```
[sudo] password for usuario:
```
(luego abre nano)

---
### **apt install**
Instala paquetes.

**Entrada:**
```
$ sudo apt install git
```
**Salida:**
```
Leyendo lista de paquetes... Hecho
Construyendo árbol de dependencias
Leyendo la información de estado... Hecho
Se instalarán los siguientes paquetes nuevos:
  git
Descargando: 64% [##########........]
Instalando...
```

---
### **apt update**
Actualiza lista de paquetes.

**Entrada:**
```
$ sudo apt update
```
**Salida:**
```
Obteniendo:1 http://archive.ubuntu.com stable InRelease
Obteniendo:2 http://archive.ubuntu.com stable/main amd64 Packages
Leyendo lista de paquetes... Hecho
```

---
### **apt upgrade**
Actualiza los paquetes instalados.

**Entrada:**
```
$ sudo apt upgrade
```
**Salida:**
```
Calculando actualización... Hecho
Se actualizarán 5 paquetes.
Descargando: 57% [######........]
Instalando actualizaciones...
```

---
### **ps**
Muestra procesos activos.

**Entrada:**
```
$ ps
```
**Salida:**
```
  PID TTY          TIME CMD
 2134 pts/0    00:00:00 bash
 2457 pts/0    00:00:01 python3
 2601 pts/0    00:00:00 ps
```

---
### **kill**
Termina procesos.

**Entrada:**
```
$ kill 2457
$ ps
```
**Salida:**
```
  PID TTY          TIME CMD
 2134 pts/0    00:00:00 bash
 2601 pts/0    00:00:00 ps
```

---
### **man**
Abre el manual de un comando.

**Entrada:**
```
$ man ls
```
**Salida:** *(se abre el manual)*

---

## 5. Comandos de Git

### git config --global user.name
Configura el nombre de usuario global que Git usará en los commits.

**Entrada:**
```
$ git config --global user.name "Mi Nombre"
```

---
### git config --global user.email
Configura el correo global que Git usará en los commits.

**Entrada:**
```
$ git config --global user.email "correo@example.com"
```

---
### git init
Crea un repositorio Git vacío en la carpeta actual (inicializa el control de versiones).

**Entrada:**
```
$ git init
```
**Salida:**
```
Initialized empty Git repository in /home/usuario/proyecto/.git/
```

---
### git add
Añade archivos al área de "staging" para prepararlos antes del commit.

**Entrada:**
```
$ git add notas.md
```

---
### git commit -m "mensaje"
Crea un commit (registro) con los cambios que están en staging, usando el mensaje indicado.

**Entrada:**
```
$ git commit -m "Primer commit"
```
**Salida:**
```
[main 3a5f9c1] Primer commit
 1 file changed, 3 insertions(+)
```

---
### git push
Envía tus commits locales al repositorio remoto configurado (por ejemplo, origin).

**Entrada:**
```
$ git push
```
**Salida:**
```
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), done.
Pushed to origin
```

---
### git push -u origin main
Sube la rama local al remoto y configura el seguimiento entre la rama local y la rama remota.

**Entrada:**
```
$ git push -u origin main
```
**Salida:**
```
Branch 'main' set up to track remote branch 'main' from 'origin'.
```

---
### git pull
Descarga cambios desde el remoto y los fusiona automáticamente en la rama actual (fetch + merge o fast-forward).

**Entrada:**
```
$ git pull
```
**Salida:**
```
Updating 3a5f9c1..9bd4e21
Fast-forward
 archivo.txt | 2 ++
```

---

## Conclusión
He simulado entradas y salidas de los comandos incluidos en mi documentación, cuidando que sean ejemplos realistas y prácticos para un entorno Ubuntu. Empecé con comandos de navegación y manipulación de archivos (pwd, cd, ls, mkdir, mv, rm), pasé por gestión de permisos y ejecución (chmod, ./), administración del sistema (sudo, apt) y finalmente las operaciones básicas de Git para control de versiones (configurar usuario, init, add, commit, push, pull).

Este documento sirve como mi "recorrido personal" en la terminal: puedo usarlo como referencia rápida mientras practico y lo puedo expandir con más ejemplos, errores comunes o notas personales cuando lo necesite.

