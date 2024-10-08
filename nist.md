# NIST OT/ICS

[NIST.SP.800-82r3](NIST.SP.800-82r3.pdf)

## Résumé des recommandations OT (page 59)

Une centrale électrique est dotée d'un système **SCADA** qui gère la distribution de l'énergie pour une grande installation militaire. Ce système SCADA contient deux types d'informations : des **données des capteurs en temps réel** et des **informations administratives**. La direction a évalué les impacts potentiels en cas de perte de **confidentialité**, **intégrité** et **disponibilité** de ces informations.

### Catégories de sécurité des types d'informations

| Type d'information          | Confidentialité | Intégrité | Disponibilité |
|-----------------------------|-------------------|--------------|----------------|
| Données des capteurs       | N/A               | ÉLEVÉ       | ÉLEVÉ         |
| Informations administratives | FAIBLE            | FAIBLE       | FAIBLE         |

La catégorie de sécurité initiale du système SCADA est donc la suivante, selon la règle du **maximum potentiel d'impact** pour chaque objectif de sécurité :

**SC SCADA système** : {(confidentialité, FAIBLE), (intégrité, ÉLEVÉ), (disponibilité, ÉLEVÉ)}

### Ajustement de la catégorie de confidentialité

La direction de la centrale a choisi d'élever l'impact potentiel de la perte de **confidentialité** de faible à **modéré**. Cette modification reflète une vision plus réaliste des conséquences potentielles d'une divulgation non autorisée d'informations ou de fonctions critiques du système SCADA.

La catégorie de sécurité finale du système SCADA est :

**SC SCADA système** : {(confidentialité, MODÉRÉ), (intégrité, ÉLEVÉ), (disponibilité, ÉLEVÉ)}
