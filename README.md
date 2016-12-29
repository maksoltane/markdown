//Markdown
pandoc -s readme.docx -t markdown -o readme.md
//angular:Foutain webapp

1)Controlleur 
-------------
Dans fichier html
ng-controller = "nomduCtrl"

Dand JS :
function nomduCtrl ($scoop) {
     }

2) Modules 
----------
angular
.module (monapp,[les modules angular externe à utilisés])
.conroller (nomDuconroleur,['$scoop', fontion à exectuer (&scoop) {


3) Routes                                        }
----------
angular
.module (monapp,[monapp, ['ngRoute'])
.config ('$routeProvider', function ($routeProvider) {
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


6) IComponentOptions : 

interface IComponentOptions {
 controller?: any;
 controllerAs?: string;
 template?: string | Function;
 templateUrl?: string | Function;
 bindings?: any;
 transclude?: boolean;
 require?: Object;
 $canActivate?: () => boolean;
 $routeConfig?: RouteDefinition[];
}
/teambox/resource-rest/V1_1/collaborateurs/
08YWRtaW5pdG90bw==
