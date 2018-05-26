# Learn-TheDevilBox

0.  Install Docker for Mac at https://docs.docker.com/docker-for-mac/

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

    c.  devilbox@php-7.0.20 in /shared/httpd $ cd gatsbywp2

    d.  devilbox@php-7.0.20 in /shared/httpd/gatsbywp2 $ git clone https://github.com/WordPress/WordPress wordpress.git

    e.  devilbox@php-7.0.20 in /shared/httpd/gatsbywp2 $ ln -s wordpress.git/ htdocs # symlink webroot

    f.  add an entry into /etc/hosts

        ## DevilBox - Start ##
        127.0.0.1 gatsbywp2.loc #Local Site
        127.0.0.1 www.gatsbywp2.loc #Local Site
        ## DevilBox - End #

    g.  Install the database using The Devil Box Dashboard | Tools | phpMyAdmin | user root, password <blank>

        Create new user gatsbywp2 password gatsbywp2 database gatsbywp2
    
    h.  http://gatsbywp2.loc # Install The Wordpress website version 4.9.5

    i.  username 20yXq4ffMM8eKc4zw password c4zffMw4qM8eKf)fM2ffM0yX email thomasperdana@gmail.com