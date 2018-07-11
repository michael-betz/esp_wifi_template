# Bare bones webserver template

__includes__

  * httpd webserver with basic website
  * Web debugging console
  * settings.json
  * html editor for settings.json
  * NTP time

# Write settings file to spiffs

```bash
curl --data-binary @spiffs_data/settings.json http://192.168.4.1/S/settings.json
```

Once the web-server is up,s ettings.js can be edited in browser.

# Remote flash

```bash
make web-flash
```

Edit `Makefile` and add your hostname!
