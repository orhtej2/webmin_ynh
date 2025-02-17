<!--
N.B.: This README was automatically generated by https://github.com/YunoHost/apps/tree/master/tools/README-generator
It shall NOT be edited by hand.
-->

# Webmin pour YunoHost

[![Niveau d’intégration](https://dash.yunohost.org/integration/webmin.svg)](https://dash.yunohost.org/appci/app/webmin) ![Statut du fonctionnement](https://ci-apps.yunohost.org/ci/badges/webmin.status.svg) ![Statut de maintenance](https://ci-apps.yunohost.org/ci/badges/webmin.maintain.svg)

[![Installer Webmin avec YunoHost](https://install-app.yunohost.org/install-with-yunohost.svg)](https://install-app.yunohost.org/?app=webmin)

*[Read this readme in english.](./README.md)*

> *Ce package vous permet d’installer Webmin rapidement et simplement sur un serveur YunoHost.
Si vous n’avez pas YunoHost, regardez [ici](https://yunohost.org/#/install) pour savoir comment l’installer et en profiter.*

## Vue d’ensemble

Webmin is a web-based interface for system administration for Unix. Using any modern web browser, you can setup user accounts, Apache, DNS, file sharing and much more. Webmin removes the need to manually edit Unix configuration files like `/etc/passwd`, and lets you manage a system from the console or remotely.

**Version incluse :** 2.013~ynh1

## Captures d’écran

![Capture d’écran de Webmin](./doc/screenshots/screenshot1.gif)

## Avertissements / informations importantes

* This app has **root** access which can change core things in the system, thus **breaking the YunoHost**. Use it carefully and read the [documents](https://doxfer.webmin.com/Webmin/Main_Page) two times before changing values.
* Only **user** given permission at time of the installation can **access** the Webmin login interface
* To login to webmin, use root and root password 
* Webmin will **update itself** when system updates are run. So no need to **run upgrade script** once installed.

### Fix username and password

If you can't connect you can fix the password of the user running:
```
/usr/share/webmin/changepass.pl /etc/webmin root newpassword
```

## Documentations et ressources

* Site officiel de l’app : <http://www.webmin.com>
* Dépôt de code officiel de l’app : <https://github.com/webmin/webmin>
* Documentation YunoHost pour cette app : <https://yunohost.org/app_webmin>
* Signaler un bug : <https://github.com/YunoHost-Apps/webmin_ynh/issues>

## Informations pour les développeurs

Merci de faire vos pull request sur la [branche testing](https://github.com/YunoHost-Apps/webmin_ynh/tree/testing).

Pour essayer la branche testing, procédez comme suit.

``` bash
sudo yunohost app install https://github.com/YunoHost-Apps/webmin_ynh/tree/testing --debug
ou
sudo yunohost app upgrade webmin -u https://github.com/YunoHost-Apps/webmin_ynh/tree/testing --debug
```

**Plus d’infos sur le packaging d’applications :** <https://yunohost.org/packaging_apps>