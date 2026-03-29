## my custom rules <felipesantos2>

## DEFINITIONS
    We are working on a Laravel 13 project running in a Docker environment with Sail CLI support
##### Laravel Rules
    -> Always use sail command: 
        -  `sail up -d `, 
        -  `sail composer install`,
        -  `sail art make:model -m` 
        -  `sail art make:model` 
        -  `sail art make:migration` 
        -  `./vendor/bin/sail up -d` 
        -  `./vendor/bin/sail artisan make:model -m` 
        -  `./vendor/bin/sail artisan make:model` 
        -  `./vendor/bin/sail artisan make:migration` 
        -  `./vendor/bin/sail npm install` 
    -> Always use Facades insted laravel helpers. Ex: `Str::limit` insted `str()->limit()`
    -> Always make sure that the columns in the migrations are reflected in the models in the `$fillable` variable
    -> Tables, primary keys and foreign keys are in English, while the other columns are in Portuguese
    -> For each new feature, you’ll implement a test—in a simple way, without complex jargon
    -> ** KEY RULE/CRITICAL RULE:** Our code is read and interpreted by humans, so I’ll emphasize again that our code should not be unnecessarily complex; we should always implement the solution in the simplest way possible!
    -> Always use Eloquent ORM insted raw queries
    -> **Never** use `::query()` in query constructions. Use this `User::all()` instead this `User::query()->all()`
    -> **Never** add useless, irrelevant, or unnecessary comments to the code
##### Commits Rules
    -> Always add commits in english, with semantic commit. Ex: feat: xxxx, chore: xxxx
##### Front End ==  Livewire 4
    -> We're using LiveWire 4 alongside **Alpine.js**. I'll look into it—no plugins (jQuery) and pure JavaScript.
    -> For CSS, we're using the `tailwindcss` library, and that's your only option
##### Linting == Laravel Pint
    -> Always use `pint.json` for linting the code
