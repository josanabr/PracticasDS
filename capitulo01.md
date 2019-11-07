# Introducción a los sistemas distribuidos

Este capítulo se divide en tres grandes secciones, 

* ¿Qué es un sistema distribuido?
* Sus metas de diseño
* Tipos de sistemas distribuidos

Dentro de los temas que se quieren evidenciar de forma práctica se listan los siguientes:

* Un sistema distribuido se presenta a los usuarios como una entidad única 
* Los sistemas distribuidos permiten la ejecución de código de forma remota

## Un sistema distribuido se presenta como una sola entidad

En este [enlace](https://github.com/josanabr/vagrant_haproxy.git) se puede descargar el repositorio que le permite crear un balanceador para una granja de servidores web. 

[Aquí](https://www.howtoforge.com/tutorial/ubuntu-load-balancer-haproxy/) la fuente de donde se tomaron los pasos para el despliegue automático del balanceador de carga HAProxy. 

Para usar el código de este repositorio debe ejecutar los siguientes pasos:
Clonar el repositorio

```
git clone https://github.com/josanabr/vagrant_haproxy.git
```

Ingresar a la carpeta del repositorio recien creado

```
cd  vagrant_haproxy
```

Ir al *branch* donde está la versión definitiva del código que permite crear de forma automática un balanceador de carga para una granja de servidores web

```
git checkout 06-final
```

Por último, levantar la granja de servidores

```
vagrant up
```

Apunte su navegador al URl `http://192.168.200.5`.

## Ejecución de código de forma remota

Para esta práctica se requiere crear dos máquinas virtuales. 
Usar el siguiente [Vagrantfile](Vagrantfile).
Una vez las máquinas virtuales han sido desplegadas se procede a ejecutar las actividades descritas en el siguiente [enlace](https://www.tutorialspoint.com/python_network_programming/python_remote_procedure_call.htm).

Haga los ajustes necesarios para que su código corra en el ambiente generado en el `Vagrantfile`.
