# Composants tiers / Third-party components — ZephyrFlix 1.4

Les composants gardent leurs auteurs et licences propres. Le code réservé de ZephyrFlix ne limite aucun droit accordé par leurs licences. Ce dossier documentaire ne contient pas le code propre de l'application. Les notices détaillées accompagnent le Setup ; les sources des composants tiers redistribués sont proposées séparément sur la page officielle de téléchargement.

Components retain their own authors and licences. ZephyrFlix's reserved code does not restrict any rights granted by those licences. This documentary folder does not contain the application’s own source code. Detailed notices accompany Setup; sources of redistributed third-party components are provided separately through the official download page.

| Composant / Component | Attribution / Conditions |
|---|---|
| Slint 1.17.1 | SixtyFPS GmbH ; [Slint Royalty-free 2.0](https://slint.dev/agreements/slint-royalty-free-license.pdf), application desktop ; widget AboutSlint dans les crédits / in application credits |
| SQLite | [SQLite authors](https://www.sqlite.org/copyright.html), domaine public / public domain ; bindings Rust avec notices propres / separate Rust binding notices |
| Crates Rust | Inventaire exact verrouillé et notices dans le paquet candidat / locked inventory and notices in candidate package |
| option-ext 0.2.0 | [Auteurs amont / upstream authors](https://crates.io/crates/option-ext), MPL-2.0 ; source non modifiée prévue dans les notices du paquet / unchanged source included with package notices |
| simd_helpers 0.1.0 | [Luca Barbato / upstream](https://github.com/lu-zero/simd_helpers/blob/82040194cd05affb060bf94d6f19f82a771d07fb/LICENSE), copyright 2019 ; [texte MIT exact](docs/licenses/simd_helpers-MIT.txt) retrouvé, source de la crate 0.1.0 identique / exact MIT text recovered, crate 0.1.0 source identical |
| libVLC / VLC | [VideoLAN and contributors](https://www.videolan.org), liaison dynamique / dynamic loading ; Setup : runtime sélectionné 3.0.24 avec plugins GPL filtrés, notices et sources tierces séparées / Setup: selected 3.0.24 runtime with GPL plugins filtered, notices and separate third-party sources |
| Montserrat | Montserrat.Git Project Authors ; [SIL Open Font License 1.1](docs/licenses/Montserrat-OFL.txt) |
| Logo et service TMDB | [TMDB attribution](https://developer.themoviedb.org/docs/faq), clé personnelle facultative / optional personal key |
| Logo, Kitsune et visuels ZephyrFlix | Eric Mager / Terrelfe ; [crédits et droits / credits and rights](docs/CREDITS.md) |

This product uses the TMDB API but is not endorsed or certified by TMDB.

Le **Setup x64 RC 1.4** inclut le runtime VLC 3.0.24 sélectionné avec filtrage des plugins GPL, et le runtime Microsoft Visual C++. Les sources tierces concernées sont fournies dans un paquet séparé sur la [page officielle](https://eric-mager-lab.balmylily512.chatgpt.site/downloads/zephyrflix/) ; elles n'accordent aucune licence sur le code propre ZephyrFlix. Le ZIP Portable RC initial reste distinct et ne contient aucun de ces runtimes.

**Setup x64 RC 1.4** includes selected VLC 3.0.24 with GPL plugins filtered and the Microsoft Visual C++ runtime. Relevant third-party sources are supplied in a separate package on the [official page](https://eric-mager-lab.balmylily512.chatgpt.site/downloads/zephyrflix/); they grant no licence over ZephyrFlix’s own code. The initial Portable RC ZIP is separate and contains neither runtime.

[État de validation / Validation status](docs/VALIDATION.md) · [Conditions / Terms](LICENSE.md).
