# Uso de Azure NSG
En este repositorio tenemos una demostración de la creación del recurso de Azure NSG y como aplicar su uso con una Virtual Machine.

![Microsoft-Azure-NSG](https://www.checkpoint.com/wp-content/uploads/microsoft-azure-nsg-network-security-groups-logo-1.png)

---

## Requisitos
- Cuenta en [Microsoft Azure](https://portal.azure.com)
- Un dispositivo, por ejemplo una computadora
- Acceso a internet
- Navegador de internet como Google Chrome, Opera, Mozilla Firefox, etc.

---

## Importante
- En este repositorio haremos uso de "NSG" en una "Virtual Machine", todo esto dentro de Azure.
- Es importante que el "NSG" y la "Virtual Machine", se encuentren dentro de la misma región.
- Haremos uso de la creación de reglas.

---

## Pasos a seguir

- Lo primero es entrar en [Microsoft Azure](https://portal.azure.com).
- Crearemos una "Virtual Machine"

![P1](https://github.com/DagonNR/NSG-VM/blob/main/images/P1.PNG)

- Es importante que tenga estás características

![P2](https://github.com/DagonNR/NSG-VM/blob/main/images/P2.PNG)

![P3](https://github.com/DagonNR/NSG-VM/blob/main/images/P3.PNG)

- Ahora toca crear un NSG, para ello lo buscaremos como "Grupos de seguridad de red"

![P4](https://github.com/DagonNR/NSG-VM/blob/main/images/P4.PNG)

- Ya creado el recurso, entraremos en él.
- Ahora en el apartado de "Interfaces de red"
- Clicaremos en "Asociar"

![P5](https://github.com/DagonNR/NSG-VM/blob/main/images/P5.PNG)

- Aqui buscaremos la red de la "VM".

![P6](https://github.com/DagonNR/NSG-VM/blob/main/images/P6.PNG)

- Ya asociada nos dirigiremos a "Reglas de seguridad de entrada".
- Clicaremos en "Agregar"

![P7](https://github.com/DagonNR/NSG-VM/blob/main/images/P7.PNG)

- Colocaremos lo siguiente, para poder acceder a la "VM", ya que al crearala no le dimos ningún puerto para acceder.

![P8](https://github.com/DagonNR/NSG-VM/blob/main/images/P8.PNG)

- Ya con esto agregado, podremos entrar en la "VM".

![P9](https://github.com/DagonNR/NSG-VM/blob/main/images/P9.PNG)

- Ahora haremos una regla para no poder usar internet con la "VM".
- Por ahora les mostrare que si podemos usar internet.

![P10](https://github.com/DagonNR/NSG-VM/blob/main/images/P10.PNG)

![P11](https://github.com/DagonNR/NSG-VM/blob/main/images/P11.PNG)

- Ahora regresaremos a [Microsoft Azure](https://portal.azure.com).
- Entraremos de nuevo en nuestro recurso de "NSG"
- Entraremos al apartado de "Reglas de seguridad de salida"
- Clicaremos en "+ Agregar"

![P12](https://github.com/DagonNR/NSG-VM/blob/main/images/P12.PNG)

- Para quitar el acceso a internet, colocaremos lo siguiente.

![P13](https://github.com/DagonNR/NSG-VM/blob/main/images/P13.PNG)

- Si ahora regresamos a la "VM", no podremos usar internet (tal vez tarde unos minutos).

![P14](https://github.com/DagonNR/NSG-VM/blob/main/images/P14.PNG)
