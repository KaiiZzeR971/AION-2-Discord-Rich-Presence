# AION 2 Discord Rich Presence for Windows 10/11

**English** · [Français](#français)

Show your **AION 2** session on Discord with a dedicated Windows app. It starts quietly with the game, uses the game's session time, and closes when the game exits. Game process detection supports **Global, Taiwan (TW), and Korea (KR)** clients. Automatic character name detection from the game window title has been verified on TW.

## Download and install

1. Download [AionPresence-Setup-0.7.1.exe](https://github.com/KaiiZzeR971/AION-2-Discord-Rich-Presence/releases/download/v0.7.1/AionPresence-Setup-0.7.1.exe).
2. Run the installer on Windows 10 or 11. Open **AION 2 Discord Presence** from the Start menu once to set up automatic launch.
3. Keep the Discord desktop app open. A shared Discord Application ID and presence artwork are configured by default. Choose your language and visibility settings in the app.
4. To detect a Global character automatically, install [Npcap from its official site](https://npcap.com/#download) separately. In its installer, enable **WinPcap API-compatible Mode** and leave **Restrict Npcap driver's access to Administrators only** off. Reopen the presence app afterward.

Installation is required; no PowerShell window opens. The installer is currently **unsigned**, so Windows may display a warning. You can verify the download with its [SHA-256 checksum](https://github.com/KaiiZzeR971/AION-2-Discord-Rich-Presence/releases/download/v0.7.1/AionPresence-Setup-0.7.1.sha256).

## Screenshots

![AION 2 Discord Presence overview](images/overview-en.png)

![AION 2 Discord Presence settings](images/settings-en.png)

![Update settings with automatic updates off by default](images/updates-en.png)

![Visibility settings, including the GitHub button](images/visibility-en.png)

## Features

- Automatic launch to the notification area with `Aion2.exe`, and automatic exit when the game closes.
- Character name from the game window title when available, with a manual fallback.
- Global Steam client detection using its `Saved_Steam` folder. With Npcap installed, the app reads the current character name and class from the game's local network traffic. It has been verified on the EU Israphel server. The saved name and class fields remain available as fallbacks.
- Timer based on the game process start time, preserved when the presence app restarts.
- French or English interface and presence, with individual visibility controls.
- Global EU, NA, SA and JP server regions, plus TW and KR client detection.
- Game image and class icons, including Brawler, in the Discord presence.
- A Discord button linking to this project's latest GitHub download page. Enabled by default; switch it off in Settings → Visibility.
- Check and install updates in the app. Automatic installation is available in Settings → Updates and is off by default. Downloaded installers are checked against GitHub's SHA-256 digest.
- Local preview, saved preferences, and configurable close button behavior.

The EU Israphel server name is recognized from its verified game server ID. Other Global server names can be entered once as a fallback until their IDs are confirmed. A fresh login or zone transition may be needed before the game sends character identity while the app is running. The detected identity is kept for the current game session, including when the presence app restarts. Level, equipment level, zone, and party are not yet confirmed on Global; they stay hidden unless a compatible profile data source supplies them. Npcap is not bundled with this installer.

## FAQ

**Do I need to create a Discord application?** No. A shared Application ID is included. You can enter your own ID in Settings if you prefer.

**Does the app need to stay open?** It can remain in the notification area. After its first launch, a lightweight watcher starts with Windows and opens the presence app only when the game starts.

**Why can't I see the GitHub button on my own Discord presence?** [Discord shows Rich Presence buttons only to other users](https://docs.discord.com/developers/discord-social-sdk/development-guides/setting-rich-presence#setting-buttons). Ask a friend or use a second account to view your profile and check the button.

**How do updates work?** Use Settings → Updates to check and install. When automatic updates are enabled, the app checks at most every six hours and installs a newer release if available. The app briefly closes while the installer replaces it, then restarts.

**How do I uninstall it?** Use **Windows Settings → Installed apps → AION 2 Discord Presence**.

**How can I report a problem?** Open an [issue](https://github.com/KaiiZzeR971/AION-2-Discord-Rich-Presence/issues) with your Windows version, game client region, and a description. Please do not attach personal data.

---

## Français

Affichez votre session **AION 2** sur Discord avec une application Windows dédiée. La présence démarre discrètement avec le jeu, utilise son temps de session et disparaît quand vous le quittez. La détection du processus prend en charge les clients **Global, Taïwan (TW) et Corée (KR)**. La lecture automatique du nom du personnage dans le titre de la fenêtre a été vérifiée sur TW.

### Télécharger et installer

1. Téléchargez [AionPresence-Setup-0.7.1.exe](https://github.com/KaiiZzeR971/AION-2-Discord-Rich-Presence/releases/download/v0.7.1/AionPresence-Setup-0.7.1.exe).
2. Lancez l'installateur sur Windows 10 ou 11, puis ouvrez une fois **AION 2 Discord Presence** depuis le menu Démarrer pour activer le lancement automatique.
3. Gardez l'application Discord de bureau ouverte. L'Application ID partagé et les images de la présence sont déjà configurés. Choisissez la langue et les informations affichées dans les paramètres.
4. Pour détecter automatiquement le personnage sur Global, installez [Npcap depuis son site officiel](https://npcap.com/#download) séparément. Pendant l'installation, activez **WinPcap API-compatible Mode** et laissez **Restrict Npcap driver's access to Administrators only** désactivé. Rouvrez ensuite l'application.

L'installation est requise et aucune fenêtre PowerShell ne s'ouvre. L'installateur est actuellement **non signé** ; Windows peut afficher un avertissement. Vérifiez le fichier téléchargé avec sa [somme SHA-256](https://github.com/KaiiZzeR971/AION-2-Discord-Rich-Presence/releases/download/v0.7.1/AionPresence-Setup-0.7.1.sha256).

### Captures d'écran

![Vue d'ensemble de l'application](images/overview-fr.png)

![Paramètres de l'application](images/settings-fr.png)

![Paramètres des mises à jour automatiques désactivées par défaut](images/updates-fr.png)

![Options de visibilité avec le bouton GitHub](images/visibility-fr.png)

### Fonctions

- Démarrage automatique et discret dans la zone de notification avec `Aion2.exe` ; arrêt à la fermeture du jeu.
- Nom du personnage lu dans le titre de la fenêtre du jeu lorsque le client le fournit, avec un champ de secours.
- Détection du client Global Steam grâce au dossier `Saved_Steam`. Avec Npcap installé, l'application lit le nom et la classe du personnage actif dans le trafic réseau local du jeu. Cette lecture a été vérifiée sur le serveur EU Israphel. Les champs enregistrés restent disponibles comme secours.
- Chrono fondé sur l'heure de démarrage du jeu, conservé si l'application de présence redémarre.
- Interface et présence en français ou en anglais, avec choix individuel des informations affichées.
- Régions Global EU, NA, SA et JP, ainsi que détection des clients TW et KR.
- Image du jeu et icônes des classes, dont Brawler, dans la présence Discord.
- Bouton Discord vers la page GitHub de la dernière version. Il est activé par défaut et désactivable dans **Paramètres → Visibilité**.
- Recherche et installation des mises à jour depuis l'application. L'installation automatique est disponible dans **Paramètres → Mises à jour** et désactivée par défaut. L'installateur téléchargé est vérifié avec l'empreinte SHA-256 fournie par GitHub.
- Aperçu local, préférences sauvegardées et comportement du bouton de fermeture au choix.

Le nom du serveur EU Israphel est reconnu à partir de son identifiant vérifié dans le jeu. Les autres serveurs Global peuvent être saisis une fois en attendant la validation de leurs identifiants. Une reconnexion ou un changement de zone peut être nécessaire pour que le jeu transmette l'identité pendant que l'application est ouverte. L'identité détectée reste associée à la session de jeu, même si l'application redémarre. Le niveau, le niveau d'équipement, la zone et le groupe ne sont pas encore confirmés sur Global : ils restent masqués sans source de profil compatible. Npcap n'est pas inclus dans l'installateur.

### Questions courantes

**Faut-il créer une application Discord ?** Non. Un Application ID partagé est intégré. Vous pouvez saisir le vôtre dans les paramètres.

**L'application doit-elle rester ouverte ?** Elle peut rester dans la zone de notification. Après sa première ouverture, un surveillant léger démarre avec Windows et ouvre l'application seulement lorsque le jeu se lance.

**Pourquoi le bouton GitHub n'apparaît-il pas sur ma propre présence Discord ?** [Discord affiche les boutons Rich Presence uniquement aux autres utilisateurs](https://docs.discord.com/developers/discord-social-sdk/development-guides/setting-rich-presence#setting-buttons). Demandez à un ami ou utilisez un second compte pour vérifier le bouton sur votre profil.

**Comment se font les mises à jour ?** Utilisez **Paramètres → Mises à jour** pour rechercher et installer. Si l'option automatique est activée, l'application vérifie au plus toutes les six heures et installe une nouvelle version disponible. Elle se ferme brièvement pendant l'installation, puis redémarre.

**Comment la désinstaller ?** Dans **Paramètres Windows → Applications installées → AION 2 Discord Presence**.

**Où signaler un problème ?** Ouvrez une [issue](https://github.com/KaiiZzeR971/AION-2-Discord-Rich-Presence/issues) avec la version de Windows, la région du client et une description du problème, sans données personnelles.

---

Unofficial fan application / Application de fans non officielle. Not affiliated with NCSOFT or Discord / Sans affiliation avec NCSOFT ou Discord. © 2026 KaiiZzeR971. [License notice](LICENSE.txt).
