# birthday

Passwortgeschützte Geburtstagsseite auf GitHub Pages.

- `site/` wird veröffentlicht: `index.html` fragt das Passwort ab und entschlüsselt `video.enc` (AES-GCM, PBKDF2) im Browser.
- `tools/verschluesseln.html` lokal im Browser öffnen, um aus dem fertigen Video eine neue `video.enc` zu erzeugen. Wird nicht veröffentlicht.
- Video austauschen: neue `video.enc` nach `site/` legen, committen, pushen. Die Action deployt automatisch.

Originalvideos (`*.mp4` usw.) sind per `.gitignore` ausgeschlossen. Die verschlüsselte Datei muss unter 100 MB bleiben.
