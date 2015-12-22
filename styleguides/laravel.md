# Laravel

* Comenzar cada proyecto con el repositorio [base](https://github.com/Aphix-Labs/laravel-aphix-boilerplate)
* Considerar las guias de estilo base de [PHP](php.md)
* Siempre seguir estandar [PSR2](https://github.com/php-fig/fig-standards/blob/master/accepted/PSR-2-coding-style-guide.md)
* Las tablas deben ser en ingles y en plural. Ejemplo: `users`, `products`
* Traits deben terminar con el sufijo `Trait`. Ejemplo: `QueriesTrait`

## Controladores

* Controladores deben terminar con el sufijo `Controller`. Ejemplo: `UserController`

## Modelos
* Modelos deben ser la forma singular de la tabla. Ejemplo `user`, `product`

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

