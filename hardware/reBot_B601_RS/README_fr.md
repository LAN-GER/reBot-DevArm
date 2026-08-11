# 🤖 Spécification matérielle open source du reBot DevArm

<p align="center">
  <img src="../../media/RS5_56.png" alt="Bannière reBot-DevArm">
</p>
<p align="center">
  <strong>
    <a href="./README_zh.md">简体中文</a> &nbsp;|&nbsp;
    <a href="./README.md">English</a> &nbsp;|&nbsp;
    <a href="./README_fr.md">français</a>&nbsp;|&nbsp;
    <a href="./README_es.md">Español</a>
  </strong>
</p>

| Date       | Version | Nom du fichier                   | Journal des modifications |
| ---------- | ------- | -------------------------------- | ------------------------- |
| 2026-07-09 | v1.0    | reBot_B601_RS_v1.0_20260625.step | Première mise en ligne    |

Cette BOM concerne le bras robotique reBot Arm B601 RS, qui utilise des moteurs de la série ROBOSTRIDE. L’autre version, reBot Arm B601 DM, utilise des moteurs DAMIAO ; [voir la BOM ici](../reBot_B601_DM/readme.md).

# 📦 Structure des fichiers

* `3D_Printed_Parts/` : fichiers STEP de toutes les pièces imprimées en 3D.
* `Metal_Parts/` : fichiers STEP de toutes les pièces métalliques usinées CNC.
* `Purchased_Parts/` : fichiers STEP de tous les composants achetés.
* `reBot_B601_RS_v1.0_20260625.step` : fichier d’assemblage complet du bras robotique.

# 🛒[Obtenir toutes les pièces](https://www.seeedstudio.com/reBot-Arm-B601-RS-Disassembly-Kit-Version-with-Power-Supply-Bundle.html)

* Nous proposons cinq options de kits :

  * **reBot-Arm-B601-RS-Disassembly-Kit**
  * **reBot-Arm-B601-RS-Assembly-Version**

# 📊 Nomenclature — Bill of Materials (BOM)

> [!WARNING]
> Déclaration : la BOM publiée **ne représente pas** la version finale expédiée par Seeed. Cette version open source v1.0 est optimisée pour permettre aux développeurs de la reproduire à moindre coût, avec certains détails non essentiels simplifiés.
>
> La version finale de production Seeed inclura une gravure laser sur les pièces métalliques pour faciliter l’assemblage et éviter les erreurs, certaines pièces imprimées en 3D seront remplacées par des pièces métalliques pour améliorer la durabilité, les jeux et tolérances d’usinage seront ajustés en fonction des variations de fabrication en usine, et un câblage personnalisé, par exemple avec gaine tressée de protection, sera ajouté moyennant un coût supplémentaire. Cependant, la structure mécanique reste identique.

---

## 🖨️ Pièces imprimées en 3D

| Description de la pièce                                   | Image                                                                   | Nom du fichier       | Matériau               | Qté | Remarques                                                                                                                                 |
| --------------------------------------------------------- | ----------------------------------------------------------------------- | -------------------- | ---------------------- | --- | ----------------------------------------------------------------------------------------------------------------------------------------- |
| Plateforme de base du bras robotique                      | <img src="./3D_Printed_Parts/images/02-BASE.png" width="80">            | 1-BASE-PLATE.step    | Bambu ABS noir         | 1   | Buse 0,4 mm, hauteur de couche 0,2 mm, remplissage 30 %                                                                                   |
| Maillon de base du bras robotique                         | <img src="./3D_Printed_Parts/images/02-BASE_02.png" width="80">         | 1-RSM1-STATOR-1.step | Bambu ABS noir         | 1   | Buse 0,4 mm, hauteur de couche 0,2 mm, remplissage 30 %                                                                                   |
| Garniture gauche du bras supérieur                        | <img src="./3D_Printed_Parts/images/02-DOWN_TRIM_1.png" width="80">     | 1-DOWN-DL.step       | Bambu PLA noir et vert | 1   | Buse 0,4 mm, hauteur de couche 0,2 mm, remplissage 15 %                                                                                   |
| Garniture droite du bras supérieur                        | <img src="./3D_Printed_Parts/images/02-DOWN_TRIM_2.png" width="80">     | 1-DOWN-DR.step       | Bambu PLA noir et vert | 1   | Buse 0,4 mm, hauteur de couche 0,2 mm, remplissage 15 %                                                                                   |
| Garniture centrale du bras supérieur et du bras inférieur | <img src="./3D_Printed_Parts/images/02-DOWN-FILLING.png" width="80">    | 1-SPACE-UP.step      | Bambu ABS noir         | 2   | Buse 0,4 mm, hauteur de couche 0,2 mm, remplissage 30 %                                                                                   |
| Poignée du bras                                           | <img src="./3D_Printed_Parts/images/02-HANDLE.png" width="80">          | 1-HANDLE.step        | Bambu ABS noir         | 1   | Buse 0,4 mm, hauteur de couche 0,2 mm, remplissage 30 %                                                                                   |
| Capot du bras supérieur et du bras inférieur              | <img src="./3D_Printed_Parts/images/02-DOWN-COVER.png" width="80">      | 1-COVER.step         | Bambu PLA vert         | 2   | Buse 0,4 mm, hauteur de couche 0,2 mm, remplissage 15 %                                                                                   |
| Garniture gauche du bras inférieur                        | <img src="./3D_Printed_Parts/images/02-UP-TRIM_1.png" width="80">       | 1-UP-DL.step         | Bambu PLA noir et vert | 1   | Buse 0,4 mm, hauteur de couche 0,2 mm, remplissage 15 %                                                                                   |
| Garniture droite du bras inférieur                        | <img src="./3D_Printed_Parts/images/02-UP-TRIM_2.png" width="80">       | 1-UP-DR.step         | Bambu PLA noir et vert | 1   | Buse 0,4 mm, hauteur de couche 0,2 mm, remplissage 15 %                                                                                   |
| Butée horizontale de la pince                             | <img src="./3D_Printed_Parts/images/02-SPACER.png" width="80">          | 1-STOPPER-1.step     | Bambu PLA vert         | 1   | Buse 0,4 mm, hauteur de couche 0,2 mm, remplissage 15 %                                                                                   |
| Support de rail coulissant de la pince                    | <img src="./3D_Printed_Parts/images/02-3D-RAIL-BRACKET.png" width="80"> | 1-RAIL-BASE-2.step   | Bambu PLA vert         | 1   | Buse 0,4 mm, hauteur de couche 0,2 mm, remplissage 15 %                                                                                   |
| Doigt de pince                                            | <img src="./3D_Printed_Parts/images/02-CLIP_1.png" width="80">          | 1-CLIP.step          | Bambu ABS noir         | 2   | Buse 0,4 mm, hauteur de couche 0,2 mm, remplissage 45 %. Imprimer depuis le côté de la pince afin d’améliorer la résistance structurelle. |

Le frottement prolongé du faisceau de câbles 1 peut user le connecteur du moteur et entraîner un mauvais contact électrique. L’impression des pièces listées ci-dessous permet de réduire ce risque.

| Description de la pièce                                     | Image                                                                              | Nom du fichier                      | Matériau           | Qté | Remarques                                               |
| ----------------------------------------------------------- | ---------------------------------------------------------------------------------- | ----------------------------------- | ------------------ | --- | ------------------------------------------------------- |
| Clips de faisceau de câbles pour les deux côtés du moteur 1 | <img src="./3D_Printed_Parts/images/RS_Motor1_wiring_harness_clip.jpg" width="80"> | `RS_Motor1_wiring_harness_clip.stp` | Bambu Lab ABS noir | 2   | Buse 0,4 mm, hauteur de couche 0,2 mm, remplissage 30 % |

### 🧩 Recommandations d’impression

* Hauteur de couche : 0,2 mm
* Buse : 0,4 mm
* Supports : à ajouter si nécessaire
* Matériaux : les pièces exposées à la chaleur ou aux charges doivent utiliser de l’ABS avec 30 à 80 % de remplissage ; le nylon ou les matériaux renforcés en fibre de carbone peuvent également être utilisés. Les pièces esthétiques peuvent utiliser du PLA avec 15 % de remplissage.
* Matériaux recommandés pour les pièces porteuses :

---

## 🔩 Pièces métalliques usinées CNC

> [!WARNING]
> Certaines pièces pouvant être remplacées par de l’impression 3D sont indiquées dans les remarques, ce qui permet de réduire considérablement les coûts.

| Description de la pièce                    | Image                                                                      | Nom du fichier        | Matériau                 | Qté | Usinage | Remarques                                                                                                                                                                                                                                                                                             |
| ------------------------------------------ | -------------------------------------------------------------------------- | --------------------- | ------------------------ | --- | ------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Support de roulement du moteur 1           | <img src="./Metal_Parts/images/02_Base_Reinforcement_Part.png" width="80"> | 2-RSM1-ROTOR-1.step   | Alliage d’aluminium 5052 | 1   | CNC     |                                                                                                                                                                                                                                                                                                       |
| Pièce métallique gauche Link1              | <img src="./Metal_Parts/images/Link1_Left_Metal.png" width="80">           | 2-RSM-ROTOR-L.step    | Alliage d’aluminium 5052 | 1   | CNC     |                                                                                                                                                                                                                                                                                                       |
| Pièce métallique droite Link1              | <img src="./Metal_Parts/images/Link1_Right_Metal.png" width="80">          | 2-RSM-ROTOR-R.step    | Alliage d’aluminium 5052 | 4   | CNC     |                                                                                                                                                                                                                                                                                                       |
| Pièce métallique inférieure Link1          | <img src="./Metal_Parts/images/Link1_Bottom_Metal.png" width="80">         | 2-RSM1-ROTOR-1.step   | Alliage d’aluminium 5052 | 3   | CNC     |                                                                                                                                                                                                                                                                                                       |
| Disque métallique d’articulation           | <img src="./Metal_Parts/images/2-CD.png" width="80">                       | 2-CD.step             | Alliage d’aluminium 5052 | 3   | CNC     | Utilisé pour masquer les vis                                                                                                                                                                                                                                                                          |
| Extension avant RS06                       | <img src="./Metal_Parts/images/RS06_Front_Extesnion.png" width="80">       | 2-RSM2-STATOR-1.step  | Alliage d’aluminium 5052 | 1   | CNC     |                                                                                                                                                                                                                                                                                                       |
| Extension arrière RS06                     | <img src="./Metal_Parts/images/RS06_Back_Extesnion.png" width="80">        | 2-RSM2-STATOR-2.step  | Alliage d’aluminium 5052 | 1   | CNC     |                                                                                                                                                                                                                                                                                                       |
| Pièces métalliques gauche et droite Link2  | <img src="./Metal_Parts/images/2-LINK-2_3.png" width="80">                 | 2-LINK-2_3.step       | Alliage d’aluminium 5052 | 2   | CNC     |                                                                                                                                                                                                                                                                                                       |
| Butée supérieure L                         | <img src="./Metal_Parts/images/Upper_limit_L.png" width="80">              | 2-Upper-Limit_L.stp   | Alliage d’aluminium 5052 | 1   | CNC     |                                                                                                                                                                                                                                                                                                       |
| Butée supérieure R                         | <img src="./Metal_Parts/images/Upper_limit_R.png" width="80">              | 2-Upper-Limit_R.stp   | Alliage d’aluminium 5052 | 1   | CNC     |                                                                                                                                                                                                                                                                                                       |
| Liaison bras inférieur et bras supérieur L | <img src="./Metal_Parts/images/2-RSM3-ROTATOR-L.png" width="80">           | 2-RSM3-ROTATOR-L.step | Alliage d’aluminium 5052 | 1   | CNC     |                                                                                                                                                                                                                                                                                                       |
| Liaison bras inférieur et bras supérieur R | <img src="./Metal_Parts/images/2-RSM3-ROTATOR-R.png" width="80">           | 2-RSM3-ROTATOR-R.step | Alliage d’aluminium 5052 | 1   | CNC     |                                                                                                                                                                                                                                                                                                       |
| Pièce métallique gauche Link3              | <img src="./Metal_Parts/images/Link3-Left-Metal.png" width="80">           | 2-LINK-3_4-L.step     | Alliage d’aluminium 5052 | 1   | CNC     |                                                                                                                                                                                                                                                                                                       |
| Pièce métallique droite Link3              | <img src="./Metal_Parts/images/Link3-Right-Metal.png" width="80">          | 2-LINK-3_4-R.step     | Alliage d’aluminium 5052 | 1   | CNC     |                                                                                                                                                                                                                                                                                                       |
| Liaison gauche et droite Link3             | <img src="./Metal_Parts/images/Link3-Right-Left-Link.png" width="80">      | 2-SPACE-UP-2.step     | Alliage d’aluminium 5052 | 1   | CNC     |                                                                                                                                                                                                                                                                                                       |
| Fixation de câble pour moteurs 4 à 7       | <img src="./Metal_Parts/images/Motor4_Cable_Fixing.png" width="80">        | 1-O-CLIP.step         | Alliage d’aluminium 5052 | 4   | CNC     | Seeed Studio expédie cette pièce comme un composant métallique CNC intégré à une autre pièce, ce qui augmente le coût de fabrication. Si vous reproduisez le matériel vous-même, vous pouvez imprimer cette pièce en ABS et installer des écrous M2 aux emplacements indiqués par les flèches rouges. |
| Motor4 Back Cable | <img src="./Metal_Parts/images/02_Motor_Back_Spacer.png" width="80"> | 2-Motor_Back_Spacer.step | Alliage d’aluminium 5052 | 1 | CNC |  |
| Link4-5_L                                  | <img src="./Metal_Parts/images/Link4-5_L.png" width="80">                  | 2-LINK-4_5-L.step     | Alliage d’aluminium 5052 | 1   | CNC     |                                                                                                                                                                                                                                                                                                       |
| Link4-5_R                                  | <img src="./Metal_Parts/images/Link4-5_R.png" width="80">                  | 2-LINK-4_5-R.step     | Alliage d’aluminium 5052 | 1   | CNC     |                                                                                                                                                                                                                                                                                                       |
| Link5                                      | <img src="./Metal_Parts/images/Link5.png" width="80">                      | 2-RSM5-STATOR.step    | Alliage d’aluminium 5052 | 1   | CNC     |                                                                                                                                                                                                                                                                                                       |
| Connecteur de poignet A                    | <img src="./Metal_Parts/images/Wrist_Connector_A.png" width="80">          | 2-RSM6-RORATOR-1.step | Alliage d’aluminium 5052 | 1   | CNC     |                                                                                                                                                                                                                                                                                                       |
| Connecteur de poignet B                    | <img src="./Metal_Parts/images/Wrist_Connector_B.png" width="80">          | 2-RSM6-RORATOR-2.step | Alliage d’aluminium 5052 | 1   | CNC     |                                                                                                                                                                                                                                                                                                       |
| Connecteur de pince A                      | <img src="./Metal_Parts/images/02_Gripper_Connector_A.png" width="80">     | 2-M6-ROTOR.step       | Alliage d’aluminium 5052 | 1   | CNC     |                                                                                                                                                                                                                                                                                                       |
| Connecteur de pince B                      | <img src="./Metal_Parts/images/02_Gripper_Connector_B.png" width="80">     | 2-M7-STATOR.step      | Alliage d’aluminium 5052 | 1   | CNC     |                                                                                                                                                                                                                                                                                                       |
| Support métallique du coulisseau de pince  | <img src="./Metal_Parts/images/02_Slider_Bracket.png" width="80">          | 2-RAIL-BASE-1.step    | Alliage d’aluminium 5052 | 1   | CNC     | Peut être imprimé en ABS avec un fort taux de remplissage, mais n’est pas recommandé pour une utilisation à long terme                                                                                                                                                                                |
| Extension du coulisseau vers la pince      | <img src="./Metal_Parts/images/02_Slider_Extension.png" width="80">        | 2-SLIDER-FIX.step     | Alliage d’aluminium 5052 | 2   | CNC     |                                                                                                                                                                                                                                                                                                       |
| Crémaillère                                | <img src="./Metal_Parts/images/Rack.png" width="80">                       | 2-RACK-1M.step        | Alliage d’aluminium 5052 | 2   | CNC     |                                                                                                                                                                                                                                                                                                       |

### 🧩 Spécifications d’usinage

* Tolérance des dimensions critiques : ±0,02 mm, GB/T1840-M
* Finition de surface : anodisation / sablage
* Ajustement recommandé pour les pièces d’assemblage : H7 / ajustement serré

---

## 🛒 Pièces achetées — pièces standard

> [!WARNING]
> Comme chaque utilisateur devra assembler et serrer les vis lui-même, des vis à six pans creux standard ont été sélectionnées. Après une utilisation prolongée, les vis peuvent se desserrer, ce qui affectera la précision du bras robotique. Il est donc recommandé d’acheter de la colle thermofusible supplémentaire afin de verrouiller les filetages des vis au niveau de chaque articulation.
>
> Si vous disposez d’une perceuse électrique ou d’un outil similaire, vous pouvez également utiliser des rondelles frein ou des vis freinées. Cependant, il est **extrêmement important** d’utiliser le réglage de couple le plus faible avec un tournevis électrique afin d’éviter d’endommager les filetages, ce qui pourrait provoquer des dommages irréversibles.

| Nom                                         | Spécification / modèle                         | Quantité | Prix indicatif                                       | Remarques                                              |
| ------------------------------------------- | ---------------------------------------------- | -------- | ---------------------------------------------------- | ------------------------------------------------------ |
| Moteur brushless                            | RobStride RS00                                 | 4        | 125 $/unité                                          | SeeedStudio                                            |
| Moteur brushless                            | RobStride RS06                                 | 3        | 210 $/unité                                          | SeeedStudio                                            |
| Carte pilote CAN-USB                        |                                                | 1        | 15 $/unité                                           | SeeedStudio                                            |
| Carte de séparation d’alimentation XT30 2+2 |                                                | 1        | 15 $/unité                                           | SeeedStudio                                            |
| Roulement                                   | 6803ZZ                                         | 3        | 13 $/unité                                           | Amazon                                                 |
| Roulement                                   | AXK5578                                        | 1        | 12 $/unité                                           | Amazon                                                 |
| Rail linéaire                               | MGN9-170mm                                     | 1        | 23 $/unité                                           | Amazon                                                 |
| Chariot coulissant                          | MGN9                                           | 2        | 10 $/unité                                           | Amazon                                                 |
| Engrenage                                   | Module 1, type à moyeu, 16 dents, alésage 6 mm | 1        | 44 $/unité                                           | Amazon                                                 |
| Patin en silicone                           | 30x9x2mm                                       | 1        | 10 $                                                 | Amazon                                                 |
| Vis                                         | Vis KM3*7mm                                    | 80+      |                                                      | Amazon                                                 |
| Vis                                         | Vis KM3*16mm                                   | 8+       |                                                      | Amazon                                                 |
| Vis                                         | KA3*12mm                                       | 48+      |                                                      | Amazon                                                 |
| Vis                                         | Vis HM3-8mm                                    | 60+      |                                                      | Amazon                                                 |
| Vis                                         | Vis HM3-30mm                                   | 16+      |                                                      | Amazon                                                 |
| Vis                                         | Vis de pression HM4-8mm                        | 6+       |                                                      | Amazon                                                 |
| Vis                                         | Vis de pression HM4-16mm                       | 18+      |                                                      | Amazon                                                 |
| Vis                                         | Vis de pression HM4-70mm                       | 4+       |                                                      | Amazon                                                 |
| Vis                                         | Vis HM3-6mm                                    | 8+       |                                                      | Amazon                                                 |
| Vis                                         | Vis HM3-26mm                                   | 6+       |                                                      | Amazon                                                 |
| Câble XT30 2+2                              | Coudé aux deux extrémités, 320 mm              | 1+       | <img src="./Metal_Parts/images/XT30.png" width="80"> | Nécessite une fabrication personnalisée de votre côté. |
| Câble XT30 2+2                              | Coudé aux deux extrémités, 200 mm              | 4+       | <img src="./Metal_Parts/images/XT30.png" width="80"> | Nécessite une fabrication personnalisée de votre côté. |
| Câble XT30 2+2                              | Coudé d’un seul côté, 300 mm                   | 1+       | <img src="./Metal_Parts/images/XT30.png" width="80"> | Nécessite une fabrication personnalisée de votre côté. |
| Câble XT30 2+2                              | Droit aux deux extrémités                      | 1+       |                                                      |                                                        |
| Jeu de tournevis                            | Jeu de clés hexagonales                        | 1        | 16 $                                                 | Amazon                                                 |

### À propos de la fixation

Vous pouvez modifier librement la base à partir des pièces imprimées en 3D que nous fournissons. Vous pouvez également utiliser des serre-joints en G selon l’épaisseur de votre bureau.

| Nom                       | Spécification / modèle    | Quantité | Prix indicatif | Remarques |
| ------------------------- | ------------------------- | -------- | -------------- | --------- |
| Serre-joint de menuiserie | Serre-joint en G 6 pouces | 2        | 20 $/unité     | Amazon    |

### À propos de l’alimentation

Le bras robotique est expédié par défaut sans alimentation. Vous pouvez connecter votre propre batterie ou acheter une alimentation fiable MeanWell 48 V 12,5 A fabriquée à Taïwan. Vous devrez également acheter une prise tripolaire conforme aux normes locales ainsi qu’un faisceau de câbles avec connecteur XT30 femelle.

#### BOM des consommables

| Nom                                                       | Spécification                                                                                                                               | Qté | Prix indicatif | Remarques  |                                           Image                                          |
| :-------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------ | :-: | :------------: | :--------- | :--------------------------------------------------------------------------------------: |
| Alimentation                                              | LRS-600-48（48V12.5A）                                                                                                                        |  1  |      $69.5     | amazon     |                  <img src="./Purchased_Parts/LRS-600-48.png" width="80">                 |
| Cordon d’alimentation                                     | Câble secteur standard US                                                                                                                   |  1  |      $4.49     | amazon     |             <img src="./Purchased_Parts/US Standard AC Cable.png" width="80">            |
| Port de sortie                                            | Connecteur fixe femelle XT60E ; XT60E femelle + cosse, 10 cm, trou de cosse 4 mm                                                            |  1  |      $9.99     | amazon     |      <img src="./Purchased_Parts/XT60E Female to Copper Lug Pigtail.png" width="80">     |
| Câblage secteur                                           | 1,5 mm² ; rouge, bleu, jaune, 1 de chaque. L’utilisateur doit sertir les bornes sur les fils ; les fils présertis ne sont pas inclus. 10 cm |  3  |      $0.99     | aliexpress | <img src="./Purchased_Parts/RV Grounding Wire Coil with Y-Terminal Lugs.png" width="80"> |
| Prise IEC 3-en-1                                          | Type à connexion rapide avec interrupteur rouge, double écrou                                                                               |  1  |      $1.98     | aliexpress |           <img src="./Purchased_Parts/3-in-1 IEC Inlet Socket.png" width="80">           |
| Câble adaptateur XT30 vers XT60                           | XT30U femelle vers XT60 mâle                                                                                                                 |  1  |      $8.99     | amazon     |          <img src="./Purchased_Parts/XT30U_female_to_XT60_male.png" width="80">          |
| Vis cruciforme à tête fraisée en acier inoxydable 304     | M4x6                                                                                                                                        |  10 |      $0.37     | /          |                                             /                                            |
| Vis cruciforme à tête fraisée en acier inoxydable 304     | M3x8                                                                                                                                        |  2  |      $0.36     | /          |                                             /                                            |
| Vis cruciforme à tête cylindrique en acier inoxydable 304 | M3x8                                                                                                                                        |  2  |      $0.32     | /          |                                             /                                            |
| Écrou hexagonal                                           | M3x2.5                                                                                                                                      |  2  |    2.10 CNY    | /          |                                             /                                            |

BOM des pièces imprimées :

| Nom                                                                                           | Image                                                                                 | Quantité | Remarques                                                    |
| --------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | -------- | ------------------------------------------------------------ |
| [Coque avant](./3D_Printed_Parts/RS-power-Top%20Cover.stp)                                    | <img src="./3D_Printed_Parts/images/RS-power-Top Cover.png" width="80">               | 1        | PLA, buse 0,4 mm, hauteur de couche 0,2 mm, remplissage 30 % |
| [Coque arrière](./3D_Printed_Parts/RS-power-Bottom%20Cover.stp)                               | <img src="./3D_Printed_Parts/images/RS-power-Bottom Cover.png" width="80">            | 1        | PLA, buse 0,4 mm, hauteur de couche 0,2 mm, remplissage 30 % |
| [Coque avant — capot coulissant](./3D_Printed_Parts/RS-power-Top%20Cover-Sliding%20Cover.stp) | <img src="./3D_Printed_Parts/images/RS-power-Top Cover-Sliding Cover.png" width="80"> | 1        | PLA, buse 0,4 mm, hauteur de couche 0,2 mm, remplissage 30 % |

#### Assemblage de l’alimentation

* Les étapes d’assemblage de l’alimentation sont divisées en deux parties : coque avant et coque arrière.

##### 1. Assemblage de la coque avant

| Étape | Description                                                                                 | Image                                                                                                                                                                                                                                  | Remarques                                                                                            |
| :---: | ------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------- |
|  1-1  | Préparer les pièces et composants imprimés nécessaires à l’assemblage de la coque avant     | <img src="./Assembly_Steps/powerstep_images/1-1.png" width="80">                                                                                                                                                                       | Vérifier que toutes les pièces sont présentes                                                        |
|  1-2  | Instructions relatives à l’ordre de câblage de chaque composant ; assembler selon cet ordre | <img src="./Assembly_Steps/powerstep_images/1-2(1).png" width="80" style="margin-right:4%;"><img src="./Assembly_Steps/powerstep_images/1-2(2).png" width="80"><br><img src="./Assembly_Steps/powerstep_images/1-2(3).png" width="80"> | Connecter strictement selon l’ordre de câblage                                                       |
|  1-3  | Installer le connecteur XT60                                                                | <img src="./Assembly_Steps/powerstep_images/1-3（1）.png" width="80" style="margin-right:4%;"><img src="./Assembly_Steps/powerstep_images/1-3（2）.png" width="80">                                                                        | Fixer avec des vis cruciformes fraisées M3x8 en acier inoxydable 304 et des écrous hexagonaux M3x2.5 |
|  1-4  | Installer la prise IEC 3-en-1                                                               | <img src="./Assembly_Steps/powerstep_images/1-4（1）.png" width="80" style="margin-right:4%;"><img src="./Assembly_Steps/powerstep_images/1-4（2）.png" width="80">                                                                        | Fixer la prise IEC 3-en-1 avec des vis cruciformes à tête cylindrique M3x8 en acier inoxydable 304   |
|  1-5  | Câblage interne de la coque avant                                                           | <img src="./Assembly_Steps/powerstep_images/1-5（1）.png" width="80"><br><img src="./Assembly_Steps/powerstep_images/1-5（2）.png" width="80">                                                                                             | Vérifier les connexions selon le schéma de câblage                                                   |
|  1-6  | Fixer la coque avant des deux côtés de l’alimentation                                       | <img src="./Assembly_Steps/powerstep_images/1-6（1）.png" width="80" style="margin-right:4%;"><img src="./Assembly_Steps/powerstep_images/1-6（2）.png" width="80">                                                                        | 4 vis cruciformes fraisées M4x6 en acier inoxydable 304                                              |
|  1-7  | Installer le capot coulissant                                                               | <img src="./Assembly_Steps/powerstep_images/1-7（1）.png" width="80" style="margin-right:4%;"><img src="./Assembly_Steps/powerstep_images/1-7(2).png" width="80">                                                                        | Insérer depuis le bas de l’alimentation                                                              |
|  1-8  | Fixer le capot coulissant                                                                   | <img src="./Assembly_Steps/powerstep_images/1-8.png" width="80">                                                                                                                                                                       | 2 vis cruciformes fraisées M4x6 en acier inoxydable 304                                              |

---

##### 2. Assemblage de la coque arrière

| Étape | Description                                                                               | Image                                                                                                                                                           | Remarques                                               |
| :---: | ----------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------- |
|  2-1  | Préparer les pièces et composants imprimés nécessaires à l’assemblage de la coque arrière | <img src="./Assembly_Steps/powerstep_images/2-1.png" width="80">                                                                                                | Vérifier que tous les accessoires sont complets         |
|  2-2  | Assembler la coque arrière avec l’alimentation                                            | <img src="./Assembly_Steps/powerstep_images/2-2.png" width="80">                                                                                                | Aligner la position                                     |
|  2-3  | Fixer la coque arrière des deux côtés de l’alimentation                                   | <img src="./Assembly_Steps/powerstep_images/2-3(1).png" width="80" style="margin-right:4%;"><img src="./Assembly_Steps/powerstep_images/2-3(2).png" width="80"> | 4 vis cruciformes fraisées M4x6 en acier inoxydable 304 |

---

##### 3. Finalisation

| Étape | Description                          | Image                                                          | Remarques                                     |
| :---: | ------------------------------------ | -------------------------------------------------------------- | --------------------------------------------- |
|   1   | Assemblage de l’alimentation terminé | <img src="./Assembly_Steps/powerstep_images/3.png" width="80"> | Vérifier que toutes les vis sont bien serrées |
