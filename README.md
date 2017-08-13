# docker-phusion-laravel-build
Laravel CI environment

To build:
docker build -t ozkaa/laravel-build .

To run Unit tests
docker run -it --volume=/Users/oscarfrowijn/PhpstormProjects/staff-dir-change/:/app --workdir="/app" ozkaa/laravel-build phpunit

Where volume = staffdir volume

PHPunit is run automatically and output should be:

PHPUnit 5.7.21 by Sebastian Bergmann and contributors.

.......                                                             7 / 7 (100%)

Time: 4.56 seconds, Memory: 78.00MB

OK (7 tests, 12 assertions)

