symfony new digit_event_V4 --full
symfony console make:controller
git init 
git add .
git commit -m 'first'
git remote add origin (lien)
(git remote rm digitevent: au cas ou cela existe déjé)
git push -u origin master

ensuite 
git add .
git commit -m 'second'
git push

integrer le template admin dans public ,creer les parties, les assets, includs et exends 
Data base: digit_event_V4 et MailHog (port 1025 dans .env et 8025 dans le navigateur)
Creer les bases 1 et 2 pour visiteur et organisateur 
Lancer le serveur wamp, creer la base et les pages register et login
definir la route de redirection
php bin/console doctrine:database:create
symfony console make:user /auth /registration-form
symfony console doctrine:schema:update --force
comptes creer: test1@test.tg et lawsonerick19228@gmail.com ( MP: 654321)

mot de pass oublier:installer composer require symfonycasts/reset-password-bundle 
entrer symfony console make:reset-password


symfony console make:auth
php bin/console make:migration
php bin/console d:m:m

composer require easycorp/easyadmin-bundle
php bin/console make:admin:dashboard
symfony console make:admin:crud

npm install --force
npm run dev


yarn install sass-loader@^9.0.1 node-sass --save-dev

symfony new billetweb --full
composer require symfony/webpack-encore-bundle
npm install --force
modififier dans assets/styles (scss dans app.css)
symfony serve -d


symfony new digit_event --full

readme.md
symfony serve -d
symfony server:stop
php bin/console doctrine:database:create

Creation des entite
symfony console make:entity organisateur/Visiteur/Admin/Publication/Evenement
symfony console make:form 

php bin/console doctrine:database:create
php bin/console make:migration
php bin/console d:m:m

EventController
symfony console make:controller

Utilisatateurs (test@test.tg et test@test.tg ; MP: testtest)
symfony console make:user Utilisateurs
symfony console make:registration-form
route , redirection vers event ( dans le Todo) 
composer require symfony/webpack-encore-bundle
npm install --force

modififier dans assets/styles (scss dans app.css)

npm install sass-loader@^12.0.0 --save-dev
npm install postcss-loader autoprefixer --dev
npm run build ( pour builder les fichiers)

postcss.config.js

module.exports = {
	plugins: {
		autoprefixer: {}
	}
}

decomenter .enableSassLoader() dans  webpack.config.js 
npm install bootstrap

@import "~bootsrap/scss/bootstrap";

npm install jquery @popperjs/core --save-dev

meta name="viewport" content="width=device-width, initial-scale=1">
et les link javascrip et css et bootstrap 