<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo"></a></p>

<p align="center">
<a href="https://github.com/laravel/framework/actions"><img src="https://github.com/laravel/framework/workflows/tests/badge.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p>

## About Laravel

Laravel is a web application framework with expressive, elegant syntax. We believe development must be an enjoyable and creative experience to be truly fulfilling. Laravel takes the pain out of development by easing common tasks used in many web projects, such as:

- [Simple, fast routing engine](https://laravel.com/docs/routing).
- [Powerful dependency injection container](https://laravel.com/docs/container).
- Multiple back-ends for [session](https://laravel.com/docs/session) and [cache](https://laravel.com/docs/cache) storage.
- Expressive, intuitive [database ORM](https://laravel.com/docs/eloquent).
- Database agnostic [schema migrations](https://laravel.com/docs/migrations).
- [Robust background job processing](https://laravel.com/docs/queues).
- [Real-time event broadcasting](https://laravel.com/docs/broadcasting).

Laravel is accessible, powerful, and provides tools required for large, robust applications.

## Learning Laravel

Laravel has the most extensive and thorough [documentation](https://laravel.com/docs) and video tutorial library of all modern web application frameworks, making it a breeze to get started with the framework.

You may also try the [Laravel Bootcamp](https://bootcamp.laravel.com), where you will be guided through building a modern Laravel application from scratch.

If you don't feel like reading, [Laracasts](https://laracasts.com) can help. Laracasts contains over 2000 video tutorials on a range of topics including Laravel, modern PHP, unit testing, and JavaScript. Boost your skills by digging into our comprehensive video library.

## Laravel Sponsors

We would like to extend our thanks to the following sponsors for funding Laravel development. If you are interested in becoming a sponsor, please visit the Laravel [Patreon page](https://patreon.com/taylorotwell).

### Premium Partners

- **[Vehikl](https://vehikl.com/)**
- **[Tighten Co.](https://tighten.co)**
- **[Kirschbaum Development Group](https://kirschbaumdevelopment.com)**
- **[64 Robots](https://64robots.com)**
- **[Cubet Techno Labs](https://cubettech.com)**
- **[Cyber-Duck](https://cyber-duck.co.uk)**
- **[Many](https://www.many.co.uk)**
- **[Webdock, Fast VPS Hosting](https://www.webdock.io/en)**
- **[DevSquad](https://devsquad.com)**
- **[Curotec](https://www.curotec.com/services/technologies/laravel/)**
- **[OP.GG](https://op.gg)**
- **[WebReinvent](https://webreinvent.com/?utm_source=laravel&utm_medium=github&utm_campaign=patreon-sponsors)**
- **[Lendio](https://lendio.com)**

## Contributing

Thank you for considering contributing to the Laravel framework! The contribution guide can be found in the [Laravel documentation](https://laravel.com/docs/contributions).

## Code of Conduct

In order to ensure that the Laravel community is welcoming to all, please review and abide by the [Code of Conduct](https://laravel.com/docs/contributions#code-of-conduct).

## Security Vulnerabilities

If you discover a security vulnerability within Laravel, please send an e-mail to Taylor Otwell via [taylor@laravel.com](mailto:taylor@laravel.com). All security vulnerabilities will be promptly addressed.

## License

The Laravel framework is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).
"# laravel-sample-project" 
"# laravel-sample-project" 



// this is the setup of some feature

C:\Users\eldad>cd C:\xampp\htdocs\school\basic

C:\xampp\htdocs\school\basic>php artisan make:controller Demo/DemoController

   INFO  Controller [C:\xampp\htdocs\school\basic\app/Http/Controllers/Demo/DemoController.php] created successfully.


C:\xampp\htdocs\school\basic>php artisan make:middleware CheckAge

   INFO  Middleware [C:\xampp\htdocs\school\basic\app/Http/Middleware/CheckAge.php] created successfully.


C:\xampp\htdocs\school\basic>composer require laravel/breeze --dev
Cannot use laravel/breeze's latest version v2.3.8 as it requires php ^8.2.0 which is not satisfied by your platform.
./composer.json has been updated
Running composer update laravel/breeze
Loading composer repositories with package information
Updating dependencies
Lock file operations: 1 install, 0 updates, 0 removals
  - Locking laravel/breeze (v1.19.2)
Writing lock file
Installing dependencies from lock file (including require-dev)
Package operations: 1 install, 0 updates, 0 removals
  - Downloading laravel/breeze (v1.19.2)
    Failed to download laravel/breeze from dist: curl error 28 while downloading https://api.github.com/repos/laravel/breeze/zipball/725e0c4fb1f630afdd90b5fba2a7f6d8d547ac29: Connection timed out after 10009 milliseconds
    Now trying to download from source
  - Syncing laravel/breeze (v1.19.2) into cache
  - Installing laravel/breeze (v1.19.2): Cloning 725e0c4fb1 from cache
Generating optimized autoload files
> Illuminate\Foundation\ComposerScripts::postAutoloadDump
> @php artisan package:discover --ansi

   INFO  Discovering packages.

  laravel/breeze ................................................................................................ DONE
  laravel/sail .................................................................................................. DONE
  laravel/sanctum ............................................................................................... DONE
  laravel/tinker ................................................................................................ DONE
  nesbot/carbon ................................................................................................. DONE
  nunomaduro/collision .......................................................................................... DONE
  nunomaduro/termwind ........................................................................................... DONE
  spatie/laravel-ignition ....................................................................................... DONE

82 packages you are using are looking for funding.
Use the `composer fund` command to find out more!
> @php artisan vendor:publish --tag=laravel-assets --ansi --force

   INFO  No publishable resources for tag [laravel-assets].

Found 3 security vulnerability advisories affecting 3 packages.
Run "composer audit" for a full list of advisories.
Using version ^1.19 for laravel/breeze

C:\xampp\htdocs\school\basic>npm install && npm run dev

added 35 packages, and audited 36 packages in 43s

10 packages are looking for funding
  run `npm fund` for details

3 moderate severity vulnerabilities

To address all issues (including breaking changes), run:
  npm audit fix --force

Run `npm audit` for details.

> dev
> vite


C:\xampp\htdocs\school\basic>composer require laravel/breeze --dev
Cannot use laravel/breeze's latest version v2.3.8 as it requires php ^8.2.0 which is not satisfied by your platform.
./composer.json has been updated
Running composer update laravel/breeze
Loading composer repositories with package information
Updating dependencies
Lock file operations: 1 install, 0 updates, 0 removals
  - Locking laravel/breeze (v1.19.2)
Writing lock file
Installing dependencies from lock file (including require-dev)
Package operations: 1 install, 0 updates, 0 removals
  - Downloading laravel/breeze (v1.19.2)
    Failed to download laravel/breeze from dist: curl error 28 while downloading https://api.github.com/repos/laravel/breeze/zipball/725e0c4fb1f630afdd90b5fba2a7f6d8d547ac29: Connection timed out after 10009 milliseconds
    Now trying to download from source
  - Syncing laravel/breeze (v1.19.2) into cache
  - Installing laravel/breeze (v1.19.2): Cloning 725e0c4fb1 from cache
Generating optimized autoload files
> Illuminate\Foundation\ComposerScripts::postAutoloadDump
> @php artisan package:discover --ansi

   INFO  Discovering packages.

  laravel/breeze ................................................................................................ DONE
  laravel/sail .................................................................................................. DONE
  laravel/sanctum ............................................................................................... DONE
  laravel/tinker ................................................................................................ DONE
  nesbot/carbon ................................................................................................. DONE
  nunomaduro/collision .......................................................................................... DONE
  nunomaduro/termwind ........................................................................................... DONE
  spatie/laravel-ignition ....................................................................................... DONE

82 packages you are using are looking for funding.
Use the `composer fund` command to find out more!
> @php artisan vendor:publish --tag=laravel-assets --ansi --force

   INFO  No publishable resources for tag [laravel-assets].

Found 3 security vulnerability advisories affecting 3 packages.
Run "composer audit" for a full list of advisories.
Using version ^1.19 for laravel/breeze

C:\xampp\htdocs\school\basic>npm install && npm run dev

added 35 packages, and audited 36 packages in 43s

10 packages are looking for funding
  run `npm fund` for details

3 moderate severity vulnerabilities

To address all issues (including breaking changes), run:
  npm audit fix --force

Run `npm audit` for details.

> dev
> vite


  VITE v4.5.14  ready in 1018 ms

  ➜  Local:   http://localhost:5173/
  ➜  Network: use --host to expose
  ➜  press h to show help

  LARAVEL v9.52.20  plugin v0.7.8

  ➜  APP_URL: http://localhost

C:\xampp\htdocs\school\basic>php artisan breeze:install

  Which stack would you like to install?
  blade ............................................................................................................ 0
  react ............................................................................................................ 1
  vue .............................................................................................................. 2
  api .............................................................................................................. 3
❯ 0

  Would you like to install dark mode support? (yes/no) [no]
❯ no

  Would you prefer Pest tests instead of PHPUnit? (yes/no) [no]
❯ no

   INFO  Installing and building Node dependencies.


added 118 packages, and audited 154 packages in 1m

40 packages are looking for funding
  run `npm fund` for details

3 moderate severity vulnerabilities

To address all issues (including breaking changes), run:
  npm audit fix --force

Run `npm audit` for details.

> build
> vite build

    vite v4.5.14 building for production...
    transforming...
    ✓ 57 modules transformed.
    rendering chunks...
    computing gzip size...
public/build/manifest.json              0.26 kB │ gzip:  0.14 kB
public/build/assets/app-385ab86b.css   27.70 kB │ gzip:  5.43 kB
public/build/assets/app-4ba226a4.js   152.63 kB │ gzip: 56.63 kB
✓ built in 4.26s

   INFO  Breeze scaffolding installed successfully.



up to date, audited 154 packages in 2s

40 packages are looking for funding
  run `npm fund` for details

3 moderate severity vulnerabilities

To address all issues (including breaking changes), run:
  npm audit fix --force

Run `npm audit` for details.

> dev
> vite


  VITE v4.5.14  ready in 494 ms

  ➜  Local:   http://localhost:5173/
  ➜  Network: use --host to expose
  ➜  press h to show help

  LARAVEL v9.52.20  plugin v0.7.8

  ➜  APP_URL: http://localhost

C:\xampp\htdocs\school\basic>php artisan migrate

   INFO  Preparing database.

  Creating migration table ................................................................................. 27ms DONE

   INFO  Running migrations.

  2014_10_12_000000_create_users_table ..................................................................... 65ms DONE
  2014_10_12_100000_create_password_resets_table ........................................................... 66ms DONE
  2019_08_19_000000_create_failed_jobs_table ............................................................... 67ms DONE
  2019_12_14_000001_create_personal_access_tokens_table .................................................... 85ms DONE


C:\xampp\htdocs\school\basic>php artisan r:l

  GET|HEAD  / ........................................................................................................
  POST      _ignition/execute-solution . ignition.executeSolution › Spatie\LaravelIgnition › ExecuteSolutionController
  GET|HEAD  _ignition/health-check ............. ignition.healthCheck › Spatie\LaravelIgnition › HealthCheckController
  POST      _ignition/update-config .......... ignition.updateConfig › Spatie\LaravelIgnition › UpdateConfigController
  GET|HEAD  api/user .................................................................................................
  GET|HEAD  confirm-password .............................. password.confirm › Auth\ConfirmablePasswordController@show
  POST      confirm-password ................................................ Auth\ConfirmablePasswordController@store
  GET|HEAD  dashboard ...................................................................................... dashboard
  POST      email/verification-notification ... verification.send › Auth\EmailVerificationNotificationController@store
  GET|HEAD  forgot-password ............................... password.request › Auth\PasswordResetLinkController@create
  POST      forgot-password .................................. password.email › Auth\PasswordResetLinkController@store
  GET|HEAD  login ................................................. login › Auth\AuthenticatedSessionController@create
  POST      login .......................................................... Auth\AuthenticatedSessionController@store
  POST      logout .............................................. logout › Auth\AuthenticatedSessionController@destroy
  PUT       password ................................................ password.update › Auth\PasswordController@update
  GET|HEAD  profile ............................................................ profile.edit › ProfileController@edit
  PATCH     profile ........................................................ profile.update › ProfileController@update
  DELETE    profile ...................................................... profile.destroy › ProfileController@destroy
  GET|HEAD  register ................................................. register › Auth\RegisteredUserController@create
  POST      register ............................................................. Auth\RegisteredUserController@store
  POST      reset-password ......................................... password.store › Auth\NewPasswordController@store
  GET|HEAD  reset-password/{token} ................................ password.reset › Auth\NewPasswordController@create
  GET|HEAD  sanctum/csrf-cookie .................... sanctum.csrf-cookie › Laravel\Sanctum › CsrfCookieController@show
  GET|HEAD  verify-email ................................ verification.notice › Auth\EmailVerificationPromptController
  GET|HEAD  verify-email/{id}/{hash} ................................ verification.verify › Auth\VerifyEmailController

                                                                                                   Showing [25] routes
