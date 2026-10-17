# ZephyrFlix
![ZephyrFlix — votre cinéma, chez vous](https://eric-mager-lab.balmylily512.chatgpt.site/assets/zephyrflix-logo.png)

[Français](#français) · [English](#english)

## Français

ZephyrFlix organise vos fichiers vidéo locaux dans une médiathèque Windows : films, séries, saisons, favoris et reprise de lecture. **Il ne fournit aucun film ni aucune série.**

| Dimension | État au 17 octobre 2026 |
|---|---|
| Maturité | **1.4.0 — version de test / Release candidate** |
| Distribution / prix | Version de test gratuite, proposée via la page officielle du LAB |
| Code / droits | Code propre privé et réservé ; ce dossier contient la documentation et les visuels autorisés |

### Un projet né dans l'atelier
Eric Mager, alias **Terrelfe**, voulait retrouver ses anciens films sans parcourir une arborescence de dossiers. Une première approche web a rencontré les limites des formats lisibles dans un navigateur. Le projet est devenu une application Windows native avec Rust, Slint, SQLite et libVLC.

Une première version fonctionnait en septembre 2026. Après la perte des sources, la reprise d'octobre s'est appuyée sur l'historique technique survivant. Elle a aussi permis de retravailler le catalogue, le lecteur, les données et les détails de l'interface. Le besoin initial a évolué ; l'envie de soigner l'outil et de le proposer gratuitement est restée.

Zéphyr est l'identité de l'IA personnelle d'Eric et sa partenaire de réflexion et de création. Eric conçoit, arbitre et valide ; l'assistance IA et Codex participent au développement et à la documentation. Le Kitsune blanc aux marques rouges et aux yeux ambrés accompagne cet univers.

### Ce qui a été vérifié localement
- Catalogue de films et séries, saisons et épisodes ; recherche, filtres, tris et tags personnels.
- Favoris, progression, reprise et protection des choix d'identification manuels.
- Lecteur natif : lecture, pause, déplacement dans la vidéo, volume, arrêt, plein écran F11 et retour Échap.
- Import facultatif d'une ancienne bibliothèque par copie sauvegardée ; premier lancement et données séparées de l'application.
- Aide & retours : brouillon mail sans envoi ni fichier joint automatiques ; adresse copiable.
- Identification assistée : **PROBABLE reste une suggestion à confirmer**. Le service TMDB est facultatif et son authentification avec une clé utilisateur n'a pas encore été vérifiée.

![Premier lancement réel avec profil de test vierge](https://eric-mager-lab.balmylily512.chatgpt.site/assets/zephyrflix-onboarding.png)

### Télécharger et démarrer la version de test
**[Page officielle de téléchargement — ZephyrFlix 1.4.0 RC](https://eric-mager-lab.balmylily512.chatgpt.site/downloads/zephyrflix/)**

Version de test gratuite pour **Windows 10 x64 (1809 ou ultérieur) et Windows 11 x64**. Le test sur un autre PC Windows x64 n'a pas encore été réalisé ; cette version n'est pas annoncée comme stable.

L'installateur **Setup x64 RC 1.4** propose le français et l'anglais, installe l'application pour votre compte **sans droits administrateur**, et crée les raccourcis Bureau et menu Démarrer. **Le lecteur VLC 3.0.24 sélectionné pour cette distribution et le runtime Visual C++ sont inclus** : aucune installation séparée de VLC n'est nécessaire pour ce Setup. Les données du profil restent séparées de l'application et sont conservées lors de la désinstallation.

1. Télécharger le **Setup x64 RC** depuis la page officielle et vérifier son SHA-256 si souhaité.
2. Double-cliquer dessus, choisir la langue et suivre les étapes d'installation.
3. Ouvrir ZephyrFlix depuis le raccourci, choisir ses dossiers vidéo et leur type, puis lancer l'analyse.

Le **ZIP Portable RC initial** est un autre paquet : il requiert **VLC 3 x64 installé séparément** et **Microsoft Visual C++ Redistributable x64 si absent**. Ne mélangez pas ses instructions avec celles du Setup.

Le scan ne renomme ni ne déplace les vidéos. [Guide et raccourcis](docs/GUIDE.md) · [FAQ](docs/FAQ.md). Les sources et notices des composants tiers redistribués sont proposées séparément sur la même page de téléchargement ; le code propre de ZephyrFlix reste privé.

### Limites et droits
Les contrôles locaux comprennent 33 tests Rust, les compilations debug/release, fmt, check et Clippy, ainsi que des scénarios UI et de lecture natifs. Ils ne remplacent pas un test sur une autre machine ; tous les formats et fichiers ne sont pas garantis. L'exécutable ne possède pas de certificat de signature Windows. La notice MIT de `simd_helpers` a été retrouvée dans l'amont et sa source comparée à la version utilisée ; le texte exact est [conservé ici](docs/licenses/simd_helpers-MIT.txt). Le Setup et son paquet de sources tierces sont distincts de l'ancien candidat Portable. [État daté de validation](docs/VALIDATION.md).

Application gratuite, code **réservé pour le moment, pas open source**. La gratuité ne confère aucun droit de réutilisation du code ou des visuels. Les composants tiers conservent leurs propres licences. [Conditions exactes](LICENSE.md) · [Notices](THIRD_PARTY_NOTICES.md) · [Crédits et visuels](docs/CREDITS.md) · [Confidentialité](docs/PRIVACY.md).

### Contact et atelier
**zephyr.essentiel@gmail.com** — [signaler un bug](mailto:zephyr.essentiel@gmail.com?subject=ZephyrFlix%20-%20Bug), [proposer une idée](mailto:zephyr.essentiel@gmail.com?subject=ZephyrFlix%20-%20Amelioration), [demander de l'aide](mailto:zephyr.essentiel@gmail.com?subject=ZephyrFlix%20-%20Aide). Aucun délai de réponse garanti. Relisez les informations que vous choisissez d'envoyer ; ne joignez pas de clé ou de bibliothèque privée.

[ERIC MAGER — LAB](https://eric-mager-lab.balmylily512.chatgpt.site) · [Page projet du LAB](https://eric-mager-lab.balmylily512.chatgpt.site/fr/projets/zephyrflix/) · [Notre univers](docs/UNIVERSE.md) · [Histoire](docs/HISTORY.md) · [Changelog](CHANGELOG.md).

## English

ZephyrFlix turns your own local video files into a Windows library with films, series, seasons, favourites and playback resume. **It supplies no films or series.**

| Dimension | Status on 17 October 2026 |
|---|---|
| Maturity | **1.4.0 — test version / Release candidate** |
| Distribution / price | Free test version, offered through the official LAB page |
| Code / rights | Own source code private and reserved; this folder contains documentation and approved visuals |

### From a practical need to a shared project
Eric Mager, also known as **Terrelfe**, wanted to find old films without browsing endless folders. An early web approach ran into browser format limitations. ZephyrFlix became a native Windows application built with Rust, Slint, SQLite and libVLC.

The first working version dates to September 2026. Following source loss, the October recovery used surviving technical history and became an opportunity to improve the catalogue, playback, data handling and interface. Although the original need has evolved, the intention remains to refine a useful tool and share it for free.

Zéphyr is the identity of Eric's personal AI and his thinking and creation partner. Eric directs and validates the work; AI assistance and Codex support development and documentation. The white Kitsune, with red markings and amber eyes, is part of this creative universe.

### Locally verified features
- Film and series catalogue, seasons and episodes; search, filters, sorting and personal tags.
- Favourites, progress, resume and protection of manual identification choices.
- Native playback: play, pause, seek, volume, stop, F11 fullscreen and Escape to return.
- Optional legacy-library import through a backed-up copy, first-run flow and separate application/user data.
- Help & feedback opens an email draft with no automatic sending or attachments; the address can be copied.
- Assisted identification: **PROBABLE is a suggestion requiring confirmation**. TMDB is optional; authentication with a user API key has not been tested.

### Download and start the test version
**[Official download page — ZephyrFlix 1.4.0 RC](https://eric-mager-lab.balmylily512.chatgpt.site/downloads/zephyrflix/)**

Free test version for **Windows 10 x64 (1809 or later) and Windows 11 x64**. Testing on a separate Windows x64 PC has not been performed; this version is not advertised as stable.

The **Setup x64 RC 1.4** installer offers French and English, installs for your account **without administrator privileges**, and creates desktop and Start menu shortcuts. **The selected VLC 3.0.24 player runtime and Visual C++ runtime are included**: this Setup does not require a separate VLC installation. Profile data stays separate from application files and is preserved when uninstalling.

1. Download **Setup x64 RC** from the official page and check SHA-256 if desired.
2. Double-click it, choose a language and follow the installation steps.
3. Open ZephyrFlix through its shortcut, select your video folders and their types, then scan.

The **original Portable RC ZIP** is a separate package: it needs **VLC 3 x64 installed separately** and the **Microsoft Visual C++ x64 Redistributable if missing**. Its instructions differ from Setup instructions.

Scanning does not move or rename videos. [Guide](docs/GUIDE.md) · [FAQ](docs/FAQ.md). Sources and notices for redistributed third-party components are provided separately through the same download page; ZephyrFlix's own code remains private.

### Validation, rights and contact
Local checks include 33 Rust tests, debug/release builds, fmt, check, Clippy, UI and native playback scenarios. They do not substitute for independent-machine testing or guarantee every file/format. There is no Windows code-signing certificate. The upstream MIT notice for `simd_helpers` was found and its source compared with the version in use; the [exact notice is included](docs/licenses/simd_helpers-MIT.txt). Setup and its third-party source package are separate from the original Portable candidate. [Dated validation status](docs/VALIDATION.md).

Free to use; own code **reserved for now, not open source**. Third-party components retain their licences. [Project terms in French](LICENSE.md) · [Notices](THIRD_PARTY_NOTICES.md) · [Credits](docs/CREDITS.md) · [Privacy](docs/PRIVACY.md).

**zephyr.essentiel@gmail.com** — [bug](mailto:zephyr.essentiel@gmail.com?subject=ZephyrFlix%20-%20Bug), [idea](mailto:zephyr.essentiel@gmail.com?subject=ZephyrFlix%20-%20Idea), [help](mailto:zephyr.essentiel@gmail.com?subject=ZephyrFlix%20-%20Help). No guaranteed response time. Please review anything you choose to send and keep personal libraries and API keys private.

[ERIC MAGER — LAB](https://eric-mager-lab.balmylily512.chatgpt.site) · [LAB project page](https://eric-mager-lab.balmylily512.chatgpt.site/en/projects/zephyrflix/) · [Our Universe](docs/UNIVERSE.md) · [History](docs/HISTORY.md) · [Changelog](CHANGELOG.md).

Vitrine documentaire / Documentary showcase : [GitHub](https://github.com/magerericsev-design/magerericsev-design/tree/main/projects/zephyrflix).
