# Docker RSS Feed Validator Instance with modifications for validation of INSPIRE Download Services based on Atom Feed

Installs and runs an instance of http://validator.w3.org/feed/ from the source
tree at https://github.com/bor8/feedvalidator.git

# Scope
This feedvalidator includes modifications to support validation of [INSPIRE Download Services based on Atom Feed](http://inspire.ec.europa.eu/documents/technical-guidance-implementation-inspire-download-services "Technical Guidance for the implementation of INSPIRE Download Services") as used by [GDI-DE Testsuite](http://www.geoportal.de/EN/GDI-DE/Components/GDI-DE-Testsuite/gdi-de-testsuite.html?lang=en "GDI-DE Testsuite").

**Use this docker feed validator instance only in context of GDI-DE Testsuite and INSPIRE Download Services based on Atom Feed. For all other purposes  use this docker feed validator: ** [feed validator docker image by Unboxed Consulting](https://github.com/unboxed/docker-feed-validator )   
  
# Usage

```sh
$ sudo docker run -d -p 8080:80 doemming/feedvalidator
```

Options:

* "-d" Runs in the background
* "-p 8080:80" Redirects port 8080 on the docker host to port 80 on the container.

Once you have run the above command, connect to your Docker server on port 8080
with a url like http://dockerserver.example:8080/feedvalidator

# Queries

Please raise issues on the project GitHub page.

# Build Process

```shell
$ ./build.sh
```

# Thanks

Thanks go to [bor8](https://github.com/bor8) for providing feed validator modifications to support validation of INSPIRE Download Services based on Atom Feed.

Thanks go to [Unboxed Consulting](https://github.com/unboxed/docker-feed-validator) for their Docker instance of http://validator.w3.org/feed/ .
  
Thanks go to [Dan Pupius](https://medium.com/dev-tricks/apache-and-php-on-docker-44faef716150)
for his Apache config files from his blog.

Additional thanks go to
[magnetikonline/html5validator](https://registry.hub.docker.com/u/magnetikonline/html5validator/)
for further Apache config options, and his related HTML5 validator Docker
instance.

# License

MIT License - please see the project LICENSE file for details.

# Maintenance
This docker instance is maintained by [bespire UG](http://www.bespire.de)
