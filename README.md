# Git et Github - Évaluation

Module : Git et Github

Promotion : 2è année

Version : 1

Durée : 1h

Date : 24/10/24

- [Git et Github - Évaluation](#git-et-github---évaluation)
  - [Comment rendre votre travail](#comment-rendre-votre-travail)
  - [Notation](#notation)
  - [Énoncé](#énoncé)
    - [QCM](#qcm)


## Comment rendre votre travail

> Merci de **lire attentivement** les consignes !

Envoyer votre travail par **un e-mail** à l’adresse suivante :  

<a href="mailto:pschuhmacher@myges.fr?subject=git-github-evaluation x_abc">pschuhmacher@myges.fr</a>, **ayant le sujet suivant** : 

`git-github-evaluation x_abc` 

où **`x`** est la première lettre de votre nom et **`abc`** votre prénom. Ainsi, j'enverrai un e-mail avec le sujet `git-github-evaluation s_paul`

Dans l'e-mail :

- **Placer l'URL de votre dépôt Git**.


## Notation

L'évaluation est notée sur 20, **coefficient 1**. Sauf mention contraire, chaque question est notée sur 1 point.

La qualité du document (hiérarchie du contenu, lisibilité) et **le respect des consignes sera pris en compte dans la note** (**3pt**). 

**Merci de penser au correcteur**.

<!-- ## Consignes

- Étant donné le caractère fondamental des notions vues dans ce module, **l'usage d'IA générative, comme chatGPT ou CoPilot, est interdite** ! **Toute dérogation à cette règle entraînera une note de 0**;
- Vous pouvez consulter vos notes de cours. -->

## Énoncé

1. Depuis votre compte Github, **forker** [ce dépôt](https://github.com/paul-schuhm/git-github-exam) et **cloner** le sur votre machine.
2. Sur le dépôt, **créer** une branche `answers` et placez-vous y.
3. **Répondez** [aux questions suivantes](#qcm). Pour cela, **modifier** le fichier `README.md` de sorte à ne **conserver que la ou les bonnes réponses sous la question**. Chaque réponse à une question est une modification du fichier et **doit être publiée sous forme de commit**. Il doit y avoir (au moins) **autant de commits dans votre branche que de questions**. (4pts)

Exemple de modification :
~~~bash
1. De quel couleur était le cheval blanc d'Henry IV ?
- Blanc
- Bleu
- Noir
- Vert
~~~

Réponse :
~~~bash
1. De quel couleur était le cheval blanc d'Henry IV ?
- Blanc
~~~

5. Lorsque vous avez terminé, nettoyer vos commits au besoin (squash, commentaires, etc.), **fusionner** votre branche `answers` dans votre branche principale **en créant un merge commit**. Ce commit doit apparaître dans votre historique de commits.
6. **Ajouter un tag** sur ce commit ayant pour label votre nom et prénom;
7. **Publier** vos changements sur Github sur la branche `main`.
8. **Publier également votre branche** `answers` sur Github.
9.  **Ouvrir** une **Pull Request** sur ce dépôt. Dans la *code review* ouverte avec la PR, **ajouter le commentaire** suivant: *"Voici ma contribution, (nom et prénom)"*. (2pt)

### QCM

1. Qui a inventé le logiciel git ?
- Linus Torvalds

2. Pour créer un dépôt localement à partir d'un répertoire vide, quelle est la commande git à utiliser ?
 - init

3. Parmi les protocoles suivants, quels sont les protocoles qui sont utilisables pour communiquer avec la plateforme GitHub ?
 - SSH
 - HTTP
 - HTTPS

4. À quoi sert la commande `git remote -vv` ?
 - lister les alias des dépôts distants configurés sur le dépôt local

5. Quels sont les 2 types de branches qui existent dans un dépôt git *sur* l'ordinateur d'un·e développeur·se ?
 - les références locales de branches distantes

6. À quoi sert la commande `git fetch -p` ? Utiliser la documentation `man git fetch`.
 - mettre à jour les références locales de branches distantes et supprimer celles qui n'existent plus sur le dépôt distant

7. Quelle est la commande git qui permet d'ajouter un nouveau fichier dans un futur commit ?
 - add

8. Est-il possible d'ajouter un répertoire vide dans un dépôt git ?
 - Non

9. Quel est le chemin du fichier de configuration locale d'un dépôt git ?
 - .git/config

10. À la première utilisation, quelles sont les informations nécessaires pour créer un commit ?
 - l'adresse mail de l'utilisateur git
  
11. Quelle est la commande qui permet de mettre à jour la branche sur laquelle on se trouve par rapport à un dépôt distant ? 
 - pull

12. Quelle est la commande qui permet de se mettre sur n'importe quel commit d'un historique git ? 
 - checkout

13. Dans quelles conditions est-ce qu'un conflit apparaît avec git ? 
- Lorsqu'il y a un merge entre deux branches qui modifient la même partie d'un fichier

14. Lorsqu'il y a un conflit, qu'indique la commande `git status` sur les fichiers qui demandent une résolution ? 
 - both modified
  
15. Dans quelle zone du dépôt est-ce que les modifications sont regroupées *avant* de créer un commit ? 
 - le stage

16. Lorsque vous résolvez un conflit, quelle est la dernière commande git que vous tapez ? 
 - commit

17. Quelle est la commande git qui permet de propager ses modifications sur un dépôt distant ? 
- push

18. Comment s'appelle le mécanisme qui permet d'accepter ou de refuser une contribution sur un dépôt GitHub ? 
 - Pull Request

19. Après avoir accepté une contribution sur la branche principale sur Github, que devez vous faire pour mettre à jour votre branche principale localement ? 
 - se mettre sur la branche principale et faire un git pull

20. Qu'est-ce que fait la commande `git merge` ?
 -  fusionne l'historique d'une branche avec une autre en créant un nouveau commit de fusion

21. Quelle est une conséquence potentielle de l'utilisation de `git rebase` sur une branche publique ?
 - Les autres collaborateurs ayant déjà récupéré la branche peuvent rencontrer des problèmes de synchronisation avec l'historique modifié.

22. Les branches de suivi (*tracking branch*) sont:
 - Des branches locales configurées pour suivre les modifications d'une branche distante. 

23. Pour mettre à jour (dans le même état) les branches de suivi (*tracking branch*) avec les branches distantes, il faut:
  - Utiliser `git fetch`.

24. `git pull` fait automatiquement un rapatriement de commits d'une branche à l'autre via une stratégie de *merge*: 
 - Vrai.


25. Le nom `origin` donné à un dépôt distant est:
 - Une convention.