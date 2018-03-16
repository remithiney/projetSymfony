# projetSymfony
le projet symfony pour le groupe stage M1 upjv

EN LOCAL TRAVAILLER DANS C:\wamp64\www\projetSymfony

# Nomage
Système de nomage

# Assemblage
Comment on assemble

# Fusion
Comment on fusionne

#SUJET 
il est également disponible dans le git.

Architecture web des SI Projet 1 - année 2018
Gestion d'un site d'évaluation des connaissances
Le site web d'évaluation des connaissances propose des questionnaires à des apprenants qui leur
permet d'évaluer leur niveau de connaissance sur les thèmes qui les intéressent.
Les apprenants souhaitent évaluer leurs connaissances :
• un apprenant est un utilisateur authentifié
• chaque apprenant a une liste de thématiques qui l’intéressent
• l'apprenant se voit proposer des questionnaires dans ses thématiques
• il peut répondre à un questionnaire :
◦ quand il considère qu'il a fini de répondre, il clôt le questionnaire : il ne pourra plus
changer ses réponses, le questionnaire est "rempli"
• il peut consulter la liste des questionnaires qu'il a passé/rempli et voir la correction si elle a
été effectuée.
◦ un questionnaire rempli et corrigé précise le pourcentage de réponses correctes, ainsi
qu'un commentaire pour chaque réponse incorrecte
◦ il dispose d'une moyenne générale des pourcentage de réussite
Les entraîneurs rédigent des questionnaires:
• un entraîneur est un utilisateur authentifié
• un entraîneur rédige des questionnaires, les modifie et les supprime
• chaque questionnaire comporte plusieurs questions, est daté et figure dans une thématique
• quand l'entraîneur considère que la rédaction d'un questionnaire est finie, il peut le publier
• tant que le questionnaire n'est pas publié, il peut ajouter, modifier et supprimer des
questions.
• il voit la liste de ses questionnaires publiés ou non
• il ne peut supprimer un questionnaire que non publié.
Les correcteurs corrigent les réponses à un questionnaire :
• un correcteur est un utilisateur authentifié : il peut être aussi un entraîneur
• chaque correcteur a une liste de thèmes pour lesquels il est susceptible d'être correcteur
• il voit les questionnaires passés/remplis, correspondant à ses thèmes, non corrigés ou qu'il
est en train de corriger
• la correction d'un questionnaire rempli consiste à corriger chacune des réponses :
◦ indiquer si chaque réponse est correcte ou non
◦ et, si la réponse n'est pas correcte, rédiger un commentaire
◦ il ne voit pas le nom de l'apprenant qui l'a rempli
◦ le questionnaire est corrigé quand toutes les réponses sont corrigées
• un questionnaire rempli par un apprenant n'est corrigé que par un seul et même correcteur
Le secrétaire gère les utilisateurs :
• c'est un utilisateur authentifié
• Il ajoute, supprime les utilisateurs et gère leur(s) rôle(s) :
◦ il peut changer leur mot de passe et leurs thématiques
• il peut retrouver un utilisateur par son nom ou une partie de son nom
• il ajoute des thèmes et en supprime s'ils sont inutilisés
• pour chaque apprenant, il dispose d'un état récapitulatif des questionnaires remplis avec leur
pourcentage de réussite ainsi qu'une moyenne générale.
• il peut supprimer un apprenant, et cela supprime ses copies
Réalisation
Le projet est à réaliser en Symfony 3.3.9 avec Doctrine.
Il comporte les 4 modules décrits plus haut et est à réaliser en groupe de 4 apprenants : chacun
ayant un module.
L'analyse (très légère) donnée ci-avant est faite pour vous aider mais est insuffisante. Exemple :
attention aux suppressions ! Ne cherchez pas, non plus, à trop perfectionner le cahier des charges !
Vous pouvez poser demander des précisions par mail : didier.ferment@u-picardie.fr.
Le développement se déroulera principalement pendant les séances restantes du module : chacun
des développeur sera présent. Les membres du projet doivent se mettre d'accord sur leur modèle de
données, les parties communes de développement, la gestion de la sécurité s'il y a.
Il est inutile de réaliser un bel affichage avec du CSS.
Vous pouvez vous aider avec la génération du Crud mais il doit être amélioré : entre-autre, pas d’id
d’entité qui traîne!
Pour tester, mais aussi pour soutenir, pensez à préparer des jeux de tests de données (comme mes
fonctions testActions) , voire utiliser les fixtures Doctrine.
Vous rendrez un rapport très simple (papier) :
- 1 page pour le modèle (en entités et associations avec cascade et « coté owner »)
- 1 page pour chacune des 4 parties précisant les contrôleurs et actions
Vous copierez votre projet zippé sur ma clef USB ; la racine est le répertoire du projet symfony et
le contenu de var/cache est supprimé.
La soutenance aura lieu lors de la dernière séance : elle est collective et individuelle.
Lors de la soutenance, chaque développeur sera responsable de sa partie et devra la soutenir : vous
exécuterez le projet et aurez à répondre sur les lignes de votre code.


