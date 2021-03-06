Light_QuickMailAlert
===========
2020-08-14 -> 2021-03-15



A [light](https://github.com/lingtalfi/Light) service to send quick email alerts to the admin.


This is a [Light plugin](https://github.com/lingtalfi/Light/blob/master/doc/pages/plugin.md).

This is part of the [universe framework](https://github.com/karayabin/universe-snapshot).


Install
==========
Using the [planet installer](https://github.com/lingtalfi/Light_PlanetInstaller) via [light-cli](https://github.com/lingtalfi/Light_Cli)
```bash
lt install Ling.Light_QuickMailAlert
```

Using the [uni](https://github.com/lingtalfi/universe-naive-importer) command.
```bash
uni import Ling/Light_QuickMailAlert
```

Or just download it and place it where you want otherwise.






Summary
===========
- [Light_QuickMailAlert api](https://github.com/lingtalfi/Light_QuickMailAlert/blob/master/doc/api/Ling/Light_QuickMailAlert.md) (generated with [DocTools](https://github.com/lingtalfi/DocTools))
- [Services](#services)
- Pages
    - [Conception notes](https://github.com/lingtalfi/Light_QuickMailAlert/blob/master/doc/pages/conception-notes.md)






Services
=========


Here is an example of the service configuration:

```yaml
quick_mail_alert:
    instance: Ling\Light_QuickMailAlert\Service\LightQuickMailAlertService
    methods:
        setContainer:
            container: @container()
        setOptions:
            options:
                appName: my app 01
        setGroups:
            groups:
                admin:
                    template: Ling.Light_QuickMailAlert/admin_alert
                    recipients:
                        - the_admin@gmail.com







```



History Log
=============

- 1.1.7 -- 2021-05-31

    - Removing trailing plus in lpi-deps file (to work with Light_PlanetInstaller:2.0.0 api

- 1.1.6 -- 2021-05-10

    - Fix assets missing.

- 1.1.5 -- 2021-03-15

    - update planet to adapt Ling.Light:0.70.0

- 1.1.4 -- 2021-03-09

    - update planet to adapt last Ling.Light_Mailer change
  
- 1.1.3 -- 2021-03-05

    - update README.md, add install alternative

- 1.1.2 -- 2020-12-08

    - Fix lpi-deps not using natsort.

- 1.1.1 -- 2020-12-04

    - Add lpi-deps.byml file

- 1.1.0 -- 2020-08-17

    - add admin_notif template
    
- 1.0.0 -- 2020-08-14

    - initial commit