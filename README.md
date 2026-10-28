# Manarat Al Firdaous — site source (prototype déployable)

## Structure

```
Manarat_Al_Firdaous_Deploy/
├── index.html          # Site public
├── styles.css          # Styles responsive
├── script.js           # Interactions, frise, projets et actualités
├── data.js             # Contenus initiaux et stockage local
├── admin.html          # Éditeur de DÉMONSTRATION (non sécurisé)
├── admin.js            # Logique de cet éditeur
└── assets/
    ├── logo-manarat.png
    └── images/
        └── classroom-illustration.svg  # Illustration locale originale
```

## Déployer

1. Décompressez le ZIP.
2. Dans Netlify (ou un hébergement statique), déployez le dossier `Manarat_Al_Firdaous_Deploy` comme racine du site ; `index.html` doit rester à la racine.
3. Vous pouvez aussi déposer ces fichiers dans le répertoire `public_html` d'un hébergement traditionnel.
4. Pour vérifier localement : ouvrez `index.html` ou lancez `python -m http.server 8000` dans le dossier et accédez à `http://localhost:8000`.

Les images nécessaires à l'affichage (logo et illustration de couverture) sont incluses. Les polices utilisent Google Fonts, avec polices de repli système lorsque l'accès est bloqué. L'illustration de couverture est **un visuel générique**, pas une photographie réelle de l'école.

## IMPORTANT : administration et contenu en production

L'interface `admin.html` est une **maquette d'éditeur local**. Elle n'est pas protégée par un mot de passe et ses changements sont sauvegardés uniquement dans le navigateur utilisé. Elle **ne publie pas** les changements pour tous les visiteurs. Ne la présentez pas comme un compte d'administration réel. Pour une gestion éditoriale en ligne, il faut intégrer un vrai CMS avec authentification, sauvegarde serveur, rôle et workflow de validation.

Le formulaire de contact utilise l'application de messagerie du visiteur : il ne réceptionne pas automatiquement les demandes sur le serveur. Une adresse officielle doit être configurée. Les portraits, photographies de mineurs, résultats, dates et chiffres devront être validés par l'établissement avant lancement public.

Cette archive est donc **un site statique publiable comme démo**, et non une application de gestion scolaire complète prête pour une exploitation institutionnelle.
