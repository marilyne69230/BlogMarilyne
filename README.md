
    *** COMMANDES INSTALLATION ***

    - composer create-project symfony/website-skeleton secondProject "5.4.*”
    - création fichier .php-version
    - création .env.local
    - DATABASE_URL="mysql://root:@127.0.0.1:3306/blog_marilyne"
    - cd blogMarilyne
    - symfony console doctrine:database:create

    *** DEPOT GIT ***
    - git init
    - git add .
    - git commit -m "first commit"
    - git branch -M main
    - git remote add origin https://github.com/marilyne69230/BlogMarilyne.git
    - git push -u origin main

    *** CREATION ENTITY ***
    - symfony console make:entity 
    - User (nom de l'entity)
    - symfony console make:migration (prepare la migration)
    - symfony console doctrine:migration:migrate (migration vers la BDD)