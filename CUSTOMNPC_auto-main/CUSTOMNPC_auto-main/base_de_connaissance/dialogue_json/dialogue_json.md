dialogs:

7.json
"je viens blablabla"
    disponibilité: apres quête
    type: déchange une quete 
    déclenche:
      - quête: non
      - commande: oui
      - mail: non
      - son: non

1.json:
"Bob"
    disponibilité: avant quête
    type: à choix
    options:
      - 4 choix: mènent vers 4 dialogues 
    déclenche:
      - quête: non
      - commande: non
      - mail: non
      - son: oui

3.json
"que doij fair mainteant
    type: choix_retour
    disponibilité: sans_restriction  # accessible uniquement via un autre dialogue
    option: retour vers 1_bob_intro.json
    déclenche:
      - quête: non
      - commande: non
      - mail: oui, le mail contient un item du texte pas de quete.
      - son: non

4.json
 "bonjour aventurier"
    type: choix_retour
    disponibilité: sans_restriction  # accessible uniquement via un autre dialogue
    option: revoie a un dialogue
    déclenche:
      - quête: non
      - commande: oui
      - mail: non
      - son: non

2.json:
  "ou suis je exactement.json"
    type: choix_retour
    disponibilité: sans_restriction  # accessible uniquement via un autre dialogue
    option: revoie a un dialogue
    déclenche:
      - quête: non
      - commande: non
      - mail: non
      - son: non

  2_bob_retour.json:
    type: choix_retour
    disponibilité: sans_restriction  # accessible uniquement via un autre dialogue
    option: revoie a un dialogue
    déclenche:
      - quête: non
      - commande: non
      - mail: non
      - son: non

  je suis prets.json:
    disponibilité: avant quête
    type: déclencheur
    action: démarre la quête "parle_au_forgeron"
    déclenche:
      - quête: oui
      - commande: non
      - mail: non
      - son: non
