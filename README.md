<p align="center">
    <img alt="Pandemie" src="https://nicolas-schaber.de/assets/logo.png" width="200" />
</p>
<h1 align="center">
  Pandemie
</h1>
<h3 align="center">
Lösungsvorschlag für den InformatiCup 2020 der Gesellschaft für Informatik
</h3>
<p align="center">
Dieses Repository beeinhaltet die Lösung für den InformatiCup 2020 des Teams Nicolas Schaber, Daniel Schulz und Max Schiffer der DHBW Karlsruhe.
</p>
<p align="center">
Repository der Aufgabe: https://github.com/informatiCup/informatiCup2020
</p>
<p align="center">
    <img alt="GitHub top language" src="https://img.shields.io/github/languages/top/nicosc77/pandemie?style=for-the-badge">
 <img alt="GitHub Pipenv locked dependency version" src="https://img.shields.io/github/pipenv/locked/dependency-version/nicosc77/pandemie/flask?color=lightgrey&style=for-the-badge">
  <img alt="GitHub Pipenv locked dependency version" src="https://img.shields.io/github/pipenv/locked/dependency-version/nicosc77/pandemie/tensorflow?color=yellow&style=for-the-badge">
  <img alt="GitHub Pipenv locked dependency version" src="https://img.shields.io/github/pipenv/locked/dependency-version/nicosc77/pandemie/keras?color=red&style=for-the-badge">
</p>

## 🚀 Deployment

- **Docker:**
Mithilfe des Dockerfile im Root-Verzeichnis des Projekt lässt sich ein Image bauen, das als Container mit Docker ausgeführt werden kann. Die Anwendung ist dann unter http://localhost:5000 zu erreichen. 
  ```shell
  docker build -t pandemie .
  docker run -p 5000:5000 -d pandemie
  ```

- **Cloud-Plattform:**
 Zudem besteht die Möglichkeit die bereits laufende Anwendung über das Internet zu verwenden. Wir lassen dazu den Docker-Container auf einem Google Kubernetes Engine Cluster laufen. Die Anwendung hier ist unter der URL http://pandemie.nicolas-schaber.de zu erreichen.

## 🔧Testen
Mithilfe der aktuellsten Version des Kommandozeilen-Tools aus dem Repository des Wettbewerbs kann mit der Software ein Spiel gespielt werden. Dazu führt man das Tool mit Angabe der URL (Je nach Deployment-Methode) der Anwendung aus. Auf Unix- System muss das Tool eventuell zuerst ausführbar gemacht werden.

Hier z.B. für das lokale Deployment:
- **Windows:**
  ```shell
  ic20_windows.exe -u "http://localhost:5000"
  ```
- **Linux:**
  ```shell
  ./ic20_linux -u "http://localhost:5000"
  ```
- **macOS:**
  ```shell
  ./ic20_darwin -u "http://localhost:5000"
  ```

Anschließend spielt das Tool gegen unsere KI der Software ein Spiel. Nachdem entweder gewonnen oder verloren wurde wird das Tool beendet. Im Feld "outcome" lässt sich der Ausgang des Spiels durch "win" oder "loss" feststellen.

## 📄Dokumentation
Genauere Informationen zu dieser Software ist in der [Dokumentation](Dokumentation.pdf) zu finden.
