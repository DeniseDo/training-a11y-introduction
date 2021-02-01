## TP1 — Audit d'accessibilité

### Objectif

L'objectif de ce TP est de vous faire réaliser votre premier audit d'accessibilité afin de vous familiariser avec la démarche.


### Pré-requis

Pour pouvoir réaliser ce TP vous devez vous assurez d'avoir accès à un navigateur web (Firefox, Safari, Chrome, etc.) connecté à Internet.

Pour enregistrer les résultats de votre audit nous allons utiliser [l'outil d'aide au reporting du W3C](https://www.w3.org/WAI/eval/report-tool) (en anglais). Cependant, vous pouvez également réaliser cette audit en utilisant d'autre support de reporting comme par exemple [le kit RGAA 4.0](https://www.numerique.gouv.fr/publications/rgaa-accessibilite/kit/#contenu) ou votre propre checklist que vous aurez créée avec la suite bureautique de votre choix (Office, OpenOffice, Google Apps, etc.).

Vous devez ensuite décider du site web que vous allez auditer. Cela peut être le site de votre entreprise ou un site que vous utilisez régulièrement. Comme il s'agit de votre premier audit, nous vous conseillons de sélectionner un site plutôt orienté contenus (un site de e-commerce ou un journal en ligne par exemple) plutôt qu'une application très interactive (comme un réseau social ou un moteur de recherche par exemple)

Enfin, sélectionnez 3 ou 4 pages différentes sur le site qui vous servirons d'échantillons de test. Par exemple, si vous choisissez un site de presse, vous pouvez sélectionner :

- La page d'accueil
- Un listing d'articles
- Une page d'article
- La page du formulaire d'abonnement


---

### Exercice 1

Ce premier exercice à pour vocation à préparer l'audit.

Dans un onglet de votre navigateur, ouvrez la page: https://www.w3.org/WAI/eval/report-tool et sélectionner directement l'étape 3 « <i lang="en">Select Sample</i> ».

Remplissez le formulaire avec les pages du site que vous avez prévus d'examiner dans la sous-partie « <i lang="en">Structured Sample Web Pages</i> ».

Pour chacune des pages que vous avez sélectionné et que vous avez ajouté au formulaire d'audit, ouvrez là dans un nouvel onglet de votre navigateur.

Notez que l'outil d'aide au reporting du W3C n'est pas un outils linéaire, vous pouvez passer d'une étape à l'autre sans contrainte. L'objectif est de remplir les champs de cet outils le plus complètement possible pour obtenir le rapport le plus utile possible, pas de vous forcer à suivre une procédure d'audit particulière.

_Dans le cadre de cet exercice, il n'est pas nécessaire de passer beaucoup de temps à sélectionner votre échantillon de pages à tester mais n'oubliez pas que dans le cadre d'un audit complet, cette phase est critique pour être sur qu'on a une bonne représentativité des capacités et contenus du site examiné._

> Si vous ne souhaitez pas utiliser l'outil d'aide au reporting du W3C, vous
> pouvez créer votre propre document d'audit. Une pratique commune consiste à
> utiliser un outils de feuille de calcul comme Microsoft Excel pour créer une
> matrice d'audit qui permettra de recueillir toutes les données d'audit pour
> chacune des pages que l'on inspectera. Typiquement, la première colonne
> contiendra tous les critères de succès WCAG et chacune des colones
> subséquente contiendra les résultats d'audit pour chacune des pages de notre
> échantillon.


---

### Exercice 2

Ce second exercice à pour vocation de collecter les informations d'audit.

A présent rendez-vous à [l'étape 4 de l'outil d'aide au reporting du W3C](https://www.w3.org/WAI/eval/report-tool/#!/evaluation/audit). C'est ici que l'on va rassembler les informations d'audit. Avant de commencer nous allons définir les critères de succès qui vont s'appliquer. Dans le cadre de cet exercice, sélectionnez uniquement la **spécification WCAG 2.0** et le **niveau A**. (Dans le cadre d'un audit de conformité réglementaire il sera plus souvent demandé de se conformer à WCAG 2.1 en niveau AA).

A présent, pour chacune des pages, vous allez devoir vérifier la conformité de chaque critère de succès et reporter le résultat dans l'outil d'aide au reporting du W3C.

Cette vérification de conformité se déroule en plusieurs étapes :

1. Vérifier que le critère est applicable à la page que vous examinez
2. Vérifier qu'aucunes des conditions d'échec du critère n'est remplis
3. Vérifier qu'au moins une des conditions suffisantes du critère est remplis

Pendant votre audit, nous vous conseillons de garder un onglet ouvert avec [la référence rapide de WCAG 2.1](https://www.w3.org/WAI/WCAG21/quickref/), ce qui vous permettra d'accéder rapidement aux conditions suffisantes de succès (<i lang="en">Sufficient Techniques</i>) et d'échecs (<i lang="en">Failures </i>).

> Si vous le souhaitez, vous pouvez vous faire aider dans votre audit par des
> outils comme [l'outil WAVE de WebAIM](https://wave.webaim.org/). Quelque soit
> l'outil que vous utilisez, pensez à le mentionner dans votre rapport
> d'audit.

_L'objectif ici n'est pas la quantité mais la qualité. Il vaut mieux passer tout le temps de l'exercice à valider correctement un seul critère de succès sur une seul page en comprenant exactement ce que vous faites plutôt que d'essayer de valider à tout prix tous les critères de succès sur toute les pages sans les comprendre._

> Si vous ne souhaitez pas utiliser l'outil d'aide au reporting du W3C, c'est
> le moment de remplir la matrice que vous avez créer à l'exercice 1. Pour
> chaque page et pour chaque critère de succès il vous faudra déterminé si le
> critère est conforme, non-conforme ou inapplicable. Dans le cas ou le critère
> serais non-conforme n'oubliez pas de préciser la raison pour laquelle il
> ne l'est pas.


---

### Exercice 3

Ce dernier exercice à pour objet de formaliser les résultats de votre audit et proposant un plan de mise en conformité.

Une fois que vous avez terminer votre évaluation, il ne vous reste plus qu'à mettre la dernière touche à votre audit.

En vous rendant à [l'étape 5 de l'outil d'aide au reporting du W3C](https://www.w3.org/WAI/eval/report-tool/#!/evaluation/report), vous verrez un résumé des résultats de votre évaluation. Ici vous devez vérifier deux choses :

1. Pour chacun des critères qui sont en échec, vous devez avoir un commentaire <i lang="en">Findings</i> expliquant la cause de l'échec.
2. Remplissez le champ <i lang="en">Executive summary</i>. Ce champs doit contenir un résumé des principaux problèmes rencontrés et une liste d'actions correctives.

Une fois tous les champs remplis, vous pouvez passer à [l'étape final qui va vous afficher votre rapport d'audit](https://www.w3.org/WAI/eval/report-tool/#!/view_report).

Si vous avez fait cet exercice à plusieurs, c'est le moment d'échanger vos trouvailles afin d'estimer le degrés de conformité de du site examiné.

> Si vous ne souhaitez pas utiliser l'outil d'aide au reporting du W3C, vous
> allez devoir formaliser votre rapport d'audit vous même. N'importe quelle
> suite bureautique fera l'affaire. Un rapport d'audit doit contenir à minima,
>  * le nom de la personne ayant réaliser l'audit,
>  * la date de l'audit
>  * la liste des outils utilisés
>  * une description de la méthode d'audit
>  * la liste des pages examinées
>  * la liste de tous les critères de succès et l'état de leur conformité (tous
>    ceux qui ne sont pas conforme doivent êtres accompagnés d'un explication
>    des raisons de l'échec)
>  * Un résumé de l'état de la conformité est une liste des actions correctives
>    à mener.
