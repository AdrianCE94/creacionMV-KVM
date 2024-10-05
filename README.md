# creacionMV-KVM
apartado para ver como crear maquinas virtuales con KVM

![alt text](image.png)


# Index

- 1.Crear maquina con virt-manager
- 2.Crear maquina linea de comandos
- 3.Crear maquina linea de comandos con fichero xml
- 4.Modificar maquina


# 1. Crear maquina con virt-manager

Simplemente abrimos virt-manager y le damos a crear nueva maquina virtual, seguimos los pasos y ya tendremos nuestra maquina creada.De manera grafica es muy sencillo.

# 2. Crear maquina linea de comandos

Para crear una maquina virtual con la linea de comandos usaremos el comando virt-install, con la siguiente información:
    
    - Nombre de la maquina: --name
    - Tipo de virtualizacion: --virt-type kvm
    - ISO de instalación: --cdrom
    - Variante de la maquina: --os-variant (para saber las variantes disponibles usar el comando osinfo-query os)
    - Tamaño de la memoria RAM: --memory
    - Numero de CPUs: --vcpus
    - Tamaño del disco duro: --disk size (se creara con la imagen del disco duro en /var/lib/libvirt/images)