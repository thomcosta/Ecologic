# Ecologic
Open source web application for registration of recyclable waste collection points

<img src="https://i.postimg.cc/L8jLJKQt/ecoleta-tela1.jpg" height="600" widith="800">
  This one is zoomed out 50%:
<img src="https://i.postimg.cc/MZhYHDK8/cadastro-tela2.jpg" height="600" widith="800">


## How it was build:
With Node.js and using Nunjucks as a template engine to increment and make HTML dynamic. It has a SQL database with MySQL for the registration of waste collection points, and uses IBGE(Brasilian institute of geography and statistics) database to grab states and cities infos.

    Obs: It has a Express server confuguration that must to be changed (for "false") before uploaded to a web host:
                     
                     in - server.js:
                            const nunjucks = require("nunjucks")
                            nunjucks.configure ("src/views",{ 
                                express: server,
                                noCache: true //change for false
                                  })
      
## Folder structure
    pontos_de_coleta  
      public
        assets 
           imagens.svg
        scripts
           index.js
         styles
            main.css
      src
          database
             db.js
          views
             index.html
          server.js
      node_modules    
    
 ###### Feel free to use and contribute
    It has responsive pages, also very basic, that must be improoved as the search features.
 Created by Thom M. Costa based on a RocketSeat bootcamp project - 2020 jun.
