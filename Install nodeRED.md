# NodeRED

## NodeRED lokal installieren

### tldr;

1. NodeJS installieren (v 12.X.)
2. npm install -g --unsafe-perm node-red
3. http://localhost:1880/
4. "Neuen Typ 'mqtt-broker' hinzufügen": Server "maqiatto.com", Port: 1883
5. Test-Topic: "christopher.ringel@hs-heilbronn.de/test"

### NodeRED lokal installieren:

1. NodeJS 12.X (recommended) installieren: https://nodejs.org/dist/v12.9.1/
		○ Windows: https://nodejs.org/dist/v12.9.1/node-v12.9.1-x64.msi
![grafik](https://user-images.githubusercontent.com/83697765/117122005-a7178180-ad95-11eb-80be-2243e3027ea8.png)
2. NodeRED installieren:
		○ Windows: npm install -g --unsafe-perm node-red
3. NodeRED starten: node-red
4. Hinweis: Windows Firewall Anfrage bestätigen
5. http://localhost:1880/
6. Strg+C im Konsolenfenster, um NodeRED Server zu terminieren


Troubleshooting und mehr Infos hier: https://nodered.org/docs/getting-started/local#running

### NodeRED und MQTT-Broker Maqiatto verbinden:

1. NodeRED Server lokal starten
2. Im Flow ein "mqtt in" Node erstellen ![grafik](https://user-images.githubusercontent.com/83697765/117122035-b1398000-ad95-11eb-9b78-66a0f38d4b3b.png)
3. Doppelklick auf den Node zum parametrisieren
4. Bei Server: "Neuen Typ 'mqtt-broker' hinzufügen" bearbeiten ![grafik](https://user-images.githubusercontent.com/83697765/117122110-cd3d2180-ad95-11eb-9460-660060e5fb40.png)
5. Name: Maqiatto
6. Reiter "Verbindung": Server "maqiatto.com", Port: 1883 ![grafik](https://user-images.githubusercontent.com/83697765/117122155-de862e00-ad95-11eb-8401-c70634918740.png)
7. Reiter "Sicherheit": Benutzername christopher.ringel@hs-heilbronn.de, Passwort: sose21 ![grafik](https://user-images.githubusercontent.com/83697765/117122170-e2b24b80-ad95-11eb-8e3f-85a69b0ead17.png)
8. Oben rechts: "Hinzufügen" (roter Button) klicken 
9. Zum testen der Verbindung: Topic: "christopher.ringel@hs-heilbronn.de/test" eintragen (oder eins Eurer Gruppen-Topics)
10. "Fertig" ![grafik](https://user-images.githubusercontent.com/83697765/117122201-eba31d00-ad95-11eb-9186-1d80825a555b.png)
11. "Übernahme (deploy)" ![grafik](https://user-images.githubusercontent.com/83697765/117122217-f362c180-ad95-11eb-94d8-c7c6d65d8b88.png)
12. "Verbunden" sollte neben dem Node erscheinen ![grafik](https://user-images.githubusercontent.com/83697765/117122228-f5c51b80-ad95-11eb-82dd-e059135423c0.png)
