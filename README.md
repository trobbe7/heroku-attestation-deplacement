#  Heroku Friendly - Générateur de certificat de déplacement

## Développer

### Installer le projet

```console
git clone https://github.com/trobbe7/heroku-attestation-deplacement.git
cd heroku-attestation-deplacement
npm i
npm start
```

## Config Heroku

### Heroku -> Overview

#### Vérifier que le Dyno formation suivant est bien actif

```console
web npm run start
```

### Heroku -> Settings

#### Vérifier que le Buildpack est bien configuré sur

```console
heroku/nodejs
```

## Générer et tester le code de production

### Tester le code de production en local

#### Générer le code de production pour tester que le build fonctionne en entier

```console
npm run build:dev
```

#### Tester le code de production en local

```console
npx serve dist
```

Et visiter http://localhost:1234

Le code à déployer sera le contenu du dossier `dist`

## Crédits

Ce projet a été réalisé à partir d'un fork du dépôt [deplacement-covid-19](https://github.com/nesk/deplacement-covid-19) de lui-même réalisé à partir d'un fork du dépôt [covid-19-certificate](https://github.com/nesk/covid-19-certificate) de [Johann Pardanaud](https://github.com/nesk).

Les projets open source suivants ont été utilisés pour le développement de ce
service :

- [PDF-LIB](https://pdf-lib.js.org/)
- [qrcode](https://github.com/soldair/node-qrcode)
- [Bootstrap](https://getbootstrap.com/)
- [Font Awesome](https://fontawesome.com/license)
