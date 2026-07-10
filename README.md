<div align="center">

# EvaluacionGeoMarket

![Laravel](https://img.shields.io/badge/Laravel-FF2D20?style=flat-square&logo=laravel&logoColor=white)
![PHP](https://img.shields.io/badge/PHP-777BB4?style=flat-square&logo=php&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)
![Tailwind](https://img.shields.io/badge/TailwindCSS-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)

</div>

## 📋 Descripción

Proyecto de evaluación académica (SENA) enfocado en el manejo de relaciones de base de datos con Eloquent ORM en Laravel 12. El dominio simulado es "GeoMarket", un contexto de marketplace geolocalizado usado como caso de estudio para practicar diseño relacional.

## 🎯 Objetivos del ejercicio

Este proyecto evalúa específicamente:

1. **Migraciones**: creación de tablas con sus respectivas llaves foráneas.
2. **Relaciones a nivel de modelo**: definición de relaciones Eloquent (`belongsTo`, `hasMany`, etc.) entre los modelos del dominio GeoMarket.
3. **Verificación de relaciones**: pruebas de las relaciones a través de un `OrmController` dedicado, que expone el resultado de las consultas relacionales.

No es una aplicación de producto terminada — es un ejercicio dirigido a demostrar dominio técnico de Eloquent y diseño de base de datos relacional.

## 🛠️ Stack tecnológico

**Backend**
- Laravel 12.0
- PHP ^8.2
- Composer

**Frontend**
- Blade (vistas)
- Tailwind CSS 4.0
- Vite 7.0.7
- Axios 1.11

**Testing**
- PHPUnit 11.5.3
- Mockery

**Herramientas de desarrollo**
- Laravel Pint (formateo de código)
- Laravel Pail (monitoreo de logs)
- Laravel Sail (contenedores Docker)
- FakerPHP (datos de prueba)

## 📦 Instalación

```bash
git clone https://github.com/Camilocostas/EvaluacionGeoMarket.git
cd EvaluacionGeoMarket

composer install
npm install

cp .env.example .env
php artisan key:generate
```

Configura tu base de datos en `.env`, luego:

```bash
php artisan migrate
npm run build
php artisan serve
```

O, de forma más rápida, usando el script de Composer incluido:

```bash
composer setup
```

## 🔧 Desarrollo

```bash
composer dev     # Levanta servidor, queue, logs (pail) y npm en paralelo
npm run dev      # Solo Vite con hot reload
composer test    # Ejecutar tests con PHPUnit
```

## 🗂️ Estructura del proyecto

```
EvaluacionGeoMarket/
├── app/            # Modelos, controladores (incluye OrmController)
├── database/       # Migraciones y seeders
├── resources/      # Vistas Blade y assets (CSS/JS)
├── routes/         # Definición de rutas
├── tests/          # Tests unitarios y de feature
└── ...
```

## 🧪 Verificar las relaciones

El `OrmController` es el punto central para comprobar que las relaciones entre modelos funcionan correctamente. Revisa `app/Http/Controllers/OrmController.php` y las rutas asociadas para ver las consultas relacionales en acción.

## 📄 Licencia

Este proyecto está bajo la Licencia MIT. Ver el archivo [LICENSE](LICENSE) para más detalles.

## 📞 Contacto

Repositorio: [Camilocostas/EvaluacionGeoMarket](https://github.com/Camilocostas/EvaluacionGeoMarket)
