# Learn-TheDevilBox

1.  https://deliciousbrains.com/devilbox-local-wordpress-development-docker/

    a.  $ git clone https://github.com/cytopia/devilbox
        $ cd devilbox/
        $ cp env-example .env
        $ ./update-docker.sh
        $ docker-compose up -d
        $ docker-compose ps

    b.  http://localhost # The Dashboard of The Devil Box

2.  https://devilbox.readthedocs.io/en/latest/examples/setup-wordpress.html

    a.  $ ./shell.sh

    b.  devilbox@php-7.0.20 in /shared/httpd $ mkdir gatsbywp2

    c.  devilbox@php-7.0.20 in /shared/httpd $ cd my-wp

    d.  devilbox@php-7.0.20 in /shared/httpd/my-wp $ git clone https://github.com/WordPress/WordPress wordpress.git

    e.  devilbox@php-7.0.20 in /shared/httpd/my-wp $ ln -s wordpress.git/ htdocs # symlink webroot

    f.  add an entry into /etc/hosts
        127.0.0.1 my-wp.loc

    g.  http://my-wp.loc # The Wordpress website version 4.9.5