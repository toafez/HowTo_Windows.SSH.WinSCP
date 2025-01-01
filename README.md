[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Ftoafez%2FHowTo_Windows.SSH.WinSCP&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://hits.seeyoufarm.com)

# HowTo: SSH-Key mit WinSCP für Windows

## Worum geht es?
Die folgende Anleitung baut auf meiner Anleitung [HowTo: SSH-Key mit PuTTY und PuTTYgen](https://github.com/toafez/HowTo_Windows.SSH.PuTTY.PuTTYgen) auf, in der bereits eine passwortfreie SSH-Public-Key-Authentifizierung von einem lokalen Linux-System zu einem entfernten Linux-Server beschrieben wurde. **Durch die Einbindung des** bereits mit PuTTYgen erzeugten **privaten Schlüssels in das Windows-Programm WinSCP kann** auch hier **ein passwortfreier Zugriff auf einen entfernten Linux-Server erfolgen**.

## WinSCP installieren
Das Programm WinSCP kann als Windows-Installer von der [WinSCP Download-Seite](https://winscp.net/eng/download.php) heruntergeladen werden.

## WinSCP öffnen
1. Starte **WinSCP** aus der Liste der Windows-Programme.
2. Wähle im linken Abschnitt **Sitzung /Übertragungsprotokoll** den Punkt **SCP** aus dem Aufklappmenü aus.
3. Gib in den Abschnitten **Session / Server Address** und **Port Number** die IP-Adresse des Remote-Servers ein, mit dem du dich verbinden möchtest und passe ggf. den zu verwendenden Port an. In diesem Beispiel wird die IP-Adresse 172.16.1.12 und der Port 22 verwendet.
4.  Gib im Abschnitt **Session / Benutzername** den Benutzernamen ein, mit dem du dich auf dem Remote-Server anmelden möchtest. In diesem Beispiel wird der Superuser **root** verwendet.
5. Klicke auf die Schaltfläche **Erweitert**

    ![01_WinSCP_Configuration](/images/01_WinSCP_Configuration.png)

6. Wähle im rechten Abschnitt **SSH / Authentifizierung** und klicke dann im rechten Bereich **Authentifizierungsparameter / Datei mit privatem Schlüssel:** auf die gelb markierte Schaltfläche, um im Dateisystem nach dem privaten Schlüssel zu suchen, den du bereits nach meiner Anleitung [HowTo: SSH-Key mit PuTTY und PuTTYgen](https://github.com/toafez/HowTo_Windows.SSH.PuTTY.PuTTYgen) erstellt und an einem sicheren Ort gespeichert hast.

    ![02_WinSCP_Configuration](/images/02_WinSCP_Configuration.png)

7. Wähle die passende Datei aus und klicke auf **Öffnen**

    ![03_WinSCP_Configuration](/images/03_WinSCP_Configuration.png)

8. Der Pfad inklusive Dateiname sollte nun im gelb markierten Textfeld angezeigt werden. Klicke auf die Schaltfläche **OK** um zur Anmeldeseite von WinSCP zurückzukehren.

    ![04_WinSCP_Configuration](/images/04_WinSCP_Configuration.png)

9. Speichere deine Eingaben, indem du auf die Schaltfläche **Speichern* klickst.

    ![05_WinSCP_Configuration](/images/05_WinSCP_Configuration.png)

10. Gib unter **Name des Verbindungsziels:** einen beliebigen Namen ein oder verwende den vorgegebenen Namen. Klicke auf **OK**, um die Sitzung zu speichern.

    ![06_WinSCP_Configuration](/images/06_WinSCP_Configuration.png)

11. Dein gespeichertes Verbindungsziel kannst du ab sofort auf der linken Seite auswählen, um eine Verbindung zu deinem Remote Server herzustellen. Klicke dazu auf die Schaltfläche **Verbinden**.



