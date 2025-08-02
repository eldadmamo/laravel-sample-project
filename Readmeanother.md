C:\Users\eldad>node -v
v22.17.1

C:\Users\eldad>cd C:\xampp\htdocs\school

C:\xampp\htdocs\school>php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');"

C:\xampp\htdocs\school>php -r "if (hash_file('sha384', 'composer-setup.php') === 'dac665fdc30fdd8ec78b38b9800061b4150413ff2e3b6f88543c636f7cd84f6db9189d43a81e5503cda447da73c7e5b6') { echo 'Installer verified'.PHP_EOL; } else { echo 'Installer corrupt'.PHP_EOL; unlink('composer-setup.php'); exit(1); }"
Installer verified

C:\xampp\htdocs\school>php composer-setup.php
All settings correct for using Composer
Downloading...

Composer (version 2.8.10) successfully installed to: C:\xampp\htdocs\school\composer.phar
Use it: php composer.phar


C:\xampp\htdocs\school>php -r "unlink('composer-setup.php');"

C:\xampp\htdocs\school>composer -v
   ______
  / ____/___  ____ ___  ____  ____  ________  _____
 / /   / __ \/ __ `__ \/ __ \/ __ \/ ___/ _ \/ ___/
/ /___/ /_/ / / / / / / /_/ / /_/ (__  )  __/ /
\____/\____/_/ /_/ /_/ .___/\____/____/\___/_/
                    /_/
Composer version 2.8.10 2025-07-10 19:08:33

Usage:
  command [options] [arguments]

Options:
  -h, --help                     Display help for the given command. When no command is given display help for the list command
  -q, --quiet                    Do not output any message
  -V, --version                  Display this application version
      --ansi|--no-ansi           Force (or disable --no-ansi) ANSI output
  -n, --no-interaction           Do not ask any interactive question
      --profile                  Display timing and memory usage information
      --no-plugins               Whether to disable plugins.
      --no-scripts               Skips the execution of all scripts defined in composer.json file.
  -d, --working-dir=WORKING-DIR  If specified, use the given directory as working directory.
      --no-cache                 Prevent use of the cache
  -v|vv|vvv, --verbose           Increase the verbosity of messages: 1 for normal output, 2 for more verbose output and 3 for debug

Available commands:
  about                Shows a short information about Composer
  archive              Creates an archive of this composer package
  audit                Checks for security vulnerability advisories for installed packages
  browse               [home] Opens the package's repository URL or homepage in your browser
  bump                 Increases the lower limit of your composer.json requirements to the currently installed versions
  check-platform-reqs  Check that platform requirements are satisfied
  clear-cache          [clearcache|cc] Clears composer's internal package cache
  completion           Dump the shell completion script
  config               Sets config options
  create-project       Creates new project from a package into given directory
  depends              [why] Shows which packages cause the given package to be installed
  diagnose             Diagnoses the system to identify common errors
  dump-autoload        [dumpautoload] Dumps the autoloader
  exec                 Executes a vendored binary/script
  fund                 Discover how to help fund the maintenance of your dependencies
  global               Allows running commands in the global composer dir ($COMPOSER_HOME)
  help                 Display help for a command
  init                 Creates a basic composer.json file in current directory
  install              [i] Installs the project dependencies from the composer.lock file if present, or falls back on the composer.json
  licenses             Shows information about licenses of dependencies
  list                 List commands
  outdated             Shows a list of installed packages that have updates available, including their latest version
  prohibits            [why-not] Shows which packages prevent the given package from being installed
  reinstall            Uninstalls and reinstalls the given package names
  remove               [rm|uninstall] Removes a package from the require or require-dev
  require              [r] Adds required packages to your composer.json and installs them
  run-script           [run] Runs the scripts defined in composer.json
  search               Searches for packages
  self-update          [selfupdate] Updates composer.phar to the latest version
  show                 [info] Shows information about packages
  status               Shows a list of locally modified packages
  suggests             Shows package suggestions
  update               [u|upgrade] Updates your dependencies to the latest version according to composer.json, and updates the composer.lock file
  validate             Validates a composer.json and composer.lock

C:\xampp\htdocs\school>composer create-project laravel/laravel basic
Creating a "laravel/laravel" project at "./basic"
Cannot use laravel/laravel's latest version v12.2.0 as it requires php ^8.2 which is not satisfied by your platform.
Installing laravel/laravel (v9.5.2)
  - Installing laravel/laravel (v9.5.2): Extracting archive
Created project in C:\xampp\htdocs\school\basic
> @php -r "file_exists('.env') || copy('.env.example', '.env');"
Loading composer repositories with package information
Updating dependencies
Lock file operations: 112 installs, 0 updates, 0 removals
  - Locking brick/math (0.11.0)
  - Locking carbonphp/carbon-doctrine-types (2.1.0)
  - Locking dflydev/dot-access-data (v3.0.3)
  - Locking doctrine/deprecations (1.1.5)
  - Locking doctrine/inflector (2.0.10)
  - Locking doctrine/instantiator (1.5.0)
  - Locking doctrine/lexer (2.1.1)
  - Locking dragonmantank/cron-expression (v3.4.0)
  - Locking egulias/email-validator (3.2.6)
  - Locking fakerphp/faker (v1.24.1)
  - Locking filp/whoops (2.18.3)
  - Locking fruitcake/php-cors (v1.3.0)
  - Locking graham-campbell/result-type (v1.1.3)
  - Locking guzzlehttp/guzzle (7.9.3)
  - Locking guzzlehttp/promises (2.2.0)
  - Locking guzzlehttp/psr7 (2.7.1)
  - Locking guzzlehttp/uri-template (v1.0.4)
  - Locking hamcrest/hamcrest-php (v2.1.1)
  - Locking laravel/framework (v9.52.20)
  - Locking laravel/pint (v1.5.0)
  - Locking laravel/sail (v1.44.0)
  - Locking laravel/sanctum (v3.3.3)
  - Locking laravel/serializable-closure (v1.3.7)
  - Locking laravel/tinker (v2.10.1)
  - Locking league/commonmark (2.7.1)
  - Locking league/config (v1.2.0)
  - Locking league/flysystem (3.30.0)
  - Locking league/flysystem-local (3.30.0)
  - Locking league/mime-type-detection (1.16.0)
  - Locking mockery/mockery (1.6.12)
  - Locking monolog/monolog (2.10.0)
  - Locking myclabs/deep-copy (1.13.4)
  - Locking nesbot/carbon (2.73.0)
  - Locking nette/schema (v1.2.5)
  - Locking nette/utils (v4.0.7)
  - Locking nikic/php-parser (v5.6.0)
  - Locking nunomaduro/collision (v6.4.0)
  - Locking nunomaduro/termwind (v1.15.1)
  - Locking phar-io/manifest (2.0.4)
  - Locking phar-io/version (3.2.1)
  - Locking phpoption/phpoption (1.9.3)
  - Locking phpunit/php-code-coverage (9.2.32)
  - Locking phpunit/php-file-iterator (3.0.6)
  - Locking phpunit/php-invoker (3.1.1)
  - Locking phpunit/php-text-template (2.0.4)
  - Locking phpunit/php-timer (5.0.3)
  - Locking phpunit/phpunit (9.6.23)
  - Locking psr/clock (1.0.0)
  - Locking psr/container (2.0.2)
  - Locking psr/event-dispatcher (1.0.0)
  - Locking psr/http-client (1.0.3)
  - Locking psr/http-factory (1.1.0)
  - Locking psr/http-message (2.0)
  - Locking psr/log (3.0.2)
  - Locking psr/simple-cache (3.0.0)
  - Locking psy/psysh (v0.12.9)
  - Locking ralouphie/getallheaders (3.0.3)
  - Locking ramsey/collection (1.3.0)
  - Locking ramsey/uuid (4.9.0)
  - Locking sebastian/cli-parser (1.0.2)
  - Locking sebastian/code-unit (1.0.8)
  - Locking sebastian/code-unit-reverse-lookup (2.0.3)
  - Locking sebastian/comparator (4.0.8)
  - Locking sebastian/complexity (2.0.3)
  - Locking sebastian/diff (4.0.6)
  - Locking sebastian/environment (5.1.5)
  - Locking sebastian/exporter (4.0.6)
  - Locking sebastian/global-state (5.0.7)
  - Locking sebastian/lines-of-code (1.0.4)
  - Locking sebastian/object-enumerator (4.0.4)
  - Locking sebastian/object-reflector (2.0.4)
  - Locking sebastian/recursion-context (4.0.5)
  - Locking sebastian/resource-operations (3.0.4)
  - Locking sebastian/type (3.2.1)
  - Locking sebastian/version (3.0.2)
  - Locking spatie/backtrace (1.7.4)
  - Locking spatie/flare-client-php (1.10.1)
  - Locking spatie/ignition (1.14.2)
  - Locking spatie/laravel-ignition (1.7.0)
  - Locking symfony/console (v6.0.19)
  - Locking symfony/css-selector (v6.0.19)
  - Locking symfony/deprecation-contracts (v3.0.2)
  - Locking symfony/error-handler (v6.0.19)
  - Locking symfony/event-dispatcher (v6.0.19)
  - Locking symfony/event-dispatcher-contracts (v3.0.2)
  - Locking symfony/finder (v6.0.19)
  - Locking symfony/http-foundation (v6.0.20)
  - Locking symfony/http-kernel (v6.0.20)
  - Locking symfony/mailer (v6.0.19)
  - Locking symfony/mime (v6.0.19)
  - Locking symfony/polyfill-ctype (v1.32.0)
  - Locking symfony/polyfill-intl-grapheme (v1.32.0)
  - Locking symfony/polyfill-intl-idn (v1.32.0)
  - Locking symfony/polyfill-intl-normalizer (v1.32.0)
  - Locking symfony/polyfill-mbstring (v1.32.0)
  - Locking symfony/polyfill-php80 (v1.32.0)
  - Locking symfony/polyfill-php81 (v1.32.0)
  - Locking symfony/polyfill-uuid (v1.32.0)
  - Locking symfony/process (v6.0.19)
  - Locking symfony/routing (v6.0.19)
  - Locking symfony/service-contracts (v3.0.2)
  - Locking symfony/string (v6.0.19)
  - Locking symfony/translation (v6.0.19)
  - Locking symfony/translation-contracts (v3.0.2)
  - Locking symfony/uid (v6.0.19)
  - Locking symfony/var-dumper (v6.0.19)
  - Locking symfony/yaml (v6.0.19)
  - Locking theseer/tokenizer (1.2.3)
  - Locking tijsverkoyen/css-to-inline-styles (v2.3.0)
  - Locking vlucas/phpdotenv (v5.6.2)
  - Locking voku/portable-ascii (2.0.3)
  - Locking webmozart/assert (1.11.0)
Writing lock file
Installing dependencies from lock file (including require-dev)
Package operations: 112 installs, 0 updates, 0 removals
  - Downloading myclabs/deep-copy (1.13.4)
  - Installing doctrine/inflector (2.0.10): Extracting archive
  - Installing doctrine/deprecations (1.1.5): Extracting archive
  - Installing doctrine/lexer (2.1.1): Extracting archive
  - Installing symfony/polyfill-ctype (v1.32.0): Extracting archive
  - Installing webmozart/assert (1.11.0): Extracting archive
  - Installing dragonmantank/cron-expression (v3.4.0): Extracting archive
  - Installing symfony/deprecation-contracts (v3.0.2): Extracting archive
  - Installing psr/container (2.0.2): Extracting archive
  - Installing fakerphp/faker (v1.24.1): Extracting archive
  - Installing symfony/polyfill-mbstring (v1.32.0): Extracting archive
  - Installing symfony/http-foundation (v6.0.20): Extracting archive
  - Installing fruitcake/php-cors (v1.3.0): Extracting archive
  - Installing psr/http-message (2.0): Extracting archive
  - Installing psr/http-client (1.0.3): Extracting archive
  - Installing ralouphie/getallheaders (3.0.3): Extracting archive
  - Installing psr/http-factory (1.1.0): Extracting archive
  - Installing guzzlehttp/psr7 (2.7.1): Extracting archive
  - Installing guzzlehttp/promises (2.2.0): Extracting archive
  - Installing guzzlehttp/guzzle (7.9.3): Extracting archive
  - Installing symfony/polyfill-php80 (v1.32.0): Extracting archive
  - Installing guzzlehttp/uri-template (v1.0.4): Extracting archive
  - Installing laravel/pint (v1.5.0): Extracting archive
  - Installing symfony/yaml (v6.0.19): Extracting archive
  - Installing symfony/polyfill-intl-normalizer (v1.32.0): Extracting archive
  - Installing symfony/polyfill-intl-grapheme (v1.32.0): Extracting archive
  - Installing symfony/string (v6.0.19): Extracting archive
  - Installing symfony/service-contracts (v3.0.2): Extracting archive
  - Installing symfony/console (v6.0.19): Extracting archive
  - Installing voku/portable-ascii (2.0.3): Extracting archive
  - Installing phpoption/phpoption (1.9.3): Extracting archive
  - Installing graham-campbell/result-type (v1.1.3): Extracting archive
  - Installing vlucas/phpdotenv (v5.6.2): Extracting archive
  - Installing symfony/css-selector (v6.0.19): Extracting archive
  - Installing tijsverkoyen/css-to-inline-styles (v2.3.0): Extracting archive
  - Installing symfony/var-dumper (v6.0.19): Extracting archive
  - Installing symfony/polyfill-uuid (v1.32.0): Extracting archive
  - Installing symfony/uid (v6.0.19): Extracting archive
  - Installing symfony/routing (v6.0.19): Extracting archive
  - Installing symfony/process (v6.0.19): Extracting archive
  - Installing symfony/polyfill-intl-idn (v1.32.0): Extracting archive
  - Installing symfony/mime (v6.0.19): Extracting archive
  - Installing psr/event-dispatcher (1.0.0): Extracting archive
  - Installing symfony/event-dispatcher-contracts (v3.0.2): Extracting archive
  - Installing symfony/event-dispatcher (v6.0.19): Extracting archive
  - Installing psr/log (3.0.2): Extracting archive
  - Installing egulias/email-validator (3.2.6): Extracting archive
  - Installing symfony/mailer (v6.0.19): Extracting archive
  - Installing symfony/error-handler (v6.0.19): Extracting archive
  - Installing symfony/http-kernel (v6.0.20): Extracting archive
  - Installing symfony/finder (v6.0.19): Extracting archive
  - Installing symfony/polyfill-php81 (v1.32.0): Extracting archive
  - Installing ramsey/collection (1.3.0): Extracting archive
  - Installing brick/math (0.11.0): Extracting archive
  - Installing ramsey/uuid (4.9.0): Extracting archive
  - Installing psr/simple-cache (3.0.0): Extracting archive
  - Installing nunomaduro/termwind (v1.15.1): Extracting archive
  - Installing symfony/translation-contracts (v3.0.2): Extracting archive
  - Installing symfony/translation (v6.0.19): Extracting archive
  - Installing psr/clock (1.0.0): Extracting archive
  - Installing carbonphp/carbon-doctrine-types (2.1.0): Extracting archive
  - Installing nesbot/carbon (2.73.0): Extracting archive
  - Installing monolog/monolog (2.10.0): Extracting archive
  - Installing league/mime-type-detection (1.16.0): Extracting archive
  - Installing league/flysystem (3.30.0): Extracting archive
  - Installing league/flysystem-local (3.30.0): Extracting archive
  - Installing nette/utils (v4.0.7): Extracting archive
  - Installing nette/schema (v1.2.5): Extracting archive
  - Installing dflydev/dot-access-data (v3.0.3): Extracting archive
  - Installing league/config (v1.2.0): Extracting archive
  - Installing league/commonmark (2.7.1): Extracting archive
  - Installing laravel/serializable-closure (v1.3.7): Extracting archive
  - Installing laravel/framework (v9.52.20): Extracting archive
  - Installing laravel/sail (v1.44.0): Extracting archive
  - Installing laravel/sanctum (v3.3.3): Extracting archive
  - Installing nikic/php-parser (v5.6.0): Extracting archive
  - Installing psy/psysh (v0.12.9): Extracting archive
  - Installing laravel/tinker (v2.10.1): Extracting archive
  - Installing hamcrest/hamcrest-php (v2.1.1): Extracting archive
  - Installing mockery/mockery (1.6.12): Extracting archive
  - Installing filp/whoops (2.18.3): Extracting archive
  - Installing nunomaduro/collision (v6.4.0): Extracting archive
  - Installing sebastian/version (3.0.2): Extracting archive
  - Installing sebastian/type (3.2.1): Extracting archive
  - Installing sebastian/resource-operations (3.0.4): Extracting archive
  - Installing sebastian/recursion-context (4.0.5): Extracting archive
  - Installing sebastian/object-reflector (2.0.4): Extracting archive
  - Installing sebastian/object-enumerator (4.0.4): Extracting archive
  - Installing sebastian/global-state (5.0.7): Extracting archive
  - Installing sebastian/exporter (4.0.6): Extracting archive
  - Installing sebastian/environment (5.1.5): Extracting archive
  - Installing sebastian/diff (4.0.6): Extracting archive
  - Installing sebastian/comparator (4.0.8): Extracting archive
  - Installing sebastian/code-unit (1.0.8): Extracting archive
  - Installing sebastian/cli-parser (1.0.2): Extracting archive
  - Installing phpunit/php-timer (5.0.3): Extracting archive
  - Installing phpunit/php-text-template (2.0.4): Extracting archive
  - Installing phpunit/php-invoker (3.1.1): Extracting archive
  - Installing phpunit/php-file-iterator (3.0.6): Extracting archive
  - Installing theseer/tokenizer (1.2.3): Extracting archive
  - Installing sebastian/lines-of-code (1.0.4): Extracting archive
  - Installing sebastian/complexity (2.0.3): Extracting archive
  - Installing sebastian/code-unit-reverse-lookup (2.0.3): Extracting archive
  - Installing phpunit/php-code-coverage (9.2.32): Extracting archive
  - Installing phar-io/version (3.2.1): Extracting archive
  - Installing phar-io/manifest (2.0.4): Extracting archive
  - Installing myclabs/deep-copy (1.13.4): Extracting archive
  - Installing doctrine/instantiator (1.5.0): Extracting archive
  - Installing phpunit/phpunit (9.6.23): Extracting archive
  - Installing spatie/backtrace (1.7.4): Extracting archive
  - Installing spatie/flare-client-php (1.10.1): Extracting archive
  - Installing spatie/ignition (1.14.2): Extracting archive
  - Installing spatie/laravel-ignition (1.7.0): Extracting archive
70 package suggestions were added by new dependencies, use `composer suggest` to see details.
Generating optimized autoload files
> Illuminate\Foundation\ComposerScripts::postAutoloadDump
> @php artisan package:discover --ansi

   INFO  Discovering packages.

  laravel/sail ..................................................................... DONE
  laravel/sanctum .................................................................. DONE
  laravel/tinker ................................................................... DONE
  nesbot/carbon .................................................................... DONE
  nunomaduro/collision ............................................................. DONE
  nunomaduro/termwind .............................................................. DONE
  spatie/laravel-ignition .......................................................... DONE

82 packages you are using are looking for funding.
Use the `composer fund` command to find out more!
> @php artisan vendor:publish --tag=laravel-assets --ansi --force

   INFO  No publishable resources for tag [laravel-assets].

Found 3 security vulnerability advisories affecting 3 packages.
Run "composer audit" for a full list of advisories.
> @php artisan key:generate --ansi

   INFO  Application key set successfully.


C:\xampp\htdocs\school>cd basic

C:\xampp\htdocs\school\basic>code .

C:\xampp\htdocs\school\basic>php artisan serve

   INFO  Server running on [http://127.0.0.1:8000].

  Press Ctrl+C to stop the server

  2025-08-02 10:42:51 .............................................................. ~ 0s
  2025-08-02 10:42:51 /favicon.ico ................................................. ~ 0s
  2025-08-02 11:14:21 .............................................................. ~ 0s
  2025-08-02 11:14:21 /favicon.ico ................................................. ~ 0s
  2025-08-02 11:14:27 .............................................................. ~ 0s
  2025-08-02 11:14:27 /favicon.ico ................................................. ~ 0s
  2025-08-02 11:14:59 .............................................................. ~ 0s
  2025-08-02 11:14:59 /favicon.ico ................................................. ~ 0s
  2025-08-02 11:18:18 .............................................................. ~ 0s
  2025-08-02 11:18:18 /favicon.ico ................................................. ~ 0s
  2025-08-02 11:20:51 .............................................................. ~ 1s
  2025-08-02 11:20:51 /favicon.ico ................................................. ~ 1s
  2025-08-02 12:01:06 .............................................................. ~ 1s
  2025-08-02 12:01:06 /favicon.ico ................................................. ~ 1s
  2025-08-02 12:01:10 .............................................................. ~ 1s
  2025-08-02 12:01:10 /favicon.ico ................................................. ~ 1s
  2025-08-02 12:01:22 .............................................................. ~ 0s
  2025-08-02 12:01:22 /favicon.ico ................................................. ~ 0s
  2025-08-02 12:03:49 .............................................................. ~ 0s
  2025-08-02 12:03:49 /favicon.ico ................................................. ~ 0s
  2025-08-02 12:03:53 .............................................................. ~ 0s
  2025-08-02 12:03:53 /favicon.ico ................................................. ~ 0s
  2025-08-02 12:04:07 .............................................................. ~ 0s
  2025-08-02 12:04:07 /favicon.ico ................................................. ~ 0s
  2025-08-02 14:22:50 .............................................................. ~ 1s
  2025-08-02 14:22:51 /favicon.ico ................................................. ~ 0s
  2025-08-02 14:22:53 .............................................................. ~ 1s
  2025-08-02 14:22:54 /favicon.ico ................................................. ~ 0s
  2025-08-02 14:23:06 .............................................................. ~ 1s
  2025-08-02 14:23:07 /favicon.ico ................................................. ~ 0s
  2025-08-02 14:23:21 .............................................................. ~ 0s
  2025-08-02 14:23:21 /favicon.ico ................................................. ~ 0s
  2025-08-02 14:23:23 .............................................................. ~ 1s
  2025-08-02 14:23:24 /favicon.ico ................................................. ~ 0s
  2025-08-02 14:26:16 .............................................................. ~ 0s
  2025-08-02 14:26:17 /favicon.ico ................................................. ~ 0s
  2025-08-02 14:26:21 .............................................................. ~ 1s
  2025-08-02 14:26:21 /favicon.ico ................................................. ~ 1s
  2025-08-02 14:26:24 .............................................................. ~ 1s
  2025-08-02 14:26:25 /favicon.ico ................................................. ~ 0s
  2025-08-02 14:26:27 .............................................................. ~ 0s
  2025-08-02 14:26:27 /favicon.ico ................................................. ~ 0s
  2025-08-02 14:41:56 .............................................................. ~ 0s
  2025-08-02 14:41:56 /favicon.ico ................................................. ~ 0s
  2025-08-02 14:42:04 .............................................................. ~ 0s
  2025-08-02 14:42:04 /favicon.ico ................................................. ~ 0s
  2025-08-02 14:42:09 .............................................................. ~ 0s
  2025-08-02 14:42:09 /favicon.ico ................................................. ~ 0s
  2025-08-02 14:42:15 .............................................................. ~ 1s
  2025-08-02 14:42:16 /favicon.ico ................................................. ~ 0s
  2025-08-02 14:42:22 .............................................................. ~ 1s
  2025-08-02 14:42:22 /favicon.ico ................................................. ~ 1s
  2025-08-02 14:42:24 .............................................................. ~ 1s
  2025-08-02 14:42:25 /favicon.ico ................................................. ~ 0s
  2025-08-02 14:45:07 .............................................................. ~ 0s
  2025-08-02 14:45:07 /favicon.ico ................................................. ~ 0s
  2025-08-02 14:45:08 .............................................................. ~ 1s
  2025-08-02 14:45:09 /favicon.ico ................................................. ~ 0s
  2025-08-02 15:52:32 .............................................................. ~ 1s
  2025-08-02 15:52:33 /favicon.ico ................................................. ~ 0s
  2025-08-02 15:52:34 .............................................................. ~ 1s
  2025-08-02 15:52:35 .............................................................. ~ 0s
  2025-08-02 15:52:35 /favicon.ico ................................................. ~ 0s
  2025-08-02 15:52:36 .............................................................. ~ 0s
  2025-08-02 15:52:36 .............................................................. ~ 0s
  2025-08-02 15:52:36 /favicon.ico ................................................. ~ 0s
  2025-08-02 15:52:37 .............................................................. ~ 0s
  2025-08-02 15:52:37 .............................................................. ~ 0s
  2025-08-02 15:52:37 /favicon.ico ................................................. ~ 0s
  2025-08-02 15:54:13 .............................................................. ~ 0s
  2025-08-02 15:54:13 /favicon.ico ................................................. ~ 0s
  2025-08-02 15:54:15 .............................................................. ~ 1s
  2025-08-02 15:54:16 .............................................................. ~ 0s
  2025-08-02 15:54:16 /favicon.ico ................................................. ~ 0s
  2025-08-02 15:54:16 .............................................................. ~ 1s
  2025-08-02 15:54:16 .............................................................. ~ 1s
  2025-08-02 15:54:17 /favicon.ico ................................................. ~ 0s
  2025-08-02 15:54:38 .............................................................. ~ 0s
  2025-08-02 15:54:38 /favicon.ico ................................................. ~ 0s
  2025-08-02 15:54:39 .............................................................. ~ 2s
  2025-08-02 15:54:41 /favicon.ico ................................................. ~ 0s
  2025-08-02 15:55:36 .............................................................. ~ 0s
  2025-08-02 15:55:36 /favicon.ico ................................................. ~ 0s
  2025-08-02 15:55:38 .............................................................. ~ 0s
  2025-08-02 15:55:38 /favicon.ico ................................................. ~ 0s
  2025-08-02 15:55:40 .............................................................. ~ 0s
  2025-08-02 15:55:40 /favicon.ico ................................................. ~ 0s
  2025-08-02 15:58:00 .............................................................. ~ 0s
  2025-08-02 15:58:00 /favicon.ico ................................................. ~ 0s
  2025-08-02 15:58:03 .............................................................. ~ 0s
  2025-08-02 15:58:03 /favicon.ico ................................................. ~ 0s
  2025-08-02 15:58:05 .............................................................. ~ 1s
  2025-08-02 15:58:06 /favicon.ico ................................................. ~ 0s
  2025-08-02 15:58:07 .............................................................. ~ 0s
  2025-08-02 15:58:07 .............................................................. ~ 1s
  2025-08-02 15:58:08 /favicon.ico ................................................. ~ 0s
  2025-08-02 15:58:09 .............................................................. ~ 0s
  2025-08-02 15:58:09 .............................................................. ~ 0s
  2025-08-02 15:58:09 /favicon.ico ................................................. ~ 0s
  2025-08-02 15:58:11 /favicon.ico ................................................. ~ 0s
  2025-08-02 15:58:11 /favicon.ico ................................................. ~ 1s
  2025-08-02 15:58:12 /favicon.ico ................................................. ~ 1s
  2025-08-02 15:58:17 .............................................................. ~ 0s
  2025-08-02 15:58:17 .............................................................. ~ 0s
  2025-08-02 15:58:17 /favicon.ico ................................................. ~ 0s
  2025-08-02 15:58:21 .............................................................. ~ 0s
  2025-08-02 15:58:21 /favicon.ico ................................................. ~ 0s
  2025-08-02 15:59:30 .............................................................. ~ 0s
  2025-08-02 15:59:30 /favicon.ico ................................................. ~ 0s

   INFO  Environment modified. Restarting server...

   INFO  Server running on [http://127.0.0.1:8000].

  Press Ctrl+C to stop the server

  2025-08-02 17:09:32 .............................................................. ~ 0s
  2025-08-02 17:09:33 .............................................................. ~ 0s
  2025-08-02 17:09:33 /favicon.ico ................................................. ~ 0s
  2025-08-02 17:09:42 .............................................................. ~ 4s
  2025-08-02 17:09:46 /build/assets/app-385ab86b.css ............................... ~ 0s
  2025-08-02 17:09:46 /build/assets/app-4ba226a4.js ................................ ~ 0s
  2025-08-02 17:09:46 /favicon.ico ................................................. ~ 0s
  2025-08-02 17:11:49 .............................................................. ~ 0s
  2025-08-02 17:11:49 .............................................................. ~ 0s
  2025-08-02 17:11:49 /build/assets/app-385ab86b.css ............................... ~ 0s
  2025-08-02 17:11:49 /build/assets/app-4ba226a4.js ................................ ~ 0s
  2025-08-02 17:11:49 /favicon.ico ................................................. ~ 0s
  2025-08-02 17:12:02 .............................................................. ~ 1s
  2025-08-02 17:12:03 .............................................................. ~ 3s
  2025-08-02 17:12:06 /build/assets/app-385ab86b.css ............................... ~ 0s
  2025-08-02 17:12:06 /build/assets/app-4ba226a4.js ................................ ~ 0s
  2025-08-02 17:12:06 /favicon.ico ................................................. ~ 0s
  2025-08-02 17:13:25 .............................................................. ~ 1s
  2025-08-02 17:13:25 .............................................................. ~ 1s
  2025-08-02 17:13:26 /favicon.ico ................................................. ~ 0s
  2025-08-02 17:30:42 .............................................................. ~ 0s
  2025-08-02 17:30:42 /favicon.ico ................................................. ~ 0s
  2025-08-02 21:42:37 .............................................................. ~ 4s
  2025-08-02 21:42:41 /build/assets/app-385ab86b.css ............................... ~ 0s
  2025-08-02 21:42:41 /build/assets/app-4ba226a4.js ................................ ~ 0s
  2025-08-02 21:42:41 /favicon.ico ................................................. ~ 0s
  2025-08-02 21:42:56 .............................................................. ~ 1s
  2025-08-02 21:42:56 .............................................................. ~ 1s
  2025-08-02 21:42:57 /favicon.ico ................................................. ~ 0s
  2025-08-02 21:43:00 .............................................................. ~ 0s
  2025-08-02 21:43:00 /build/assets/app-385ab86b.css ............................... ~ 0s
  2025-08-02 21:43:00 /build/assets/app-4ba226a4.js ................................ ~ 0s
  2025-08-02 21:43:00 /favicon.ico ................................................. ~ 0s
  2025-08-02 21:43:13 .............................................................. ~ 0s
  2025-08-02 21:43:13 .............................................................. ~ 1s
  2025-08-02 21:43:13 /favicon.ico ................................................. ~ 1s
  2025-08-02 21:43:15 .............................................................. ~ 1s
  2025-08-02 21:43:15 /build/assets/app-385ab86b.css ............................... ~ 1s
  2025-08-02 21:43:16 /build/assets/app-4ba226a4.js ................................ ~ 0s
  2025-08-02 21:43:16 /favicon.ico ................................................. ~ 0s
  2025-08-02 21:43:23 .............................................................. ~ 1s
  2025-08-02 21:43:23 .............................................................. ~ 1s
  2025-08-02 21:43:24 /build/assets/app-385ab86b.css ............................... ~ 0s
  2025-08-02 21:43:24 /build/assets/app-4ba226a4.js ................................ ~ 0s
  2025-08-02 21:43:24 /favicon.ico ................................................. ~ 0s
  2025-08-02 21:44:18 .............................................................. ~ 0s
  2025-08-02 21:44:18 /build/assets/app-385ab86b.css ............................... ~ 0s
  2025-08-02 21:44:18 /build/assets/app-4ba226a4.js ................................ ~ 0s
  2025-08-02 21:44:19 /favicon.ico ................................................. ~ 0s
  2025-08-02 21:44:40 .............................................................. ~ 1s
  2025-08-02 21:44:41 /build/assets/app-385ab86b.css ............................... ~ 0s
  2025-08-02 21:44:41 /build/assets/app-4ba226a4.js ................................ ~ 0s
  2025-08-02 21:44:41 /favicon.ico ................................................. ~ 0s
  2025-08-02 21:44:56 .............................................................. ~ 1s
  2025-08-02 21:44:57 /build/assets/app-385ab86b.css ............................... ~ 0s
  2025-08-02 21:44:57 /build/assets/app-4ba226a4.js ................................ ~ 0s
  2025-08-02 21:44:57 /favicon.ico ................................................. ~ 0s
  2025-08-02 21:45:01 .............................................................. ~ 1s
  2025-08-02 21:45:02 /build/assets/app-385ab86b.css ............................... ~ 0s
  2025-08-02 21:45:02 /build/assets/app-4ba226a4.js ................................ ~ 0s
  2025-08-02 21:45:02 /favicon.ico ................................................. ~ 0s
  2025-08-02 21:45:34 .............................................................. ~ 1s
  2025-08-02 21:45:34 /favicon.ico ................................................. ~ 2s
  2025-08-02 21:45:45 .............................................................. ~ 1s
  2025-08-02 21:45:45 /favicon.ico ................................................. ~ 1s
  2025-08-02 21:45:53 .............................................................. ~ 1s
  2025-08-02 21:45:53 /favicon.ico ................................................. ~ 2s
  2025-08-02 21:46:00 .............................................................. ~ 1s
  2025-08-02 21:46:01 /build/assets/app-385ab86b.css ............................... ~ 0s
  2025-08-02 21:46:01 /build/assets/app-4ba226a4.js ................................ ~ 0s
  2025-08-02 21:46:01 /favicon.ico ................................................. ~ 0s
  2025-08-02 21:46:17 .............................................................. ~ 1s
  2025-08-02 21:46:17 /build/assets/app-385ab86b.css ............................... ~ 1s
  2025-08-02 21:46:18 /build/assets/app-4ba226a4.js ................................ ~ 0s
  2025-08-02 21:46:18 /favicon.ico ................................................. ~ 0s
  2025-08-02 21:46:57 .............................................................. ~ 0s
  2025-08-02 21:46:57 /build/assets/app-385ab86b.css ............................... ~ 0s
  2025-08-02 21:46:57 /build/assets/app-4ba226a4.js ................................ ~ 0s
  2025-08-02 21:46:58 /favicon.ico ................................................. ~ 0s

   INFO  Environment modified. Restarting server...

   INFO  Server running on [http://127.0.0.1:8000].

  Press Ctrl+C to stop the server


   INFO  Environment modified. Restarting server...

   INFO  Server running on [http://127.0.0.1:8000].

  Press Ctrl+C to stop the server


   INFO  Environment modified. Restarting server...

   INFO  Server running on [http://127.0.0.1:8000].

  Press Ctrl+C to stop the server


   INFO  Environment modified. Restarting server...

   INFO  Server running on [http://127.0.0.1:8000].

  Press Ctrl+C to stop the server


   INFO  Environment modified. Restarting server...

   INFO  Server running on [http://127.0.0.1:8000].

  Press Ctrl+C to stop the server


   INFO  Environment modified. Restarting server...

   INFO  Server running on [http://127.0.0.1:8000].

  Press Ctrl+C to stop the server


   INFO  Environment modified. Restarting server...

   INFO  Server running on [http://127.0.0.1:8000].

  Press Ctrl+C to stop the server

  2025-08-02 22:00:37 .............................................................. ~ 0s
  2025-08-02 22:00:37 .............................................................. ~ 0s
  2025-08-02 22:00:37 /build/assets/app-385ab86b.css ............................... ~ 0s
  2025-08-02 22:00:37 /build/assets/app-4ba226a4.js ................................ ~ 0s
  2025-08-02 22:00:38 /favicon.ico ................................................. ~ 0s
  2025-08-02 22:00:41 .............................................................. ~ 2s
  2025-08-02 22:00:43 /build/assets/app-385ab86b.css ............................... ~ 0s
  2025-08-02 22:00:43 /build/assets/app-4ba226a4.js ................................ ~ 0s
  2025-08-02 22:00:43 /favicon.ico ................................................. ~ 0s
  2025-08-02 22:00:47 .............................................................. ~ 9s
  2025-08-02 22:00:56 .............................................................. ~ 0s
  2025-08-02 22:00:56 /build/assets/app-385ab86b.css ............................... ~ 0s
  2025-08-02 22:00:56 /build/assets/app-4ba226a4.js ................................ ~ 0s
  2025-08-02 22:00:56 /favicon.ico ................................................. ~ 0s
  2025-08-02 22:04:12 .............................................................. ~ 3s
  2025-08-02 22:04:15 /build/assets/app-385ab86b.css ............................... ~ 0s
  2025-08-02 22:04:15 /build/assets/app-4ba226a4.js ................................ ~ 0s
  2025-08-02 22:04:17 /favicon.ico ................................................. ~ 0s
  2025-08-02 22:10:00 .............................................................. ~ 1s
  2025-08-02 22:10:01 .............................................................. ~ 0s
  2025-08-02 22:10:01 /build/assets/app-385ab86b.css ............................... ~ 0s
  2025-08-02 22:10:01 /build/assets/app-4ba226a4.js ................................ ~ 0s
  2025-08-02 22:10:01 /favicon.ico ................................................. ~ 0s
  2025-08-02 22:12:23 .............................................................. ~ 0s
  2025-08-02 22:12:23 .............................................................. ~ 1s
  2025-08-02 22:12:24 /build/assets/app-385ab86b.css ............................... ~ 0s
  2025-08-02 22:12:24 /build/assets/app-4ba226a4.js ................................ ~ 0s
  2025-08-02 22:12:24 /favicon.ico ................................................. ~ 0s
  2025-08-02 22:20:18 .............................................................. ~ 1s
  2025-08-02 22:20:18 /favicon.ico ................................................. ~ 1s
  2025-08-02 22:20:20 .............................................................. ~ 1s
  2025-08-02 22:20:21 /build/assets/app-385ab86b.css ............................... ~ 0s
  2025-08-02 22:20:21 /build/assets/app-4ba226a4.js ................................ ~ 0s
  2025-08-02 22:20:21 /favicon.ico ................................................. ~ 0s
  2025-08-02 22:20:48 .............................................................. ~ 5s
  2025-08-02 22:20:53 .............................................................. ~ 0s
  2025-08-02 22:20:53 .............................................................. ~ 1s
  2025-08-02 22:20:54 /build/assets/app-385ab86b.css ............................... ~ 0s
  2025-08-02 22:20:54 /build/assets/app-4ba226a4.js ................................ ~ 0s
  2025-08-02 22:20:54 /favicon.ico ................................................. ~ 0s
  2025-08-02 22:21:29 .............................................................. ~ 0s
  2025-08-02 22:21:29 .............................................................. ~ 0s
  2025-08-02 22:21:29 /build/assets/app-385ab86b.css ............................... ~ 0s
  2025-08-02 22:21:29 /build/assets/app-4ba226a4.js ................................ ~ 0s
  2025-08-02 22:21:30 /favicon.ico ................................................. ~ 0s
  2025-08-02 22:21:39 .............................................................. ~ 0s
  2025-08-02 22:21:39 .............................................................. ~ 1s
  2025-08-02 22:21:40 /build/assets/app-385ab86b.css ............................... ~ 0s
  2025-08-02 22:21:40 /build/assets/app-4ba226a4.js ................................ ~ 0s
  2025-08-02 22:21:40 /favicon.ico ................................................. ~ 0s
  2025-08-02 22:51:06 .............................................................. ~ 1s
  2025-08-02 22:51:07 .............................................................. ~ 0s
  2025-08-02 22:51:07 /favicon.ico ................................................. ~ 0s
  2025-08-02 22:51:09 .............................................................. ~ 0s
  2025-08-02 22:51:09 /logo/logo.jpg ............................................... ~ 0s
  2025-08-02 22:51:09 /build/assets/app-385ab86b.css ............................... ~ 0s
  2025-08-02 22:51:09 /build/assets/app-4ba226a4.js ................................ ~ 0s
  2025-08-02 22:51:10 /favicon.ico ................................................. ~ 0s
  2025-08-02 22:51:15 /logo/logo.jpg ............................................... ~ 0s
  2025-08-02 22:51:15 /favicon.ico ................................................. ~ 0s
  2025-08-02 22:51:15 ............................................................. ~ 14s
  2025-08-02 22:51:29 /build/assets/app-385ab86b.css ............................... ~ 0s
  2025-08-02 22:51:29 /build/assets/app-4ba226a4.js ................................ ~ 0s
  2025-08-02 22:51:29 /logo/logo.jpg ............................................... ~ 0s
  2025-08-02 22:51:29 /favicon.ico ................................................. ~ 0s
  2025-08-02 22:51:36 .............................................................. ~ 1s
  2025-08-02 22:51:37 /build/assets/app-385ab86b.css ............................... ~ 0s
  2025-08-02 22:51:37 /build/assets/app-4ba226a4.js ................................ ~ 0s
  2025-08-02 22:51:37 /logo/logo.jpg ............................................... ~ 0s
  2025-08-02 22:51:37 /favicon.ico ................................................. ~ 0s
  2025-08-02 22:51:54 .............................................................. ~ 0s
  2025-08-02 22:51:54 /build/assets/app-385ab86b.css ............................... ~ 0s
  2025-08-02 22:51:54 /build/assets/app-4ba226a4.js ................................ ~ 0s
  2025-08-02 22:51:54 /logo/logo.jpg ............................................... ~ 0s
  2025-08-02 22:51:54 /favicon.ico ................................................. ~ 0s
  2025-08-02 22:52:07 .............................................................. ~ 1s
  2025-08-02 22:52:08 .............................................................. ~ 0s
  2025-08-02 22:52:08 /build/assets/app-385ab86b.css ............................... ~ 0s
  2025-08-02 22:52:08 /build/assets/app-4ba226a4.js ................................ ~ 0s
  2025-08-02 22:52:08 /logo/logo.jpg ............................................... ~ 0s
  2025-08-02 22:52:08 /favicon.ico ................................................. ~ 0s
  2025-08-02 22:52:23 .............................................................. ~ 0s
  2025-08-02 22:52:23 /build/assets/app-385ab86b.css ............................... ~ 0s
  2025-08-02 22:52:23 /build/assets/app-4ba226a4.js ................................ ~ 0s
  2025-08-02 22:52:23 /logo/logo.jpg ............................................... ~ 0s
  2025-08-02 22:52:23 /favicon.ico ................................................. ~ 0s
  2025-08-02 22:52:35 .............................................................. ~ 0s
  2025-08-02 22:52:35 /build/assets/app-385ab86b.css ............................... ~ 0s
  2025-08-02 22:52:35 /build/assets/app-4ba226a4.js ................................ ~ 0s
  2025-08-02 22:52:35 /logo/logo.jpg ............................................... ~ 0s
  2025-08-02 22:52:36 /favicon.ico ................................................. ~ 0s
  2025-08-02 22:52:42 .............................................................. ~ 1s
  2025-08-02 22:52:42 /build/assets/app-385ab86b.css ............................... ~ 1s
  2025-08-02 22:52:43 /build/assets/app-4ba226a4.js ................................ ~ 0s
  2025-08-02 22:52:43 /logo/logo.jpg ............................................... ~ 0s
  2025-08-02 22:52:43 /favicon.ico ................................................. ~ 0s
  2025-08-02 23:11:28 ............................................................. ~ 17s
  2025-08-02 23:11:28 ............................................................. ~ 20s
  2025-08-02 23:11:48 /build/assets/app-385ab86b.css ............................... ~ 0s
  2025-08-02 23:11:48 /logo/logo.jpg ............................................... ~ 0s
  2025-08-02 23:11:48 /build/assets/app-4ba226a4.js ................................ ~ 0s
  2025-08-02 23:11:48 /favicon.ico ................................................. ~ 0s
