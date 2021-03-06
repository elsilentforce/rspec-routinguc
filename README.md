# Introducción a RSpec para RoutingUC
El siguiente proyecto trata de un ejemplo básico para la creación de una nueva aplicación TDD.
Para ello se utiliza:
* Rails 5
* RSpec


## Creación de aplicación
Si lo que queremos es desarrollar una aplicación desde 0 utilizando como suite de pruebas RSpec debemos crearla utilizando el comando

```rails new app-name -T```

El comando -T indica que se ignore la suite de pruebas `Minitest` que viene por defecto con Rails.

## Instalación de RSpec
Para instalar RSpec basta con agregar dentro de nuestro archivo `Gemfile`

```
group :development, :test do
  gem 'rspec-rails'
end
```

Una vez agregada la gema procedemos a instalarla

``` bundle install ```

RSpec luego de ser instalada necesita ser inicializada, para ello corremos el comando

``` rails generate rspec:install ```

Esto genera el directorio `spec` donde escribiremos nuestros respectivos test.

A modo de ejemplo se generó un User Scaffold el cual automáticamente creó una serie de pruebas básicas en el directorio mencionado anteriormente.
