<div align="center">

# 🤟 HearingX

### Gebärdensprache lernen, direkt im Browser

Kamera an, Gebärde zeigen, sofort Feedback bekommen.
Komplett offline, ohne Installation, ohne Upload.

<br>

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![MediaPipe](https://img.shields.io/badge/MediaPipe-0097A7?style=for-the-badge&logo=google&logoColor=white)
![Three.js](https://img.shields.io/badge/Three.js-000000?style=for-the-badge&logo=threedotjs&logoColor=white)

![Offline](https://img.shields.io/badge/100%25-Offline-2ea44f?style=flat-square)
![Datenschutz](https://img.shields.io/badge/Kamera-bleibt_lokal-blueviolet?style=flat-square)
![Mobile](https://img.shields.io/badge/iOS_%26_Android-ready-orange?style=flat-square)
![Single File](https://img.shields.io/badge/Single-HTML_File-lightgrey?style=flat-square)

<br>

[✨ Features](#-features) &nbsp;•&nbsp; [🚀 Starten](#-starten) &nbsp;•&nbsp; [🔒 Datenschutz](#-datenschutz) &nbsp;•&nbsp; [🛠 Technik](#-technik) &nbsp;•&nbsp; [🗺 Roadmap](#-roadmap)

</div>

<br>

## ✨ Features

<table>
<tr>
<td width="50%" valign="top">

### 🖐 Handerkennung live
MediaPipe erkennt **21 Handpunkte** in Echtzeit. Ein eigener Klassifikator wertet Fingerstellung und Daumenwinkel aus, Bewegungsgebärden werden zusätzlich erkannt. Ein **10 Frame Puffer** mit Mehrheitsentscheid sorgt für stabile Ergebnisse.

</td>
<td width="50%" valign="top">

### 🧠 Lernpfad mit Leitner System
Intelligente Wiederholung: Karten wandern je nach Ergebnis in höhere oder niedrigere Boxen. Fällige Gebärden kommen genau dann, wenn du sie fast vergessen hättest.

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 📷 Kamera Prüfung
Karte aufdecken, auf **„Mit Kamera prüfen“** tippen, Gebärde zeigen. Die App bewertet dich automatisch und schiebt die Karte selbst in die richtige Box.

</td>
<td width="50%" valign="top">

### 🔥 Streak & Quiz
Echter Streak Zähler für aufeinanderfolgende Übungstage, Quizmodus zum Abfragen und ein Verlauf mit Trefferquote und nächster fälliger Wiederholung.

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🌙 Dunkelmodus
Ein Klick auf 🌙 im Header, die Einstellung wird gemerkt. Optimierte Kontraste für Lesbarkeit bei Nacht.

</td>
<td width="50%" valign="top">

### ♿ Barrierefrei & mobil
Responsives Layout, iOS Safe Area Unterstützung, Tastaturbedienung und ARIA Attribute für Screenreader.

</td>
</tr>
</table>

<br>

## 🚀 Starten

> [!IMPORTANT]
> Browser erlauben die Kamera nur über `https` oder `localhost`. Ein Doppelklick auf die Datei reicht deshalb nicht.

<details open>
<summary><b>💻 Am PC</b></summary>
<br>

```bash
git clone https://github.com/Tscheky/hearingx.git
cd hearingx
python -m http.server 8000
```

Dann im Browser öffnen: **http://localhost:8000/hearingx.html**

</details>

<details>
<summary><b>📱 Am Handy</b></summary>
<br>

Lokalen Server wie oben starten und zusätzlich einen Tunnel öffnen:

```bash
npx localtunnel --port 8000
```

oder

```bash
ngrok http 8000
```

Die angezeigte https Adresse in Safari oder Chrome öffnen.

</details>

<details>
<summary><b>🌐 Online über GitHub Pages</b></summary>
<br>

Im Repository **Settings › Pages** öffnen, Branch `main` wählen, speichern.
Die App läuft danach unter **https://tscheky.github.io/hearingx/hearingx.html**

</details>

<br>

## 🔒 Datenschutz

| | |
|:--|:--|
| 📷 **Kamerabilder** | werden ausschließlich lokal im Browser verarbeitet und nie hochgeladen |
| 💾 **Lernstand** | wird nur gespeichert, wenn du es in den Einstellungen aktivierst |
| 🗑 **Löschen** | jederzeit mit einem Klick über „Lernstand löschen“ |
| 🍪 **Tracking** | keines, keine Cookies, keine Analyse Dienste |

<br>

## 🛠 Technik

| Bereich | Umsetzung |
|:--|:--|
| **Frontend** | HTML, CSS und JavaScript in einer einzigen Datei |
| **Handerkennung** | MediaPipe Hands mit eigenem Formklassifikator |
| **Bewegungen** | Datengetriebene Lookup Tabelle für Bewegungsgebärden |
| **Stabilisierung** | Ringpuffer über 10 Frames mit Mehrheitsentscheid |
| **3D** | Three.js |
| **Lernlogik** | Leitner Spaced Repetition |
| **Speicher** | localStorage, optional und abgesichert |
| **Performance** | Vision Loop auf ca. 20 fps gedrosselt für mobile Geräte |

<br>

## 🗺 Roadmap

| Status | Vorhaben |
|:--:|:--|
| ✅ | Handerkennung, Lernpfad, Kamera Prüfung |
| ✅ | Streak, Quiz, Verlauf |
| ✅ | Dunkelmodus, Mobile, Barrierefreiheit |
| 🔄 | Desktop App mit Tauri oder Electron |
| 🔄 | Größerer Gebärdenwortschatz |
| 💡 | Backend mit eigenem Erkennungsmodell |

<br>

<div align="center">

## 👤 Autor

**Tscheky**
IT Netzwerktechniker in Ausbildung · Schulungszentrum Fohnsdorf

[![GitHub](https://img.shields.io/badge/GitHub-Tscheky-181717?style=for-the-badge&logo=github)](https://github.com/Tscheky)

<br>

⭐ Wenn dir das Projekt gefällt, lass gern einen Stern da

</div>
