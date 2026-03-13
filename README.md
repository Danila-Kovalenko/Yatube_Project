# Yatube Project

Dieses Repository enthält mehrere Entwicklungsstände von **Yatube** – einem Django-basierten sozialen Netzwerk für Blog-Beiträge – inklusive Web-Anwendung und API-Version.

## Projektüberblick

Yatube ermöglicht es Benutzerinnen und Benutzern,
- eigene Beiträge zu veröffentlichen,
- Profile und Gruppenseiten zu nutzen,
- Beiträge zu kommentieren,
- anderen Autorinnen/Autoren zu folgen,
- sowie Inhalte über eine REST-API bereitzustellen (in den API-Versionen).

## Repository-Struktur

- `Yatube_v.0.7/` – frühere Web-Version (klassische Django-Templates).
- `Yatube_v.0.8/` – API-Entwicklungsstand.
- `Yatube_v.0.9/` – erweiterte API-Version (inkl. JWT-Authentifizierung).
- `Yatube_FInal_Cut/` – finale Web-Version mit den zentralen Funktionen des sozialen Netzwerks.

## Verwendete Technologien

- Python 3.7+
- Django 2.2.x
- Django REST Framework (API-Teile)
- Pytest (Tests)

## Lokales Starten (Beispiel)

> Die folgenden Schritte gelten grundsätzlich für jeden Unterordner mit `manage.py`.

1. In die gewünschte Projektversion wechseln, z. B.:
   ```bash
   cd Yatube_FInal_Cut/yatube
   ```
2. Virtuelle Umgebung erstellen und aktivieren:
   ```bash
   python3 -m venv venv
   source venv/bin/activate
   ```
3. Abhängigkeiten installieren:
   ```bash
   pip install -r ../requirements.txt
   ```
   *(Alternativ die `requirements.txt` der jeweiligen Version verwenden.)*
4. Migrationen ausführen:
   ```bash
   python3 manage.py migrate
   ```
5. Entwicklungsserver starten:
   ```bash
   python3 manage.py runserver
   ```

## Tests

Beispiel (im jeweiligen Versionsordner):

```bash
pytest
```

---

Wenn du möchtest, kann ich als Nächstes noch eine kompaktere README pro Unterprojekt (`v0.7`, `v0.8`, `v0.9`, `Final_Cut`) erstellen, damit jede Version eine eigene, klare Dokumentation hat.
