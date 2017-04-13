# mastodon-faq-fr

La FAQ n'est pour le moment pas organisée, je jette ici les questions que l'on me pose fréquemment.

___
# Mastodon lui même
## Qui a créé Mastodon ?

Eugen, [@Gargron@mastodon.social](https://mastodon.social/@Gargron)

## Le code source

Celui-ci est disponible à l'adresse [https://github.com/tootsuite/mastodon](https://github.com/tootsuite/mastodon) et sous licence [AGPLv3.0](https://www.gnu.org/licenses/agpl-3.0.fr.html)

## Je ne comprends rien, il y a une introduction ?

Il existe des documents créés par des utilisateurs comme : 
* [Welcome to Mastodon par Aldarone](https://aldarone.fr/welcome-to-mastodon/)
* [Mastodon qu'est-ce que c'est par @numendil@mastodon.xyz](http://pixellibre.net/2017/04/mastodon-quest-cest/)

Ou des articles dans la presse :
* [Débuter sur Mastodon : 9 questions pour tout comprendre au réseau social décentralisé (Numerama)](http://www.numerama.com/tech/246684-debuter-sur-mastodon-9-questions-pour-tout-comprendre-au-reseau-social-decentralise.html)
* [Mastodon mais en fait comment ça marche ? (NextInpact)](https://www.nextinpact.com/news/103953-mastodon-mais-en-fait-comment-ca-marche.htm)
* [Mastodon, le réseau social libre et décentralisé prêt à voler dans les plumes de Twitter (NextInpact)](https://www.nextinpact.com/news/103937-mastodon-reseau-social-libre-et-decentralise-pret-a-voler-dans-plumes-twitter.htm)

___
# Fonctionnement des instances

## Comment choisir son instance ?

La liste des instances est disponible sur (https://instances.mastodon.xyz) la version JSON existe aussi (https://instances.mastodon.xyz/instances.json)

Des statistiques sont disponibles sur (http://sp3r4z.fr/mastodon/)

Il est important de se renseigner sur plusieurs points avant de choisir celle sur laquelle créer son compte :
1. **Le règlement**. Chaque instance à ses propres règles concernant les contenus autorisés et interdits, les consignes et comportement à adopter. Chaque instance devrait indiquer ces information dans une page prévue à cet effet, /about/more pour les instances mastodon.xyz, mastodon.social et mamot.fr par exemple ce sont respectivement (https://mastodon.xyz/about/more) (https://mastodon.social/about/more) (https://mamot.fr/about/more)

2. **Les aspects techniques**. Sur la page des instances vous pouvez remarquer un taux d'uptime (la disponibilité), une note pour HTTPS (le chiffrement de la connexion), support d'IPv6 ou pas.

3. **Les administrateurs**. Vous devez prendre conscience qu'un administrateur sur une instance **PEUT** faire tout ce qu'il souhaite. Il ne le fera peut être pas mais il **PEUT** lire tous vos messages, même privés, obtenir votre adresse email... En créant un compte sur une instance vous devez faire confiance à son/ses administrateur(s)

Je conseille de se connecter à une instance dont vous connaissez les admins et si vous avez une confiance aveugle en eux.
Si vous ne connaissez pas d'admin vous pouvez aller chez (https://mamot.fr) l'instance de [La Quadrature du Net](https://laquadrature.net) une association de défense des droits et libertés des citoyens sur Internet, pour qui la vie privée est importante.


## Si je suis sur une instance, puis-je discuter avec des personnes sur une autre instance ?

Oui. Les instances discutent entre elles pour que les utilisateurs de chaque instance puissent communiquer.

L'ensemble de ces instances se nomme le Fediverse (Contraction de Federation / Universe).

## Peut-on migrer son compte d'une instance à une autre ?
Réponse courte : NON

Réponse longue, la bonne pratique est de suivre ces étapes :
1. Créer un compte sur la nouvelle instance
2. Renommer son ancien compte pour y inclure le préfixe [MIGRE]
3. Écrire un dernier toot sur l'ancien compte en indiquant la migration et en spécifiant le nouveau compte.

Il est possible d'exporter puis d'importer la liste de ses abonnements, pas les abonnés, ainsi que la liste des personnes bloquées.

## Pourquoi ne puis-je pas m'inscrire sur certaines instances ?
L'administrateur de ces instances n'a pas ouvert les inscriptions, ce sont des instances privées ou publiques devenues fermées pour préserver les ressources sur l'instance.

## Installer sa propre instance de Mastodon

Si vous le désirez il est possible d'installer votre propre instance Mastodon sur votre serveur. Nous attirons votre attention sur plusieurs points avant de procéder à l'installation de celle-ci :

* avoir suffisament de ressources CPU / RAM
* un serveur stable
* une adresse IP fixe

En installant votre instance Mastodon prenez bien soin à la maintenir pour vous utilisateurs ainsi que pour vous-même. Nous regroupons ici diverses documentations :

* [Un rôle ansible pour Mastodon](https://git.legeox.net/mastodon/ansible-role)
* [Installer une instance Mastodon sous Debian 8](https://angristan.fr/installer-instance-mastodon-debian-8)
* [Running a Mastodon instance on Ubuntu 16.04 with Docker & nginx](https://github.com/ummjackson/mastodon-guide/blob/master/up-and-running.md)

## Un article sur l'infrastructure de mastodon.social par [@Gargron le créateur de Mastodon](https://github.com/Sniperovitch/mastodon-faq-fr/blob/master/README.md#qui-a-créé-mastodon-).
[Scaling Mastodon](https://medium.com/@Gargron/scaling-mastodon-1becde463090)

___
# Son compte 

## Peut-on certifier son compte ?

Non, ce principe n'existe pas contrairement à Twitter.

Néanmoins, certaines instances proposent ça en validant des comptes et en listant les noms dans la page /about/more

## Comment exporter mes données ?

Dans *Préférences > Data export* ou directement sur la page /settings/export de votre instance, par exemple pour mastodon.xyz c'est (https://mastodon.xyz/settings/export)

# Se connecter à Mastodon

## Utilisation de l'interface web Mastodon

Une fois que vous avez créé un compte sur Mastodon vous avez alors la possibilité d'utiliser l'interface web de votre instance. L'interface web est assez ressemblante à **tweetdeck**. L'interface web est par défaut découpée en quatre colonnes :

* écrire / répondre à un pouet
* consulter votre timeline
* consulter vos notifications
* consulter les pouets de votre instance, des autres instances, vos préférences, vos favoris, les utilisateurs bloqués, de la documentation, vous déconnectez

Pour écrire un pouet vous disposez ainsi de la première colonne de l'interface. Cela vous permet :

* d'écrire un pouet contenant jusqu'à 500 caractères
* d'y insérer des photos
* de positionner la visibilité de votre message (public, non listé, privé, direct)
* masquer le texte derrière un avertissement

Une fois votre message prêt il suffit de cliquer sur le bouton **POUET!** et celui-ci sera transmis.

Pour consulter les interactions de vos abonnements vous regarderez la colonne intitulée **Accueil**.

Lorsque vous recevez une interaction dans la colonne **Notifications** cela concerne : pour un nouvel abonné, un pouet favorisé, une mention ou bien un partage.
Pour répondre à un pouet il suffit de cliquer sur la flèche répondre et de compléter votre message dans la nouvelle fenêtre apparue.


## Est-ce qu'il existe un client Mastodon sur smartphone ?
Oui.
Sur iOS, pour iPhone / iPad il y a [Amaroq sur l'AppStore](https://itunes.apple.com/us/app/amaroq-for-mastodon/id1214116200?mt=8) un client gratuit, bien réalisé.

Pour Android il existe [Tusky sur Google PlayStore](https://play.google.com/store/apps/details?id=com.keylesspalace.tusky)

## Avoir les colonnes qui prennent tout l'écran sur l'interface dans le navigateur

Il existe un script pour avoir l'interface en plein écran (https://userstyles.org/styles/135697/mastodon-style-tweaks)

à utiliser avec :

*  [GreaseMonkey sur Firefox](https://addons.mozilla.org/fr/firefox/addon/greasemonkey/)
*  [JSBlocker sur Safari](http://jsblocker.toggleable.com)

___
# La modération

## C'est quoi le SILENCE ?

Un administrateur peut poser un tag SILENCE sur un compte, ce compte ne sera lisible que par ses abonnés et ne sera pas visible dans les différentes timelines. Le SILENCE peut être aussi bien posé par l'administrateur de l'instance qui héberge le compte qu'un administrateur d'une autre instance.

___
# Je suis perdu(e)

## Comment retrouver mes amis de Twitter ?
Le [Mastodon Bridge](https://mastodon-bridge.herokuapp.com) a été conçu à cette fin. Se connecter en utilisant votre compte Twitter et votre compte Mastodon, il listera vos amis de Twitter qui ont aussi utilisé le Mastodon Bridge.


___
# Utilisation générale

## Les timelines

![Une explication des timelines](https://github.com/Sniperovitch/mastodon-faq-fr/blob/master/mastodon_timelines.png)

