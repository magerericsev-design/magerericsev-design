# Guide / User guide — ZephyrFlix 1.4 RC

## Français — installation simple
Version de test gratuite disponible publiquement pour **Windows 10 x64 1809+ et Windows 11 x64**. [Page officielle de téléchargement](https://eric-mager-lab.balmylily512.chatgpt.site/downloads/zephyrflix/). Le test sur un autre PC n'a pas encore été réalisé ; l'exécutable n'a pas de certificat de signature Windows.

**Langues : site et documentation bilingues, installateur français/anglais ; interface actuelle de ZephyrFlix principalement en français.**

1. Télécharger **ZephyrFlix-1.4.0-Setup-x64-RC.exe**, puis double-cliquer sur le fichier. Choisir français ou anglais. L'installation se fait pour votre compte, sans droits administrateur.
2. Suivre les étapes : l'application, son lecteur VLC 3.0.24 sélectionné et le runtime Visual C++ sont inclus. Aucune installation séparée de VLC n'est nécessaire avec le Setup. Les raccourcis Bureau et menu Démarrer permettent de l'ouvrir simplement.
3. Dans ZephyrFlix, choisir **Parcourir**, sélectionner un dossier et son type (Films, Séries, Documentaires ou Détection automatique), puis **Ajouter**. Plusieurs dossiers sont possibles. Cliquer **Créer ma bibliothèque** ou **Analyser**.
4. Rechercher, filtrer et trier les œuvres. Une série ouvre ses saisons et épisodes. Ajouter des favoris ou des tags sur une fiche ; **Continuer** retrouve les lectures commencées.
5. Choisir **Regarder / Reprendre**. Espace met en pause ; F11 ouvre le plein écran ; Échap revient en fenêtre. Les commandes règlent le volume, la position, les pistes et les sous-titres. Le double clic vidéo n'est pas implémenté.
6. Les affiches et résumés distants demandent une clé TMDB personnelle facultative. Sans clé, les fonctions locales restent disponibles. Une suggestion **PROBABLE** se confirme manuellement ; aucun résumé n'est inventé. L'essai authentifié avec une clé utilisateur reste à réaliser.
7. **Paramètres → Aide & retours** prépare un brouillon pour un bug, une idée ou une demande d'aide. Aucun envoi ni fichier joint automatiques. Sans client mail, copier **zephyr.essentiel@gmail.com**.

### Mise à jour, sauvegarde et désinstallation
L'installation utilise un emplacement applicatif stable ; le profil installé est conservé séparément dans `%LOCALAPPDATA%/ZephyrFlix`. Fermer l'application avant de copier le dossier complet du profil pour une sauvegarde. Lors d'une mise à jour, conserver ce profil. La désinstallation Windows retire l'application et ses raccourcis ; elle conserve le profil, les favoris et la progression. Les vidéos choisies ne sont ni déplacées ni supprimées.

Un ancien profil Zephyr Media peut être proposé au premier lancement installé. Fermer l'ancienne application puis choisir Importer ou Ignorer. L'import travaille sur une copie sauvegardée, refuse d'écraser une bibliothèque existante et ne copie pas les clés API.

### Ancien ZIP Portable RC — instructions différentes
Le candidat ZIP initial n'inclut **pas** VLC ni le runtime Visual C++. Il demande [VLC 3 x64](https://www.videolan.org/vlc/) et le [Visual C++ x64 Redistributable Microsoft](https://learn.microsoft.com/en-us/cpp/windows/latest-supported-vc-redist) s'ils sont absents. Extraire tout le ZIP, ouvrir `PORTABLE.cmd` et préserver son dossier `data/`. Son `INSTALLER.cmd` est un script, distinct du nouveau Setup natif.

ZephyrFlix ne fournit aucun film ni aucune série. [FAQ](FAQ.md) · [Confidentialité](PRIVACY.md) · [Retour](../README.md).

## English — simple installation
Publicly available free test version for **Windows 10 x64 1809+ and Windows 11 x64**. [Official download page](https://eric-mager-lab.balmylily512.chatgpt.site/downloads/zephyrflix/). A separate-PC test has not yet been performed; the executable has no Windows code-signing certificate.

**The installer and documentation are available in English, but the current application interface is primarily in French. The LAB website is bilingual.**

1. Download **ZephyrFlix-1.4.0-Setup-x64-RC.exe** and double-click it. Choose French or English. Setup installs for your account without administrator privileges.
2. Follow the steps: the application, selected VLC 3.0.24 player runtime and Visual C++ runtime are included. No separate VLC installation is needed for Setup. Use the desktop or Start menu shortcut to open ZephyrFlix.
3. Use **Browse**, select a folder and its type, **Add**, then **Create my library / Scan**. Multiple folders are supported. The current application controls are French; these labels are explanatory translations.
4. Search, filter and sort works. Open a series to choose seasons and episodes. Add favourites and personal tags; **Continue** shows started videos.
5. Choose **Watch / Resume**. Space pauses; F11 enters fullscreen; Escape returns. Use controls for position, volume, audio tracks and subtitles. Video double-click is not implemented.
6. Remote posters and descriptions need an optional personal TMDB key. Local features remain available without it. **PROBABLE** suggestions need manual confirmation. No description is invented. User-key authentication remains untested.
7. **Settings → Help & feedback** prepares an email draft for a bug, idea or help request, without automatic sending or attachments. Copy **zephyr.essentiel@gmail.com** if no mail client is configured.

### Updates, backup and uninstall
Setup uses a stable application location; the installed profile is separate in `%LOCALAPPDATA%/ZephyrFlix`. Close the application before copying its complete profile folder for backup. Preserve this profile when updating. Windows uninstall removes the application and shortcuts while retaining the profile, favourites and progress. Your chosen video files are not moved or deleted.

An installed first run may offer legacy Zephyr Media import. Close the old application, then choose Import or Ignore. Import uses a backed-up copy, refuses to overwrite an existing library and excludes API keys.

### Original Portable RC ZIP — different instructions
The initial ZIP candidate includes **neither** VLC nor Visual C++. It requires [VLC 3 x64](https://www.videolan.org/vlc/) and the [Microsoft Visual C++ x64 Redistributable](https://learn.microsoft.com/en-us/cpp/windows/latest-supported-vc-redist) if missing. Extract the whole ZIP, run `PORTABLE.cmd`, and preserve `data/`. Its `INSTALLER.cmd` is a script, separate from the new native Setup.

ZephyrFlix supplies no films or series. [FAQ](FAQ.md) · [Privacy](PRIVACY.md) · [Back](../README.md).
