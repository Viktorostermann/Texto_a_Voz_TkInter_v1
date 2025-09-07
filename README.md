# Texto a Voz

Aplicación portable para convertir texto a voz con interfaz gráfica utilizando TkInter desarrollado en Python 3.10v.
La idea del proyecto es convertir un articulo existente en algun archivo de audio reproducible en formato mp3.

El audio sera extraido luego de pasar una direccion (URL) en el campo correspondiente dentro de la interfaz. Para realizar pruebas usamos URL: 
- "Nasa": https://www.npr.org/
- "BBC": https://www.bbc.com/
- "CNN": https://edition.cnn.com/
- "Nature": https://www.nature.com/
- "Reuters": https://www.reuters.com/
- "TechCrunch": https://techcrunch.com/
- "NationalGeographic" : https://www.nationalgeographic.com/
- "ScientificAmerican": https://www.scientificamerican.com/.

Asi mismo. Fueron utilizadas las bibliotecas del entorno de Python como: newspaper3k, pyttsx3 y gtts principales para el proyecto, entre otras.
tambien se espera que al encontrar el audio o articulo en audio mp3, se reproduzca y se genere el texto del mismo. Desarrollo inicial (Beta) entorno Windows.
Nueva version (V1.1) Compilada para entorno Linux Ubuntu 24.04.3 LTS / noble.

## VERSION PARA WINDOWS 10/11

## 🧩 Características

- Interfaz gráfica con TkInter
- Conversión de texto a voz con `pyttsx3`
- Ejecutable portable compilado con PyInstaller
- Firma digital trazada (certificado local, no incluido)
- Empaquetado con Inno Setup
- Estructura modular y defensiva
- Genera Logs, reportes HTML y TXT
- Almacena en su directorio los audios encontrados en articulos

## 📦 Ejecutable 

- El archivo compilado se encuentra en: https://drive.google.com/file/d/1Bh4p5DWDmux15vUM5iXSc0uxdosDbwXW/view?usp=sharing
  
## 🧩 Otros recursos.
HTML con algunos recursos declarados, utilizados para el desarrollo de Texto_a_Voz_v1: https://drive.google.com/file/d/1RwOCQ_C9ui_5OZPt9HNoWX7yFd1falgt/view?usp=sharing

> ⚠️ Los certificados `.pfx` no están incluidos por seguridad.

## 📄 Licencia

Este proyecto se publica bajo la licencia MIT.

## 🧾 ¿Qué permite la licencia MIT?

1. **Usar** el software para cualquier propósito, incluso comercial.  
2. **Copiar y modificar** el código sin restricciones.  
3. **Distribuir** el software, ya sea original o modificado.  
4. **Sub-licenciar o vender** el software como parte de otro producto.  

## ⚠️ ¿Qué condiciones impone?

1. Debes **mantener el aviso de derechos de autor** y el texto de la licencia original en todas las copias o versiones modificadas.  
2. El software se ofrece **“tal cual”**, sin garantías. El autor no se responsabiliza por errores, daños o mal funcionamiento.  

## 🧠 ¿Por qué es tan popular?

1. Es **compatible con otras licencias**, incluso con licencias más restrictivas como la GPL.  
2. Su **simplicidad** facilita el uso en proyectos personales, comerciales y colaborativos.  


## VERSION PARA LINUX UBUNTU 24.04

## 🧩 Características:

- Compilacion en 
- Entrada: texto manual y fuentes web compatibles.
- Salida: audios en Reportes/Audios_URLS/, logs en Reportes/Logs_GUI/.
- Experiencia visual: ícono y branding integrados.
- Trazabilidad: estructura de reportes organizada para auditoría.
- Requisitos previos
- Sistema: Debian/Ubuntu o derivadas.
- Dependencias de audio: libasound2, libglib2.0-0, libgomp1 (según entorno).
- GPG: requerido para verificar la firma digital.

## 📦 Instalador o Lanzador:

## Instalador: https://drive.google.com/file/d/17AltDD8rnXDVB9546bKmNmn1x50QoCg6/view?usp=sharing

Ejecución y lanzador:

Terminal: Texto_a_Voz_TkInter_v1

Interfaz gráfica: abre el menú de aplicaciones y busca “Texto a Voz (Tkinter)”.

## Instalación:

Instalar desde paquete .deb

1- Instalar paquete: sudo dpkg -i Texto_a_Voz_TkInter_v1_DEB.deb || sudo apt -f install -y

2- Verificaciones útiles:
- Binario: /usr/local/bin/Texto_a_Voz_TkInter_v1
- App: /opt/Texto_a_Voz_TkInter_v1/
- Ícono: /usr/share/icons/nouki.png
- Lanzador: /usr/share/applications/Texto_a_Voz_TkInter_v1.desktop

## Instalación remota con script

1- Permisos de ejecución: chmod +x instalar_remoto.sh
2- Ejecutar: ./instalar_remoto.sh

## Acciones: verifica firma con GPG, instala el .deb, resuelve dependencias y registra lanzador/ícono.

1- Uso de scripts .sh: instalar_remoto.sh

* Propósito: automatizar verificación e instalación.

2- Uso: ./instalar_remoto.sh

## Acciones típicas: gpg --verify, dpkg -i, apt -f install, registro de lanzador e ícono.


## 📁 Estructura de Instalador:

Texto_a_Voz_TkInter_v1_DEB/
├── DEBIAN/
│   ├── control
│   ├── postinst
│   └── postrm
├── opt/Texto_a_Voz_TkInter_v1/ ← recursos y ejecutable
├── usr/share/applications/ ← lanzador
├── usr/share/icons/ ← ícono

## 📁 Estructura de Archivos para distribución :

Distribucion_Verificada/
├── Texto_a_Voz_TkInter_v1_DEB.deb
├── Texto_a_Voz_TkInter_v1_DEB.deb.sig
├── viktore_public.asc
├── instalar_remoto.sh
├── desinstalar.sh
├── README_verificacion.txt
├── Captura_2025-09-07_12-59-18.png

## 📦 Desinstalar:

Desinstalación

1- Script dedicado: chmod +x desinstalar.sh
./desinstalar.sh

2- Alternativa con dpkg/apt: sudo dpkg -r texto-a-voz-tkinter-v1 || sudo apt remove -y texto-a-voz-tkinter-v1

## Nota: el nombre exacto del paquete depende del archivo DEBIAN/control de tu .deb.

1- desinstalar.sh: Propósito: desinstalar el paquete y limpiar recursos opcionales.
2- Uso: ./desinstalar.sh

## Ejecución y lanzador

Terminal: Texto_a_Voz_TkInter_v1

- Interfaz gráfica: abre el menú de aplicaciones y busca “Texto a Voz (Tkinter)”.

## Solución de problemas

- Firma inválida: reimporta la clave pública y verifica fecha de archivos.
- Dependencias faltantes: sudo apt -f install -y tras la instalación.
- Audio: confirma libasound2 y ejecuta desde terminal para ver logs.
- Ícono: refresca la caché o relanza la sesión si el ícono no aparece de inmediato.

## 🧾 Documentación y README para el usuario final

cluye:
- Objetivo del software
- Verificación de firma
- Instalación paso a paso
- Uso de scripts
- Desinstalación
- Ejecución desde terminal o lanzador

## README.MD: https://drive.google.com/file/d/1x1dOIuXVABJBr6zaxFR4qlCESvB86S16/view?usp=sharing
## DOC.HTML:  https://drive.google.com/file/d/12nWunGY6ljULYLBsAxwZ9I7mGdf9tO1w/view?usp=sharing

→ Si lo descargastes y te gusto el Proyecto... Dejame tu comentario y si quieres charlar sobre el tema tomemos un café!



