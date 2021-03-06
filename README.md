### About project

Configuration of Ubuntu server for hosting a Python web application.

### Platform

Lightsail (Amazon Web Services)

### How to connect server

- IP Address: `35.159.25.149`

- Port `2200` instead of `22`

- SSH Key

- Grader user (server-side key is located in user default path)

### About application

- Application repository: [Games Catalog](https://github.com/Helsh/gamecatalog)

- Application with working Google OAuth: http://35.159.25.149.xip.io/

- WSGi to handle more requests

### Apache configuration

- Application located in `/var/www`

- Logs located in `/var/log/apache2`

- Add `FlaskApp.conf` which specify `ServerName`, `WSGIScriptAlias`, paths to application directories and path to logs.

- Changed ownership to `www-data` for `/var/www`

### PIP packages installed on server:

- Flask

- SQLAlchemy

- Httplib2

- OAuth2Client

- Psycopg2

- Urllib3

### Ubuntu packages installed on server:

- Ufw

- Apache2

- Finger

## Third-party resources:

- Google OAuth

- DNS Wildcard (xip.io)