cat > README.md << EOF
# Contrôle de vitesse d’un moteur DC 12V via NE555 (PWM)

Projet de commande de vitesse d’un moteur DC 12V à l’aide d’un potentiomètre, en générant un signal PWM avec un NE555 en mode astable.

## Objectif

Réguler la vitesse d’un moteur DC 12V en faisant varier le rapport cyclique d’un signal PWM.

## Principe

- NE555 en mode astable génère un PWM.
- Un potentiomètre ajuste le rapport cyclique.
- Un MOSFET IRFZ44N commute le moteur en fonction du PWM.
- Une diode de roue libre protège le circuit.

## Structure du repo

- \`docs/\` : notes, schémas exportés, simulations.
- \`hardware/\` : schémas et PCB.
- \`assets/\` : photos, captures, vidéos.

## À venir

- Schéma électrique complet.
- PCB.
- Photos du montage.
- Vidéo de démo.
EOF
