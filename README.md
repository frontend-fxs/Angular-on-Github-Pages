# Angular-on-Github-Pages
## How to publish an Angular App into Github Pages using angular CLI

    ng new fxstreetEditorsLayoutGuideline --routing --skipTests --verbose

index.html change this

    <base href="https://frontend-fxs.github.io/fxstreetEditorsLayoutGuideline/">
    
angular.json change this

    "outputPath": "docs",
   
build

    ng build --prod

inside docs folder duplicate  index.html  to 404.html

Push to github

publish from docs folder

### Generate Home Component

    ng g c home
    
### Add HomeComponent to router
    
    const routes: Routes = [
    
        { path: '/home', component: HomeComponent },
        
         { path: '', pathMatch: 'full', redirectTo: 'home' }
         
    ];
 And import homeComponent into the  header of  app-routing.module.ts
 
 ### Add router links into the app menu app.component.html
 
    <a [routerLink]="['/home']">Home</a>

### Generate module(s) (section(s)) that contains component(s) (page(s)) with routing

    ng g m utilities --routing   -m app.module
    
#### Create first component as default page of the module

    ng g c utilities
