# dropbox with systemd

This is a systemd service file to start up dropbox on a per user basis on boot.

This assumes each user installed dropbox headless via the command line: https://www.dropbox.com/en/install?os=lnx and has setup his/her account such that running dropboxd manually works.

* Place the dropbox@.service file into /etc/systemd/system
* Reload the daemons: systemctl daemon-reload
* Enable the service for users: systemctl enable dropbox@username
* Start service: systemctl start dropbox@username
