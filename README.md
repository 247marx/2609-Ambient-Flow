# Ambient Flow

Ruhiger Bildschirm-Hintergrund für einen 65"-Screen im Büro (iiyama CMS).
Eine einzige `index.html`, keine Abhängigkeiten, alles wird live per WebGL berechnet.

- 10 selbst entworfene Welten: Seide, Nordlicht, Tinte, Topografie, Dünenmeer, Lichter, Farbfelder, Strömung, Meer, Wolken
- 25 Varianten (Welt + Farbwelt + Parameter), jede startet mit neuen Zufallswerten
- 100 s pro Variante, davon 20 s weiche Überblendung
- kein Text auf dem Bildschirm
- passt die Render-Auflösung automatisch an, damit schwache Player flüssig bleiben

## Parameter (an die URL anhängen)

| Parameter | Wirkung | Standard |
|---|---|---|
| `?dur=100` | Sekunden pro Variante | 100 |
| `?fade=20` | Sekunden Überblendung | 20 |
| `?speed=0.7` | Tempo aller Bewegungen | 1 |
| `?only=sea,silk` | nur diese Welten | alle |
| `?skip=topo` | Welten auslassen | – |
| `?brightness=0.8` | Helligkeit | 1 |
| `?maxres=1280` | max. interne Breite (für schwache Player) | 1600 |
| `?fps=30` | Bildrate (30 schont den Player, 60 = flüssiger) | 30 |
| `?debug=1` | FPS und Auflösung einblenden | aus |

Beispiel: `https://247marx.github.io/2609-Ambient-Flow/?speed=0.8&brightness=0.9`
