# Práctica 2

## Table of Contents
- [Práctica 2](#práctica-2)
  - [Table of Contents](#table-of-contents)
  - [Objetivo](#objetivo)
  - [Procedimiento](#procedimiento)

---
## Objetivo
Crear y configurar dos máquinas virtuales en Azure.

---
## Procedimiento

1. Acceder al [portal de Azure](portal.azure.com) y buscar _"Máquinas virtuales"_.
2. Creamos la primer máquina virtual con el botón **Crear**.
3. En el campo **Nombre de máquina virtual** escribimos _Sesion4-vm1_ y automáticamente se creará el grupo de recursos.

4. En el campo **Suscripción** elegimos _Azure for students_.

5. En el campo **Región** elegimos la región _Australia Central_.
6. En el campo **Imagen** seleccionamos _Windows 10 Pro, versión 21H2 - Gen2_
7. En el campo **Cuenta de administrador** colocamos el nombre de usuario y contraseña para iniciar sesión en la máquina virtual.

8. En el campo **Seleccionar puertos de entrada** seleccionamos la opción _RDP_.

9. Finalmente damos click en **Revisar y crear** y esperamos a que se complete la implementación.
10. Creamos la otra máquina virtual cuyo nombre será _Sesion4-vm2_ dentro del mismo grupo de recursos de la anterior máquina siguiendo los pasos 4 a 9. 
11. Dentro de la sección **Redes** seleccionamos la misma red virtual de la máquina virtual _Sesion4-vm1_. 
12. Finalmente damos click en **Revisar y crear** y esperamos a que se complete la implementación.
13. Podemos observar las dos máquinas virtuales dentro de nuestro grupo de recursos _sesion4-vm1_group_.

![Máquinas virtuales](https://github.com/DavePerales/Practica2_Maquinas_Virtuales/blob/main/01.png)

14. Seleccionamos la máquina virtual  _Sesion4-vm1_ y damos click en **Conectar** y seleccionamos la opción _RDP_. 

![Conectando la máquina virtual 1](https://github.com/DavePerales/Practica2_Maquinas_Virtuales/blob/main/02.png)

15. Damos click en **Descargar archivo RDP**, sin embargo, para poder abrir este archivo es necesarior ir a la Microsoft Store y descarga la aplicación _Remote Desktop_.
![Remote Desktop](https://github.com/DavePerales/Practica2_Maquinas_Virtuales/blob/main/03.png)

16. Una vez descargado el archivo procedemos a abrirlo con la aplicación _Remote Desktop_.

![Remote Desktop](https://github.com/DavePerales/Practica2_Maquinas_Virtuales/blob/main/04.png)

17. Iniciamos sesión con el usuario y contraseña que configuramos en el **paso 7**.

18. Abrimos el _Simbolo del sistema (CMD)_ y escribimos el siguiente comando:
>
>mstsc /v: Dirección IP de la segunda máquina virtual
>

Esta dirección puede ser consultada en la sección _Dispositivos conectados_ dentro de _sesion4-vm1_group-vnet_

![Direcciones IP](https://github.com/DavePerales/Practica2_Maquinas_Virtuales/blob/main/05.png)

19. Después de escribir el comando mstsc podemos acceder a la segunda máquina virtual dentro de la primer máquina virtual.








