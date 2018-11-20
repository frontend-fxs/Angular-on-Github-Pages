# Angular-on-Github-Pages
## How to publish an Angular App into Github Pages

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
