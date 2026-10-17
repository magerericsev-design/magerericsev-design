# État de validation / Validation status

**Situation au 17 octobre 2026 — ZephyrFlix 1.4.0 est disponible publiquement en version de test gratuite. La version n'est pas qualifiée stable.**

**Status on 17 October 2026 — ZephyrFlix 1.4.0 is publicly available as a free test version. It is not qualified as stable.**

[Téléchargement officiel / Official download](https://eric-mager-lab.balmylily512.chatgpt.site/downloads/zephyrflix/) · [Manifeste de distribution / Distribution manifest](../DISTRIBUTION.json).

Le manifeste distingue `status=public-test-candidate`, `stableQualified=false` et `cleanWindowsTested=false`. Le statut historique `publicReady=false` concernait la qualification stable ; il ne signifie pas que le téléchargement de test est encore en préparation. Le feu vert à la diffusion de test ne remplace pas un essai sur une autre machine.

The manifest distinguishes `status=public-test-candidate`, `stableQualified=false` and `cleanWindowsTested=false`. The historical `publicReady=false` referred to stable qualification, not a test download still awaiting publication. Permission to share a test version is not an independent-machine test.

## Contrôles locaux consignés / Recorded local checks
Cette synthèse reprend les résultats de la session 1.4 et du manifeste public existant. Elle ne publie ni profils, médias, journaux ni rapport privé, et ne transforme pas ces résultats en nouveaux essais indépendants.

This summary reflects session 1.4 results and the existing public manifest. It exposes no private profiles, media, logs or reports and does not relabel those results as fresh independent tests.

| Contrôle local / Local check | Résultat / Result |
|---|---|
| Tests Rust / Rust tests | 33 réussis / passed |
| fmt, check, debug, release, Clippy | Réussis / passed, Clippy avec `-D warnings` |
| Interface | Catalogue, séries/saisons, filtres, favoris, paramètres, aide et crédits vérifiés / checked |
| Premier lancement / First run | Profil vierge et persistance au relancement vérifiés / fresh profile and relaunch persistence checked |
| Lecteur natif / Native playback | Lecture, pause, seek, volume, arrêt, favori et reprise vérifiés / checked |
| Plein écran / Fullscreen | F11, géométrie plein écran et retour Échap natif vérifiés / checked |
| Import facultatif / Optional import | Copie, sauvegarde, WAL et préservation de l'original vérifiés sur fixtures / checked on fixtures |
| Identité / Identity | Visuel canonique inchangé, empreinte vérifiée / canonical image unchanged and hash checked |
| Archives RC / RC archives | CRC et SHA-256 revérifiés le 17 octobre 2026 / rechecked |

Le manifeste consigne également : installation, raccourcis, réinstallation conservant la bibliothèque, désinstallation conservant le profil et retirant les raccourcis ; décodage local MP4, MKV et AVI avec le lecteur embarqué. Ces contrôles concernent la machine de développement, pas un autre Windows propre.

The manifest also records installation, shortcuts, reinstall preserving the library, uninstall preserving the profile and removing shortcuts, plus local MP4, MKV and AVI decoding with the bundled player. These checks concern the development machine, not a separate clean Windows PC.

La notice MIT de `simd_helpers` a été résolue le 17 octobre 2026 : texte amont exact, copyright 2019 Luca Barbato ; source de la crate identique au commit `82040194cd05affb060bf94d6f19f82a771d07fb`. [Texte exact](licenses/simd_helpers-MIT.txt).

The `simd_helpers` MIT notice was resolved on 17 October 2026: exact upstream text, copyright 2019 Luca Barbato, with crate source identical to the cited commit.

## Distribution publiée / Published distribution
Le **Setup x64 RC 1.4** installe pour l'utilisateur, sans droits administrateur, avec raccourcis Bureau et menu Démarrer. Il inclut le runtime VLC 3.0.24 sélectionné et les composants Visual C++ nécessaires ; aucune installation externe de VLC n'est requise pour ce Setup. Les sources tierces sont proposées séparément sur la page de téléchargement. Le profil est conservé à la désinstallation.

**Setup x64 RC 1.4** installs per user without administrator privileges, with desktop and Start menu shortcuts. It includes selected VLC 3.0.24 and the required Visual C++ components; no separate VLC installation is needed for this Setup. Third-party sources are supplied separately through the download page. Uninstall preserves the profile.

Le site et la documentation sont bilingues ; l'installateur propose français et anglais. **L'interface actuelle de l'application reste principalement en français.** The website, documentation and installer are available in English, but **the current application interface is primarily in French**.

| Artefact / Artefact | Taille / Bytes | SHA-256 |
|---|---:|---|
| `ZephyrFlix-1.4.0-Setup-x64-RC.exe` | 43 236 329 | `6549fde05786679bf76779f02ad95aa83f4407656cf7c2055268ea6ebb913593` |
| `ZephyrFlix-1.4.0-Composants-Sources.zip` | 212 253 218 | `5b6bf80768cd6d205170d456a98a89cd3ee1197c5fb0837c3bb09e479eb93dcf` |

Ces références sont celles du manifeste existant et restent inchangées ; cette correction documentaire ne remplace ni ne reconstruit les artefacts. / These references match the existing manifest and remain unchanged; this documentary correction neither replaces nor rebuilds the artefacts.

L'ancien ZIP Portable RC est distinct : il nécessite VLC 3 x64 externe et le Visual C++ x64 Redistributable si absent. Ses prérequis ne s'appliquent pas au Setup autonome. / The older Portable RC ZIP is separate and requires external VLC 3 x64 and the Visual C++ x64 Redistributable if missing; those requirements do not apply to the standalone Setup.

## Vérifications encore ouvertes / Remaining checks
- **Un autre Windows x64 propre : non testé.** Démarrage, choix et scan de dossiers d'essai, navigation, lecture réelle de plusieurs formats, plein écran, reprise et aide restent à vérifier sur cette machine indépendante. / **Separate clean Windows x64 PC: not tested.** Startup, folder selection/scanning, browsing, multiple playback formats, fullscreen, resume and help remain to be checked there.
- **TMDB authentifié : non testé avec une clé utilisateur.** Ne pas présenter l'authentification réelle comme validée. / **Authenticated TMDB: not tested using a user key.** Real authentication is not advertised as verified.
- **Certificat de signature Windows : absent.** Aucun conseil de désactivation des protections Windows. / **Windows code-signing certificate: absent.** No instruction to disable Windows protections.
- Plusieurs scénarios et fichiers ont été testés, pas tous les formats ni toutes les configurations ; aucune écoute physique systématique du son n'est revendiquée. / Multiple scenarios and files were tested, not every format or configuration; no systematic physical audio-listening check is claimed.

[README](../README.md).
