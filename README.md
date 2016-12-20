//Markdown
pandoc -s readme.docx -t markdown -o readme.md
//angular:

1)Controlleur 
-------------
Dans fichier html
ng-controller = "nomduCtrl"

Dand JS :
function nomduCtrl ($scoop) {
     }

2) Modules 
----------
app = angular.module (monapp,[les modules angular externe à utilisés])
  app.conroller (nomDuconroleur,['$scoop', fontion à exectuer (&scoop) {


3) Routes                                        }
----------
app = angular.module (monapp,[monapp, ['ngRoute'])
app.config ('$routeProvider', function ($routeProvider) {
    $routeProvider
    .when (chemin URL,{templateUrl'partials/......'})
    .otherwise ({redrictTo : '/'})

4)model
-------

   a) Factory 
      -------
        Déclaration :
        app.factory ('nomdufactory', function() {})

        utilisation : 
        app.controller(controller,function($scoop,mafactory){
                                       }
        resultat  :  execute la fonction et retourne le return de la fonction global

   a) Provider

        Déclaration :
        app.provider ('nomduDrovider', function() {})

        utilisation : 
        app.controller(controller,function($scoop,mafactory){
                                    }
        resultat  : execute la fonction et retourne le return de la fonction local ($fonction())



   b) Service 

         Déclaration :
         app.service ('nomduService', function() {})

         utilisation : 
         app.controller(controller,function($scoop,mafactory){
                                       }
         resultat  :  return une fonction {objet objet }






 5)$routeParams : récuper le paramètre dans URL à déclarer dans app.controller ('Ctrl,function($scoop,$routeParams){
                                              }
               Exemple  : http://URL\:id (il récupère id) 



   6) 
