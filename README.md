# siacoin.com

The source for the website, [siacoin.com](http://siacoin.com).

### Configuration
The web site is hosted on a linode instance, and the root of this get
repositiory is located at `/srv/www/siacoin.com`. As a web server,
nginx is installed, and the web root for siacoin.com requests is
`/srv/www/siacoin.com/public_html`.

Github web hooks are used to automatically keep the web site up to
date with the git repository, and the server that handles this is
running inside of a tmux session and holds port 29989 open. This
listener also automically updates the Sia-Block-Explorer repository,
which is running on the same linode instance.
