
PASSAGE A ANGULAR 1 A 2:
http://blog.jhades.org/introduction-to-angular2-the-main-goals/ - 18/05/2015
http://blog.goyello.com/2015/06/23/angular-2/ - 23/06/2015 - first impressions on ng2
http://www.shmck.com/a-quick-look-at-angular-2-properties/ - 08/08/2015
https://www.youtube.com/watch?v=a6ffZa1szLM - 25/09/2015 - Preparing for AngularJS 2.0
https://www.youtube.com/watch?v=s0xootlbudI - 29/10/2015 - Getting Started with Angular 2

http://victorsavkin.com/post/110170125256/change-detection-in-angular-2 - 06/07/2015
http://angular-tips.com/blog/2015/09/migrating-directives-to-angular-2/ - 20/09/2015 - Migrating Directives to Angular 2
http://blog.mgechev.com/2015/09/30/lazy-loading-components-routes-services-router-angular-2/ - 30/09/2015 - Lazy loading

http://plnkr.co/edit/yEEt0pXjAtMivUa0keYe?p=catalogue - angular2 plunker starter

But d'angular2:
	- Plus de simplicité (suppression notions complexes du 1 comme communication avec les directives)
	- Plus de performance (webworkers, plus de databinding double sens, lazy loading,..)
	- Plus de compatibilité avec nouveaux standards et autres libraires (Web Component, shadow DOM, ES6 module system, plus de $apply(),..)



Plus de controllers > tout est composant

	@Component = @Directive + template
	@Directive = Ajout de comportement dans DOM

	Communication simplifiée:
	[prop] pour passer des infos à un composant enfant
	(event) pour récupérer des infos d'un composant enfant


Version DART abandonné (DART aussi) pour une version unique avec TypeScript (Microsoft)

'Rendering Layer' séparé de 'Application Layer', ce qui permet de:
	- Utiliser les webworkers des navigateurs
	- Un rendu coté serveur
	- Un rendu mobile natif ios/android

	> ng1 agit sur le DOM a chaque $digest, ng2 met a jour toutes les données puis modifi une seule fois le DOM > plus performant
	