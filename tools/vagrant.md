# Vagrant

Para mantener el mismo entorno de las herramientas de desarrollo se utiliza [vagrant](http://www.vagrantup.com)

### Homestead

La mayoria de los proyectos al ser proyectos laravel usamos el box [homestead](http://laravel.com/docs/homestead) la contiene todos los requerimientos necesarios para comenzar un proyecto laravel, tales como postgres, git, php, node, entre otros.

### Conectarse a Sequel Pro (MySQL)

Para conectarse a MySQL de la box `homestead` se deben hacer uso de los siguientes datos en la pestaña 'standard'

* Host: 127.0.0.1
* Usuario: homestead
* Clave: secret
* Puerto: 33060

<img src="/assets/vagrant/sequel_pro.png" align="middle"/>

### Conectarse a Navicat (Postgres)

Para conectarse a Postgres de la box `homestead` se deben hacer uso de los siguientes datos en la pestaña 'general'

* Host: 127.0.0.1
* Usuario: homestead
* Clave: secret
* Puerto: 54320

<img src="/assets/vagrant/navicat.png" align="middle"/>

