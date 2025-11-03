# 🧠 TP Integrador - Computación Aplicada

## 👥 Integrantes del grupo
- Manuel Krivoy
- Marcelo Sica


## 🖥️ Descripción general

Este trabajo práctico tiene como objetivo la instalación, configuración y puesta en marcha de una infraestructura de servidor Linux (Debian) virtualizada en **VirtualBox**, integrando servicios de red, web y base de datos, junto con tareas automatizadas de backup y mecanismos de persistencia y compartición de datos con el sistema host.


## 📦 Entregables

En el repositorio se incluyen los siguientes archivos comprimidos:

| Directorio | Archivo generado |
|-------------|------------------|
| `/root` | `root_bkp.tar.gz` |
| `/etc` | `etc_bkp.tar.gz` |
| `/opt` | `opt_bkp.tar.gz` |
| `/www_dir` | `www_dir_bkp.tar.gz` |
| `/backup_dir` | `backup_dir_bkp.tar.gz` |
| `/var` | `var_part_aa`, `var_part_ab`, ... *(dividido en partes de hasta 24MB)* |



## 🗺️ Diagrama topológico de la infraestructura
Se incluyo un pequeño esquema (Topología.png) que detalle como funciona la infraestructura del sistema.

**Descripción del esquema:**
- El host Windows se conecta a la VM Debian mediante VirtualBox.  
- Apache2 atiende peticiones HTTP .  
- MariaDB ejecuta la base de datos localmente.  
- Se automatizan backups con cron hacia `/backup_dir`.  
- `/mnt/entregables` sincroniza con el host para transferir entregas.  
