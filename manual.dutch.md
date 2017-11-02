# Algemene werkwijze

Na start/herstart van je Mac zijn (afhankelijk van je setup) Apache en MySQL al meteen actief.
In mijn geval moet ik de ontwikkelomgeving handmatig starten. Ik open een Terminal en start de servers:

```
$ startdevelopment
```

Apache en MySQL zijn nu klaar voor gebruik.

# Nieuwe database aanmaken

- Een nieuwe database aanmaken doe je via phpMyAdmin door in je browser te gaan naar http://phpmyadmin.dev
- Klik op **Databases** en vul onder Create database de naam van je database in en klik op Create.
- De database is dan klaar voor gebruik. Gebruikersnaam en wachtwoord is **root**.

# Nieuwe website aanmaken

Een nieuwe website aanmaken is zeer eenvoudig. Maak simpel in je Sites map een nieuwe submap aan voor de website.
Als voorbeeld maken we een website aan **testwebsite**.

```
$ mkdir ~/Development/Sites/testwebsite
```

Plaats daarna de website bestanden in de map ~/Development/Sites/testwebsite.

Je hoeft dan verder niets meer aan te passen. De website is direct in je browser benaderbaar via http://testwebsite.dev

# Development stoppen

MySQL en Apache kunnen eenvoudig gestop worden met het terminal commando:

```
$ startdevelopment
```

# Handige commando's:

## Apache

Start apache bij elke (re)boot:

```
$ sudo brew services start httpd
```

Stop apache bij elke (re)boot:

```
$ sudo brew services stop httpd
```

Start apache:

```
$ sudo apachectl start
```

Stop apache:

```
$ sudo apachectl stop
```

Herstart apache:

```
$ sudo apachectl -k restart
```

Edit httpd.conf:

```
$ open -e /usr/local/etc/httpd/httpd.conf
```

Controleer of Apache actief is:

```
$ ps -aef | grep httpd
```

# PHP

Edit php.ini 5.3:

```
$ open -e /usr/local/etc/php/5.3/php.ini
```

Edit php.ini 5.6:

```
$ open -e /usr/local/etc/php/5.6/php.ini
```

Edit php.ini 7.0:

```
$ open -e /usr/local/etc/php/7.0/php.ini
```

Edit php.ini 7.1:

```
$ open -e /usr/local/etc/php/7.1/php.ini
```

Wissel naar php 5.3:

```
$ sphp 53
```

Wissel naar php 5.6:

```
$ sphp 56
```

Wissel naar php 7.0:

```
$ sphp 70
```

Wissel naar php 7.1:

```
$ sphp 71
```

# MySQL

Start mysql na elke (re)boot:

```
$ brew services start mysql
```

Stop mysql na elke (re)boot:

```
$ brew services stop mysql
```

Congtroleer of MySQL actief is:

```
$ ps -aef | grep mysql
```