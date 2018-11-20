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

### Generate Home Component and add it to router

    ng g c home

### Generate module(s) (section(s)) that contains component(s) (page(s)) with routing

    ng g m utilities --routing    
