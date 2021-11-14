# NodeRED

## NodeRED lokal installieren

### tldr;

1. NodeJS installieren (v 12.X.)
2. NodeRED installieren: <code>npm install -g node-red</code>
3. goto: http://localhost:1880/
4. Aedes Palette zu NodeRED hinzufügen (node-red-contrib-aedes)

### NodeRED lokal installieren:

1. NodeJS 12.X (recommended) installieren. (Alle Versionen: https://nodejs.org/dist/)
2. NodeRED global installieren:
- Windows: <code>npm install -g node-red</code>
3. NodeRED starten: <code>node-red</code>
4. Hinweis: Windows Firewall Anfrage bestätigen
5. http://localhost:1880/
6. Strg+C im Konsolenfenster, um NodeRED Server zu terminieren


### Beispiel MQTT Roundtrip:

![aedes-use](https://user-images.githubusercontent.com/83697765/141686407-ed59931c-173a-43c3-99a1-51bef08d559e.gif)

### Troubleshooting:

- NodeRED: https://nodered.org/docs/getting-started/local#running
- Aedes node-red-contrib: https://github.com/martin-doyle/node-red-contrib-aedes
