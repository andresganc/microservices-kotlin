
## SOLUCION DE ERRORES COMUNES EN VISUAL STUDIO CODE PARA LINUX

### ERROR (Al ejecutar el codigo)

    - It’s hitting your system's file watchers limit
        "Visual Studio Code is unable to watch for file changes in this large workspace" (error ENOSPC)#

    
    - Está alcanzando el límite de observadores de archivos de su sistema
        "Visual Studio Code no puede observar los cambios de archivo en este gran espacio de trabajo" (error ENOSPC) #

    
    - SOLUCION

        - Ejecutar el siguiente comando en consola ruta: home - user: default 

        $ echo fs.inotify.max_user_watches=524288 | sudo tee -a /etc/sysctl.conf && sudo sysctl -p