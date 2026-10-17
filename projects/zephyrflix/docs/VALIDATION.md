# État de validation / Validation status

**Référence : 17 octobre 2026 — ZephyrFlix 1.4.0. `publicReady=false` pour une diffusion stable. Une publication distincte comme **version de test gratuite** a été explicitement autorisée.**

Cette synthèse publique reprend les résultats de validation locale de la session 1.4. Elle ne publie ni profils, médias, journaux ni rapport privé. Les valeurs ci-dessous ne sont pas un nouvel essai indépendant.

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

## Vérifications encore ouvertes / Remaining checks
- Test sur **un autre Windows x64 propre**, avec installation des prérequis si nécessaire, lancement, sélection et scan de dossiers d'essai, navigation, lecture réelle de plusieurs formats, plein écran, reprise et aide. **Non réalisé / Not performed.**
- **Notice `simd_helpers` résolue le 17 octobre 2026** : texte MIT amont retrouvé, copyright 2019 Luca Barbato ; source de la crate identique au commit `82040194cd05affb060bf94d6f19f82a771d07fb`. [Texte exact](licenses/simd_helpers-MIT.txt). / **Notice resolved**: upstream MIT text recovered, crate source identical to the cited commit.
- Setup x64 RC 1.4 : runtime VLC 3.0.24 sélectionné avec filtrage GPL et runtime Visual C++ inclus ; notices dans le paquet et sources tierces distribuées séparément. Validation finale du Setup suivie dans sa propre fiche de distribution. / Selected VLC 3.0.24 with GPL filtering and Visual C++ included; notices in package and third-party sources provided separately. Final Setup verification is recorded in its own distribution report.
- Authentification TMDB avec une clé utilisateur si présentée comme validée en conditions réelles. / User-key authentication if advertised as validated.
- Instructions de la distribution et contrôle de l'artefact téléchargé depuis le futur canal officiel. / Distribution instructions and download integrity through the future official channel.
- Publication RC de test autorisée par Eric le 17 octobre 2026 ; [canal officiel](https://eric-mager-lab.balmylily512.chatgpt.site/downloads/zephyrflix/). Ce feu vert ne vaut pas validation sur une autre machine. / Test RC publication authorised by Eric; [official channel](https://eric-mager-lab.balmylily512.chatgpt.site/downloads/zephyrflix/). This approval is not an independent-machine test.

Le ZIP Portable RC initial demande VLC 3 x64 externe et le Visual C++ x64 Redistributable si absent. Le Setup x64 RC 1.4 est distinct : installation français/anglais par utilisateur, sans administration, raccourcis Bureau et menu Démarrer, lecteur et runtime inclus ; profil conservé à la désinstallation. Les contrôles spécifiques au Setup sont suivis séparément et ne valent pas test sur une autre machine. L'exécutable n'est pas signé par un certificat de code Windows.

The original Portable RC ZIP requires external VLC 3 x64 and the Visual C++ x64 Redistributable if missing. Setup x64 RC 1.4 is separate: French/English per-user installation without elevation, desktop and Start menu shortcuts, included player/runtime, and profile preservation on uninstall. Setup-specific checks are tracked separately and do not constitute testing on another machine. The executable has no Windows code-signing certificate.

Plusieurs scénarios et fichiers ont été testés, pas tous les formats ni toutes les configurations. Aucun test local ne remplace la machine indépendante. / Multiple local scenarios and files were tested, not every format or configuration. Local testing does not replace an independent machine.

[README](../README.md).
