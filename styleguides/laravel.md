# Laravel

* Comenzar cada proyecto con el repositorio [base](https://github.com/Aphix-Labs/laravel-aphix-boilerplate)
* Considerar las guias de estilo base de [PHP](php.md)
* Siempre seguir estandar [PSR2](https://github.com/php-fig/fig-standards/blob/master/accepted/PSR-2-coding-style-guide.md)
* Las tablas deben ser en ingles y en plural. Ejemplo: `users`, `products`
* Traits deben terminar con el sufijo `Trait`. Ejemplo: `QueriesTrait`

## Rutas

* Recursos en plural. Ejemplo: `products`, `products/7`
* Nunca escribir slash al comienzo ni al final de una ruta. Mal: `/users/`, Bien: `users`
* Si se usan rutas independientes, apegarse lo mas cercano posible a la forma que son generadas cuando se usan controladores REST con la palabra `resources`. Ejemplo: `products/1/edit`[Ver documentación] (https://laravel.com/docs/5.1/controllers#restful-resource-controllers)

## Controladores

* Controladores deben terminar con el sufijo `Controller`. Ejemplo: `UserController`
* En lo posible seguir controladores REST, ya sea para mantenedores y acciones del mismo estilo

## Modelos

* Modelos deben ser la forma singular de la tabla. Ejemplo `User`, `Product`

Tip: Al generar un modelo con `artisan`, usar el flag `m` para generar el archivo de migración automaticamente

```
php artisan make:model Product -m

```

Esto generara automaticamente la migracion para la tabla products

* Para evitar `MassAsignment` se debe usar siempre la propiedad `fillable`. Cada propiedad debe ser listado en una linea nueva. Ejemplo:

```php

protected $fillable = [
    'name',
    'type',
    'user_id'
];
```

# Vistas

* Parciales comiezan con un guion bajo. Ejemplo: 'partials/_common_error.blade.php'
* Usar carpeta partials en lo posible para almacenarlos

