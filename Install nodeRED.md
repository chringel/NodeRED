# NodeRED

## NodeRED lokal installieren

### tldr;

1. NodeJS installieren
2. npm install -g --unsafe-perm node-red
3. http://localhost:1880/
4. "Neuen Typ 'mqtt-broker' hinzufügen": Server "maqiatto.com", Port: 1883
5. Test-Topic: "christopher.ringel@hs-heilbronn.de/test"

### NodeRED lokal installieren:

1. NodeJS 12.X (recommended) installieren: https://nodejs.org/dist/v12.9.1/
		○ Windows: https://nodejs.org/dist/v12.9.1/node-v12.9.1-x64.msi
2. NodeRED installieren:
		○ Windows: npm install -g --unsafe-perm node-red
3. NodeRED starten: node-red
4. Hinweis: Windows Firewall Anfrage bestätigen
5. http://localhost:1880/
6. Strg+C im Konsolenfenster, um NodeRED Server zu terminieren


Troubleshooting und mehr Infos hier: https://nodered.org/docs/getting-started/local#running

### NodeRED und MQTT-Broker Maqiatto verbinden:

1. NodeRED Server lokal starten
2. Im Flow ein "mqtt in" Node erstellen
3. Doppelklick auf den Node zum parametrisieren
4. Bei Server: "Neuen Typ 'mqtt-broker' hinzufügen" bearbeiten
5. Name: Maqiatto
6. Reiter "Verbindung": Server "maqiatto.com", Port: 1883
7. Reiter "Sicherheit": Benutzername christopher.ringel@hs-heilbronn.de, Passwort: sose21
8. Oben rechts: "Hinzufügen" (roter Button) klicken
9. Zum testen der Verbindung: Topic: "christopher.ringel@hs-heilbronn.de/test" eintragen (oder eins Eurer Gruppen-Topics)
10. "Fertig"
11. "Übernahme (deploy)"
12. "Verbunden" sollte neben dem Node erscheinen