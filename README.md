# **Flux-Prompt-Generator**

Der **Flux Prompt Generator** ist ein **ComfyUI**-Knoten, der einen flexiblen und anpassbaren Prompt-Generator für die Erstellung detaillierter und kreativer Prompts für Bildgenerierungsmodelle bereitstellt. Er basiert auf der Arbeit von [Aitrepreneur](https://huggingface.co/Aitrepreneur), die hier zu finden ist: [Flux Prompt Generator Python Code](https://huggingface.co/Aitrepreneur/FLUX-Prompt-Generator/blob/main/app.py) und wurde von [FairyRoot](https://github.com/fairy-root) für die Arbeit mit ComfyUI angepasst.

![Flux Prompt Generator](https://i.imgur.com/I3nQzaa.png "Workflow anzeigen")

## Überblick

Der **Flux Prompt Generator** nutzt eine Sammlung von JSON-Datendateien, die verschiedene Kategorien von beschreibenden Begriffen enthalten. Zu diesen Kategorien gehören:

- **Kunstform:** Fotografie, Digitale Kunst, etc.
- **Fotoart:** Porträt, Landschaft, etc.
- **Körpertypen:** Muskulös, Dünn, etc.
- **Standard-Tags:** Mann, Frau, Kind, etc.
- **Rollen:** Ritter, Zauberer, etc.
- **Frisuren:** Lang, Kurz, Geflochten, etc.
- **Zusätzliche Details:** Kleidung, Accessoires, etc.
- **Fotografiestile:** Kinematografisch, Realistisch, etc.
- **Gerät:** Kameramodelle, etc.
- **Fotograf:** Berühmte Fotografen, etc.
- **Künstler:** Berühmte Künstler, etc.
- **Digitale Kunstform:** Pixelkunst, 3D-Render, etc.
- **Ort:** Wald, Stadt, etc.
- **Beleuchtung:** Weich, Hart, etc.
- **Kleidung:** Kleid, Anzug, etc.
- **Komposition:** Drittelregel, Goldener Schnitt, etc.
- **Pose:** Stehend, Sitzend, etc.
- **Hintergrund:** Einfach, Detailliert, etc.
- **Gesichtsmerkmale:** Scharfe Kieferlinie, Hohe Wangenknochen, etc.
- **Augenfarben:** Blau, Grün, Braun, etc.
- **Gesichtsbehaarung:** Bart, Schnurrbart, etc.
- **Hautfarbe:** Hell, Dunkel, etc.
- **Altersgruppe:** Kind, Teenager, Erwachsener, etc.
- **Ethnie:** Verschiedene ethnische und kulturelle Hintergründe.
- **Accessoires:** Brillen, Hüte, Schmuck, etc.
- **Ausdruck:** Lächeln, Stirnrunzeln, Überraschung, etc.
- **Tattoos & Narben:** Detaillierte Beschreibungen von Körpermodifikationen.
- **Make-up-Stile:** Natürlich, Glamourös, etc.
- **Haarfarbe:** Blond, Braun, Schwarz, etc.
- **Körpermarkierungen:** Muttermale, Leberflecken, Sommersprossen, etc.

![Flux Prompt Generator](https://i.imgur.com/0TNizfp.png "Knoten anzeigen")

Der Knoten ermöglicht es, bestimmte Begriffe auszuwählen oder "zufällig" auszuwählen, um den Generator zufällige Begriffe aus der entsprechenden JSON-Datei auswählen zu lassen. Diese Zufälligkeit fügt den erstellten Prompts ein gewisses Maß an Unvorhersehbarkeit und Kreativität hinzu.

## Installation

1. Wechsle in den **custom_nodes**-Ordner innerhalb des **ComfyUI**-Verzeichnisses.
2. Öffne ein **cmd**-Fenster in der Adressleiste und benutze diesen Befehl:
```
git clone https://github.com/fairy-root/Flux-Prompt-Generator.git
```

## Verwendung

1. **Füge den "Flux Prompt Generator"-Knoten zu deinem ComfyUI-Workflow hinzu.**
2. **Konfiguriere die gewünschten Parameter:**
    - **Seed:** Steuert die Zufälligkeit des Generators.
    - **Custom:** Füge eigenen Text zum Prompt hinzu.
    - **Subject:** Gib das Hauptthema des Bildes an.
    - **Kunstform:** Wähle die gewünschte Kunstform (Fotografie, Digitale Kunst, etc.).
    - **... (Alle anderen Parameter wie im Überblick beschrieben)**

3. **Verbinde den Output des Knotens mit einem Text-zu-Bild-Modell (wie Flux oder Stable Diffusion, etc.), um Bilder basierend auf dem erstellten Prompt zu generieren.**

## Beispiel

Angenommen, du möchtest einen Prompt für ein Porträtfoto einer Frau mit langen Haaren, die ein Kleid trägt und in einem Wald steht, generieren. Du könntest den Knoten mit den folgenden Parametern konfigurieren:

- **Kunstform:** Fotografie
- **Fotoart:** Porträt
- **Standard-Tags:** Frau
- **Frisuren:** Lange Haare
- **Kleidung:** Kleid
- **Ort:** Wald

Der Knoten würde dann einen Prompt wie folgt generieren: "Fotografie einer Frau mit langen Haaren, die ein Kleid trägt, in einem Wald."

## Spenden

Deine Unterstützung wird geschätzt:

- USDt (TRC20): `TGCVbSSJbwL5nyXqMuKY839LJ5q5ygn2uS`
- BTC: `13GS1ixn2uQAmFQkte6qA5p1MQtMXre6MT`
- ETH (ERC20): `0xdbc7a7dafbb333773a5866ccf7a74da15ee654cc`
- LTC: `Ldb6SDxUMEdYQQfRhSA3zi4dCUtfUdsPou`

## Autor und Kontakt

- GitHub: [FairyRoot](https://github.com/fairy-root)
- Telegram: [@FairyRoot](https://t.me/FairyRoot)

## Lizenz

Dieses Projekt ist unter der MIT-Lizenz lizenziert. Siehe die [LICENSE](LICENSE)-Datei für Details.

## Beiträge

Beiträge sind willkommen! Bitte öffne ein Issue oder reiche einen Pull-Request für Verbesserungen oder neue Funktionen ein.
