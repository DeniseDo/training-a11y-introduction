# Mesurer et évaluer

<!-- .slide: class="page-title" -->



## Sommaire

<!-- .slide: id="master-toc" class="toc" -->

- [Agenda](#/0)
- [Accessibilité &amp; Handicap](#/1)
- [Standards &amp; Réglementations](#/2)
- [Web Content Accessibility Guidelines (WCAG)](#/3)
- **[Mesurer &amp; Évaluer l'Accessibilité Web](#/4)**
- [Mise en œuvre de l'Accessibilité Web](#/5)
- [Ce qu'il faut retenir](#/6)



## L'audit d'accessibilité

[Un audit d'accessibilité](https://www.w3.org/TR/WCAG-EM) est une démarche formel visant à mesurer le niveau de conformité d'un site ou une application web avec la norme WCAG.

Un audit peux conduire à :
- Un plan de correction de l'accessibilité
- Une déclaration de conformité

Un audit se déroule en 4 étapes:
1. Identifier le périmètre d'application
2. Sélectionner un échantillon représentatif des pages/vues à tester.
3. Evaluer la conformité de chaque page de l'échantillons
4. Formaliser un rapport d'audit

https://www.w3.org/WAI/eval/report-tool/



## Audit (1): Périmètre d'application

Avant de commencer un audit d'accessibilité il est primordial de bien [le périmètre d'application de l'audit](https://www.w3.org/TR/WCAG-EM/#step1) :

- Sur quel périmètre de votre site ou application web porte votre audit (domaines, langues, fonctionnalité…).
- Quel niveau de conformité est visé (A, AA, AAA)
- Quels sont les navigateurs et autres assistances techniques de référence (JAWS, NVDA, VoiceOver…)
- Définissez tous les cas particuliers qui s'appliquent.

Au delà de vous aider à définir quels critères de succès WCAG vont s'appliquer, cela va aussi vous aider à déterminer ce dont vous aurez besoin pour effectuer vos tests.



## Audit (2): Échantillons représentatif

[Commencez par identifier les éléments clés de votre site web](https://www.w3.org/TR/WCAG-EM/#step2) :

- Identifiez les pages les plus communément utilisé
- Identifiez les fonctionnalités essentielles de votre site web
- Identifiez les différents types de pages existant
- Identifiez les différentes technologies web utilisées
- Identifiez les pages dédiées à des problématiques d'accessibilités

Sur cette base, [sélectionnez un échantillons représentatif](https://www.w3.org/TR/WCAG-EM/#step3) comportant deux types de pages :

- [Les pages correspondant aux processus clés](https://www.w3.org/TR/WCAG-EM/#step3a) de votre sites/applications.
- [Un échantillons de pages prises au hasard](https://www.w3.org/TR/WCAG-EM/#step3b) (idéalement un nombres équivalent à 10% des pages de processus).



## Audit (3): Évaluer la conformité

Il s'agit ici de prendre la liste de toutes les critère d'acceptance WCAG et des les confronter de manière systématiques à l'échantillons de pages sélectionner.

[Cette évaluation ce fait pour chaque page](https://www.w3.org/TR/WCAG-EM/#step4) en suivant les pré-requis de conformité WCAG 2.1:

1. [La page remplis tous les critères de succès WCAG applicables](https://www.w3.org/TR/WCAG21/#cc1)
2. [Toute la page est conforme](http://www.w3.org/TR/WCAG21/#cc2)
3. [Si la page fait partie d'un processus, toutes les pages du processus sont conformes](http://www.w3.org/TR/WCAG21/#cc3)
4. [Toutes critères sont satisfait via des technologies accessibles](https://www.w3.org/TR/WCAG21/#cc4)
5. [La présence de technologie non-accessible n'entrave pas l'utilisation de la page](http://www.w3.org/TR/WCAG21/#cc5)

Notes :
Les critère 4 et 5 sont là pour s'assurer qu'on utilise pas des technologies pas encore supportés (un attribut aria par reconnus par exemple) ou plus supporté (Flash) pour l'accessibilité. En gros l'accessibilité ne doit pas être théorique mais bien réel.

La présence d'erreurs d'accessibilité n'est pas un signe de non-conformité. La conformité WCAG n'est pas binaire.

Ce n'est pas parce qu'il n'y a aucune erreur qu'un contenu est accessible
Ce n'est pas parce qu'il y a des erreur qu'un contenu n'est pas accessible



## Audit (4): Rapport d'audit

[Un rapport d'audit va documenter toutes les informations](https://www.w3.org/TR/WCAG-EM/#step5) formalisées ou découvertes lors des phases précédentes. L'objectif et de centraliser toutes les informations nécessaire pour envisager une déclaration de conformité ou pour mettre un place un plan d'action correctif si nécessaire (les deux ne s'excluant pas). En particulier, on attend d'un rapport d'audit d'accessibilité de fournir :

- Un états détaillé de l'évaluation de chaque page (Capture d'écran, instructions pour reproduire les conditions d'audit, les outils utilisés, les méthodes utilisé, les recommendations de correction et autres remarques associées).
- Les informations nécessaire pour réaliser une déclaration de conformité



## La déclaration de conformité

Une déclaration de conformité est une démarche visant à annoncer publiquement le niveau de conformité d'un site, d'une application ou d'une page web donnée à une date donnée. La déclaration de conformité sera généralement publié sur le site testé (des réglementations locales peuvent s'appliquer en ce qui concerne le lieu et la forme de la publication si on veux lui donner une valeur légale).

En général, une déclaration de conformité doit à minima comprendre les informations suivantes :

- La date de déclaration de conformité
- La dénomination exact de la spécification correspondante
- Le niveau de conformité atteint
- Une liste des pages concernées par la déclaration
- Une liste des technologies web concernés

https://www.w3.org/TR/WCAG21/#conformance-claims



## Outillage de mesure

**Aucun outils n'est en mesure de dire si un site est conforme WCAG !**

Tous les outils d'accessibilité sont des aides pour tester vos contenus ou pour limiter les risques d'erreurs techniques.

Les outils d'analyse automatique (linter) :
- [Axe](https://www.deque.com/axe/) qui est utilisé par beaucoup d'autre outils: [Accessibility Insights](https://accessibilityinsights.io), [AccessLint](https://accesslint.com), [Storybook A11Y](https://github.com/storybookjs/storybook/tree/next/addons/a11y), plein de [modules NPM](https://www.npmjs.com/search?q=keywords%3Aa11y), etc.

Les outils d'aide pour l'analyse manuel :
- [Google Lighthouse](https://developers.google.com/web/tools/lighthouse)
- [WebAIM WAVE](https://wave.webaim.org/)
- Des extensions pour [Chrome](https://chrome.google.com/webstore/search/accessibility?_category=extensions) et [Firefox](https://addons.mozilla.org/fr/firefox/search/?q=accessibility)

Et bien d'autre :
- https://www.w3.org/WAI/ER/tools/

Notes :
https://github.com/dequelabs/axe-core



<!-- .slide: class="page-questions" -->



<!-- .slide: class="page-tp1" -->
