# BQE Angular WebAPP served as Github Page

## STEPS:


//Package.json for build
1.  "build:client": "ng build --prod --output-path docs --base-href /apiexplorer/",

//app.module.ts for routing
2.  a. {provide: APP_BASE_HREF, useValue: '/apiexplorer/'},
     b. {provide: LocationStrategy, useClass: HashLocationStrategy}

//app.routing.ts for hash based routing
3.  {useHash: true}

Note: For Logo
Remove Forward slash under main.js

