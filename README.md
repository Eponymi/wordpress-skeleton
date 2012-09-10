WordPress Skeleton
==================

WordPress skeleton utilizing [Vagrant][1], [Composer][2], [_s][3], & [Wordpress][5].


Geting Started
--------------

1. Download & Install [Vagrant][1]

2. Install Dependencies via `./bin/install`.  This will install [Vagrant Hostmaster][6], [Composer][2], [WordPress][5] & other dependencies.

3. Setup your skeleton via `./bin/console skeleton:generate` & follw the prompts.

4. Start the development VM via `vagrant up`.

5. Create the deployment structure via `cap develop deploy:setup`.

6. Start your development environment via `cap develop deploy`.

7. **Done**!

Open <http://vagrant.[domain]/> in your browser, make changes to your theme in `/src` & refresh!


Deploying
---------

### Staging

    $ cap staging deploy:setup

_You only need to setup the deployment structure once._

    $ cap staging deploy


### Production

    $ cap production deploy:setup
    $ cap production deploy



[1]: http://vagrantup.com/
[2]: http://getcomposer.org/
[3]: http://underscores.me/
[5]: http://github.com/WordPress/WordPress
[6]: http://github.com/mosaicxm/vagrant-hostmaster
[7]: http://getcomposer.org/doc/00-intro.md#globally
[8]: http://codex.wordpress.org/Theme_Unit_Test
