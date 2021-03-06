.. _installation:

Installation
============

Installing on Windows
---------------------

There are 2 Un-Official PocketMine-MP Installers by TheDeibo Click either x64, or x86 to download your chosen one.

- One for `x64 <https://github.com/thedeibo/Windows-PocketMine-MP/raw/master/PocketMine-MP-x64.exe>`_
- One for `x86 <https://github.com/thedeibo/Windows-PocketMine-MP/raw/master/PocketMine-MP-x86.exe>`_
You can also download the latest .phar from `Bintray <https://bintray.com/pocketmine/PocketMine/PocketMine-MP-phar/view#files>`_.
These installers provide you with the files you need to make a server!

But what if I have forgotten/don't know my Windows OS?
Not to worry. We have got that covored! Simply follow these steps:

1. `Go on the PMMPInstaller file, <https://raw.githubusercontent.com/NotPocketMine/Windows-PocketMine-MP/master/pmmpinstaller.bat>`_
2. Copy it into Notepad, and save it to your chosen location. (It's Recommended to put it on Desktop)
3. Run the file. (By double clicking it.)
4. The PMMPInstaller.bat will download a exe from the internet, which will give you the correct version of PocketMine-MP-x.exe.

The Installers:
---------------

These installers will provide you with these folders and files:

1. /bin (And ALL its files inside)
2. /start.cmd
3. PocketMine-MP.phar

You will also need to download this.

`https://www.microsoft.com/en-gb/download/details.aspx?id=48145 <https://www.microsoft.com/en-gb/download/details.aspx?id=48145>`_
Please use the correct version, else the server may not work. It supplies the essential code for running the server. Without it, You will recieve an error, and would not be able to run the server, and would recieve this error

.. code-block:: winerror1

	/usr/bin/php/php.exe: error while loading shared libraries: ?:
	cannot open shared object file: No such file or directory
	
	bin\php\php.exe: Exit 127
	

If you have recieved this error:

.. code-block:: winerror2

	/usr/bin/php/php.exe: error while loading shared libraries: api-ms-win-crt-locale-l1-1-0.dll: cannot open shared object file: 
	No such file or directory
	
	bin\php\php.exe: Exit 127
	

Then, you'll need to download the correct version of this, `https://support.microsoft.com/en-us/kb/2999226 <https://support.microsoft.com/en-us/kb/2999226>`_

For more information about the installer, or how to fix some errors, please `CLICK HERE <https://forums.pocketmine.net/threads/pocketmine-1-6-php7-installer-windows.15493/>`_



Updating the Server
-------------------

Did the installer fail? It is not your taste? You cah do it your self!

Using .phar
~~~~~~~~~~~

1. Create a new directory for PocketMine-MP.
2. Download PocketMine-MP.phar from `Jenkins Website <https://jenkins.pmmp.io/job/PocketMine-MP/lastSuccessfulBuild/>`_.
3. Rename the .phar to ``PocketMine-MP.phar``.
4. Place it in the PocketMine-MP directory you just created.



Starting for the first time
---------------------------

Now you should be able to start PocketMine-MP.
The first time it starts with a set-up wizard,
this can be disabled by running ``./start.sh --no-wizard``.

.. code::

    $ ./start.sh
    [*] PocketMine-MP set-up wizard
    [*] Please select a language:
    English => en
    Español => es
    中文 => zh
    Pусский => ru
    日本語 => ja
    Deutsch => de
    한국어 => ko
    Nederlands => nl
    Français  => fr
    Italiano => it
    Melayu => ms
    Norsk => no
    Svenska => sv
    Suomi => fi
    Türkçe => tr
    [?] Language (en):

PocketMine-MP supports a few other languages.
Fill in the two letters behind the language and press enter.
Is your language not in the list? Add it on `Crowdin`_.

.. code::

    [*] English has been correctly selected.
    Welcome to PocketMine-MP!
    Before starting setting up your new server you have to accept the license.
    PocketMine-MP is licensed under the LGPL License,
    that you can read opening the LICENSE file on this folder.

    This program is free software: you can redistribute it and/or modify
    it under the terms of the GNU Lesser General Public License as published by
    the Free Software Foundation, either version 3 of the License, or
    (at your option) any later version.

    [?] Do you accept the License? (y/N):

Do you accept the `License`_?

.. code::

    [?] Do you want to skip the set-up wizard? (y/N):

You can skip the wizard from here and start the server with the default settings or continue.

.. code::

    [*] You are going to set up your server now.
    [*] If you don't want to change the default value, just press Enter.
    [*] You can edit them later on the server.properties file.
    [?] Give a name to your server (Minecraft: PE Server):
    [*] Do not change the default port value if this is your first server.
    [?] Server port (19132):
    [*] The RAM is the maximum amount of memory PocketMine-MP will use. A value of 128-256 MB is recommended
    [?] Server RAM in MB (256):
    [*] Choose between Creative (1) or Survival (0)
    [?] Default Game mode: (0):
    [?] Max. online players (20):
    [*] The spawn protection disallows placing/breaking blocks in the spawn zone except for OPs
    [?] Enable spawn protection? (Y/n):
    [*] An OP is the player admin of the server. OPs can run more commands than normal players
    [?] OP player name (example, your game name):
    [!] You will be able to add an OP user later using /op <player>
    [*] The white-list only allows players in it to join.
    [?] Do you want to enable the white-list? (y/N):
    [!] Query is a protocol used by different tools to get information of your server and players logged in.
    [!] If you disable it, you won't be able to use server lists.
    [?] Do you want to disable Query? (y/N):
    [*] RCON is a protocol to remote connect with the server console using a password.
    [?] Do you want to enable RCON? (y/N):
    [*] Getting your external IP and internal IP
    [!] Your external IP is 87.212.35.149. You may have to port-forward to your internal IP 192.168.0.150
    [!] Be sure to check it, if you have to forward and you skip that, no external players will be able to join. [Press Enter]
    [*] You have finished the set-up wizard correctly
    [*] Check the Plugin Repository to add new features, minigames, or advanced protection to your server
    [*] PocketMine-MP will now start. Type /help to view the list of available commands.

    [Server thread/INFO]: Loading pocketmine.yml...
    [Server thread/INFO]: Loading server properties...
    [Server thread/INFO]: Selected English (eng) as the base language
    [Server thread/INFO]: Starting Minecraft: PE server version v0.16.0.5 alpha
    [Server thread/INFO]: Opening server on 0.0.0.0:19132
    [Server thread/INFO]: This server is running PocketMine-MP version 1.6.1dev "Unleashed" (API 2.1.0)
    [Server thread/INFO]: PocketMine-MP is distributed under the LGPL License
    [Server thread/INFO]: Loading recipes...
    [Server thread/NOTICE]: Level "world" not found
    [Server thread/INFO]: Preparing level "world"
    [Server thread/NOTICE]: Spawn terrain for level "world" is being generated in the background
    [Server thread/INFO]: Starting GS4 status listener
    [Server thread/INFO]: Setting query port to 19132
    [Server thread/INFO]: Query running on 0.0.0.0:19132
    [Server thread/INFO]: Default game type: Survival Mode
    [Server thread/INFO]: Done (1.163s)! For help, type "help" or "?"
    
    
    
The server should have started now and you should be able to join

.. _Win-Bintray: https://bintray.com/pocketmine/PocketMine/Windows-PHP-Binaries/view#files
.. _GitHub: https://jenkins.pmmp.io/
.. _PHP-Bintray: https://jenkins.pmmp.io/
.. _PM-Stable: https://jenkins.pmmp.io/job/PocketMine-MP/lastSuccessfulBuild/
.. _PocketMine-MP for Android: https://play.google.com/store/apps/details?id=net.pocketmine.server
.. _Crowdin: http://translate.pocketmine.net
.. _License: https://github.com/pmmp/PocketMine-MP/blob/master/LICENSE
.. _Phar-Bintray: https://jenkins.pmmp.io/job/PocketMine-MP/lastSuccessfulBuild/
