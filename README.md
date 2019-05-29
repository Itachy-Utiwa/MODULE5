PT Activity(En Français)

Packet Tracer - Mise en œuvre Home IoT
Scénario

Dans ce scénario, Packet Tracer, Bob a commencé à mettre en œuvre une solution IoT chez lui. Vous explorerez la variété de dispositifs et manipulerez les facteurs environnementaux pour voir l'impact sur les capteurs et les actionneurs. Vous allez également configurer certains paramètres de base, notamment l'adressage IP pour un capteur et les paramètres de sécurité pour le routeur de passerelle. Enfin, vous vérifierez que tous les appareils de la maison disposent d’une connectivité IP.

Partie 1: Connexion de périphériques à la passerelle domestique
Étape 1: Configurez la passerelle domestique.

une. Cliquez sur Accueil pour développer le cluster.

b. Cliquez sur Home Gateway. Cliquez sur l'onglet Config.

c. Cliquez sur Internet. Sélectionnez DHCP pour la configuration IP.

ré. Cliquez sur sans fil. Entrez MyHomeGateway en tant que SSID. Sélectionnez WPA2-PSK comme authentification. Entrez CiscoIoT en tant que phrase de passe PSK.

e. Cliquez sur Home PC. Cliquez sur le bureau. Cliquez sur Configuration IP. Sélectionnez DHCP pour la configuration IP.
Étape 2: Vérifiez la connectivité de Home Gateway au serveur d'enregistrement.

une. À partir de l'ordinateur personnel, entrez www.register.pka dans le navigateur Web. Entrez admin comme nom d'utilisateur et admin comme mot de passe pour vous connecter au serveur d'enregistrement distant.

Remarque: La liste de tous les périphériques IoT peut prendre quelques minutes.

Enumérez quelques-uns des appareils IoT:

Quelles sont les actions disponibles pour ces appareils IoT?

b. À partir de l'ordinateur personnel, entrez 192.168.25.1 dans le navigateur Web. Entrez admin en tant que nom d'utilisateur et admin en tant que mot de passe pour vous connecter au serveur IoT local hébergé sur Home Gateway.

Enumérez quelques-uns des appareils IoT:

Quelles sont les actions disponibles pour ces appareils IoT?

Partie 2: Interaction avec les appareils IoT
Étape 1: automatiser le contrôle de la température.

Actuellement, le thermostat est éteint. Réglez le thermostat pour qu’il s’ajuste automatiquement au réglage souhaité.

une. Développez la barre d'état du thermostat. Cliquez sur Auto. Entrez les températures de chauffage et de refroidissement automatiques souhaitées, puis cliquez sur Définir.

b. Observez l'élément chauffant et l'élément refroidissant pendant qu'ils ajustent la température.
Étape 2: Automatiser le ventilateur de plafond.

Le ventilateur de plafond est configuré pour ne s'allumer que lorsqu'un mouvement est détecté et qu'aucun vent n'est détecté. Le SBC0 avec l’utilisation de capteurs de mouvement et de vent contrôle l’état du ventilateur de plafond.

Alt + Cliquez sur le capteur de mouvement situé près du ventilateur de plafond. Cela activera le capteur de mouvement.

Le ventilateur de plafond s'est-il allumé?

Étape 3: Automatiser les arroseurs de pelouse.

Arroser la pelouse peut être une activité contrôlée par des instructions conditionnelles configurées dans le serveur IoT local sur la passerelle domestique.

une. Développez le statut des arroseurs de pelouse, des arroseurs de pelouse0 et de la surveillance du niveau d'eau. Observez la relation entre le niveau d'eau et le statut des arroseurs de pelouse.

Quelle condition déclenche l'allumage des arroseurs de pelouse?

Quel état déclenche l'extinction des arroseurs de pelouse?

b. Cliquez sur Conditions en haut de la page Web. Localisez les instructions conditionnelles.

Combien de déclarations conditionnelles contrôlent les arroseurs de pelouse?

Étape 4: automatiser la caméra Web.

La caméra Web est actuellement configurée pour ne s'allumer que lorsque le détecteur de mouvement est déclenché.

une. Développez le statut du détecteur de mouvement et de la caméra Web. Observez la relation entre le détecteur de mouvement et l'état de la caméra Web.

b. Alt + Cliquez sur Détecteur de mouvement dans la topologie. Assurez-vous de cliquer sur celui près de la webcam.

Qu'avez-vous vu sur Webcam dans la page Web?

Étape 5: Ouvrez Windows et la porte du garage.

Une vieille voiture est en réparation dans le garage. Un détecteur de CO, une porte de garage et des fenêtres ont été installés et configurés pour prévenir l’empoisonnement au CO.

une. Développez le statut de toutes les fenêtres, de la porte du garage et du détecteur de CO du garage. Des appareils sont-ils absents de la liste?

b. Pour le périphérique non connecté, vérifiez qu'il est configuré pour se connecter à la passerelle domestique pour le serveur IoE et que DHCP est activé pour les paramètres de configuration IP.

c. Démarrez la vieille voiture avec Alt + Cliquez sur la voiture dans le garage et regardez le niveau de CO augmenter dans le garage.

ré. Alt + Cliquez sur la voiture pour éteindre la vieille voiture.

e. Observez l’interaction des fenêtres et de la porte du garage avec le niveau de CO dans le garage.
Étape 6: Suppression des incendies

Un système d'extinction d'incendie IoT a été installé dans chacune des chambres et dans la cuisine. Dans cette démonstration IoT, il y aura un incendie simulé pendant votre absence et vous pourrez observer le fonctionnement de la suppression des incendies à l'aide de l'état des détecteurs de fumée.

une. Quittez le cluster d'accueil en cliquant sur Précédent. Cliquez sur le cluster ISP-Internet pour le saisir.

b. Depuis votre smartphone, entrez www.register.pka dans le navigateur Web. Entrez admin comme nom d'utilisateur et admin comme mot de passe pour vous connecter au serveur IoT local hébergé sur le serveur d'enregistrement.

Remarque: Plusieurs tentatives peuvent être nécessaires avant que la page Web ne s’affiche.

c. Développez tous les statuts des détecteurs de fumée. Des appareils sont-ils absents de la liste?

ré. Simulez un feu dans la cuisine. Qu'advient-il des détecteurs de fumée?

Décrivez ce qui se passe ensuite.

e. Commencez une simulation d'incendie à d'autres endroits pour observer ce qui se passe.

Étape 7: enquête complémentaire

une. Au cours de l'étape précédente, vous avez constaté que Home Gateway et Registration Server peuvent être utilisés pour contrôler les périphériques IoT à distance. Vous pouvez modifier le mode d'accès à ces périphériques à distance.

1) Cliquez sur le périphérique.

2) Dans l'onglet Périphérique, sélectionnez Aucun, Passerelle domestique ou Serveur distant. Pour l'activité, l'adresse du serveur est www.register.pka (209.165.201.10) et admin comme nom d'utilisateur et mot de passe.

3) Sur le serveur, vous pouvez ajouter des instructions conditionnelles pour les périphériques capables de configurations exploitables.

b. Si vous souhaitez programmer les périphériques d'extrémité IoT, cliquez sur le périphérique, puis sur Avancé. Sélectionnez la programmation. Sélectionnez les fichiers souhaités et passez en revue les codes.
