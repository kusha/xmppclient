##XMPP/Jabber client with CLI and GUI.
---

Uses PLAIN auithorization method. Use at your own risks. Implements basics registration and authorization method. Can send and recieve messages. Also it's possible to work with roster.

	usage: xmppclient [-h] [--version] [-s server_name:port]
	                  [-r username:password] [-l username:password] [-c] [-a JID]
	                  [-m message] [-u JID] [-w ss] [-i]

	-h, --help            show this help message and exit
	--version             show program's version number and exit
	-s server_name:port, --server server_name:port
	                      specifis XMPP server address
	-r username:password, --register-user username:password
	                      register new user
	-l username:password, --log-user username:password
	                      login as a user
	-c, --show-contactlist
	                      show user contact list
	-a JID, --add-user JID
	                      adds user to contact list
	-m message, --message message
	                      specify message text
	-u JID, --user JID    specify JID of a recipient
	-w ss, --wait ss      wait for response ss seconds before exit
	-i, --interactive     enables interactive mode

###Usage examples:

	./xmppclient -s netfox.fit.vutbr.cz:5222 -r xlogin00:pass
	./xmppclient -s netfox.fit.vutbr.cz:5222 -l xlogin00:pass -c -a xlogin01@netfox.fit.vutbr.cz
	./xmppclient -s netfox.fit.vutbr.cz:5222 -l xlogin00:pass -m "testovaci zprava" -u xlogin01@netfox.fit.vutbr.cz
	./xmppclient -s netfox.fit.vutbr.cz:5222 -r xlogin00:pass -l xlogin00:pass -w 60
	./xmppclient -s netfox.fit.vutbr.cz:5222 -l xlogin00:pass  -u xlogin01@netfox.fit.vutbr.cz -i

Use `init.sh` to install Tkinter, and set permissions.

`manual.pdf` contains documentation in Czech language.

*Mark Birger (xbirge00)*

*8 October 2014 - 30 October 2014*