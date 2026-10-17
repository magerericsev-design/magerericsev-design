# Architecture — aperçu / overview

## Français
Application Windows native en Rust, interface Slint, bibliothèque SQLite et lecteur libVLC chargé dynamiquement. Les fichiers vidéo physiques et les œuvres du catalogue sont distincts : une série rassemble ses saisons et épisodes, les favoris appartiennent à l'œuvre et la progression à chaque fichier.

Le scan est incrémental et ne renomme ni ne déplace les vidéos. Les métadonnées facultatives et les miniatures passent par des tâches d'arrière-plan. Les corrections manuelles restent protégées ; les suggestions incertaines attendent une confirmation. Le cache est local, les téléchargements sont bornés et les clés restent dans le gestionnaire d'identifiants Windows.

Les données utilisateur sont séparées des fichiers de l'application. Les évolutions de schéma sont sauvegardées ; l'import d'une ancienne bibliothèque travaille sur une copie. Le lecteur rend la vidéo dans une surface native Windows. Le code propre et les détails internes de l'atelier restent privés.

## English
Native Windows application using Rust, Slint, SQLite and dynamically loaded libVLC. Physical video files are separate from catalogue works: a series groups seasons and episodes; favourites belong to the work while progress belongs to each file.

Scanning is incremental and does not move or rename videos. Optional metadata and thumbnails use background tasks. Manual corrections remain protected; uncertain suggestions require confirmation. Caching is local, downloads are bounded and keys stay in Windows Credential Manager.

User data is separate from application files. Schema updates are backed up; legacy import uses a copy. Playback renders in a native Windows surface. Own source code and internal workshop details remain private.

[README](../README.md).
