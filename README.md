# Projet_n_2_michel_mbaka
/* Définition des polices personnalisées */

@font-face
{
    font-family: 'BallparkWeiner';
    src: url('polices/ballpark.eot');
    src: url('polices/ballpark.eot?#iefix') format('embedded-opentype'),
         url('polices/ballpark.woff') format('woff'),
         url('polices/ballpark.ttf') format('truetype'),
         url('polices/ballpark.svg#BallparkWeiner') format('svg');
    font-weight: normal;
    font-style: normal;
}

@font-face
{
    font-family: 'Dayrom';
    src: url('polices/dayrom.eot');
    src: url('polices/dayrom.eot?#iefix') format('embedded-opentype'),
         url('polices/dayrom.woff') format('woff'),
         url('polices/dayrom.ttf') format('truetype'),
         url('polices/dayrom.svg#Dayrom') format('svg');
    font-weight: normal;
    font-style: normal;
}
/* Eléments principaux de la page */

body
{
    background: url('images/fond_jaune.png');
    font-family: 'Trebuchet MS', Arial, sans-serif;
    color: #181818;
}
#bloc_page
{
    width: 900px;
    margin: auto;
}
@media all and (max-device-width: 480px)
{
    #bloc_page
    {
        width: auto;
    }
}

section h1, footer h1, nav a
{
    font-family: Dayrom, serif;
    font-weight: normal;
    text-transform: uppercase;
}
/* Header */

header
{
    background: url('images/separateur.png') repeat-x bottom;
    display: flex;
    justify-content: space-between;
    align-items: flex-end;
}

#titre_principal
{
    display: flex;
    flex-direction: column;
}

#logo
{
    display: flex;
    flex-direction: row;
    align-items: baseline;
}

#logo img
{
    width: 59px;
    height: 60px;
}
@media all and (max-device-width: 480px)
{
   #logo img
    {
        width: 20px;
        height: 30px;
    } 
}

header h1
{
    font-family: 'BallparkWeiner', serif;
    font-size: 2.5em;
    font-weight: normal;
    margin: 0 0 0 10px;
}
@media all and (max-device-width: 480px)
{

    header h1
    {
       font-size: 1em;
    }
}

header h2
{
    font-family: Dayrom, serif;
    font-size: 1.1em;
    margin-top: 0px;
    font-weight: normal;
}
@media all and (max-device-width: 480px)
{

    header h2
    {
       font-size: 0,1em;
    }
}
/* Navigation */

nav ul
{
    list-style-type: none;
    display: flex;
}

nav li
{
    margin-right: 15px;
}
@media all and (max-device-width: 480px)
{

    nav li
    {
       font-size: 7px;
    }
}

nav a
{
    font-size: 1.3em;
    color: #181818;
    padding-bottom: 3px;
    text-decoration: none;
}
@media all and (max-device-width: 480px)
{

    nav a
    {
       font-size: 0,3em;
       padding-bottom: 1px;
    }
}


nav a:hover
{
    color: #760001;
    border-bottom: 3px solid #760001;
}
@media all and (max-device-width: 480px)
{

    nav a:hover
    {
       border-bottom: 1px solid #760001;
    }
}
@media all and (max-device-width: 480px)
{
    nav
    {
        width: auto;
        text-align: left;
    }
    
    nav ul
    {
        flex-direction: column;
    }

    nav li
    {
        padding-left: 4px;
    }
    @media all and (max-device-width: 480px)
{
    nav li
    {
        padding-left: 2px;
    }
}
    
    
    nav a
    {
        font-size: 1.1em;
    }
       @media all and (max-device-width: 480px)
{
    nav a
    {
        font-size: 0.1em;
    }
}
    
    nav a:hover
    {
        border-bottom: 0;
    }
}

/* Bannière */

#banniere_image
{
    margin-top: 15px;
    height: 200px;
    border-radius: 5px;
    background: url('images/sanfrancisco.jpg') no-repeat;
    position: relative;
    box-shadow: 0px 4px 4px #1c1a19;
    margin-bottom: 25px;
}
@media all and (max-width: 1024px)
{
    #banniere_image
    {
        display: none;
    }
}

#banniere_description
{
    position: absolute;
    bottom: 0;
    border-radius: 0px 0px 5px 5px;
    width: 99.5%;
    height: 33px;
    padding-top: 15px;
    padding-left: 4px;
    background-color: rgba(24,24,24,0.8);
    color: white;
    font-size: 0.8em;  
}
@media all and (max-device-width: 480px)
{
    section
    {
        flex-direction: column;
    }

    article, aside
    {
        width: auto;
        margin-bottom: 15px;
    }
    
    #fleche_bulle
    {
        display: none;
    }
    
    #photo_zozor img
    {
        width: 110px;
        float: right;
        margin-left: 15px;
    }
    
    aside p:last-child
    {
        text-align: center;
    }
}

.bouton_rouge
{
    height: 25px;
    position: absolute;
    right: 5px;
    bottom: 5px;
    background: url('images/fond_degraderouge.png') repeat-x;
    border: 1px solid #760001;
    border-radius: 5px;
    font-size: 1em;
    text-align: center;
    padding: 3px 8px 0px 8px;
    color: white;
    text-decoration: none;
}

.bouton_rouge img
{
    border: 0;
}

/* Corps */

section
{
    display: flex;
    margin-bottom: 20px;
}

article, aside
{
    text-align: justify;
}

article
{
    margin-right: 20px;
    flex: 3;
}

.ico_categorie
{
    vertical-align: middle;
    margin-right: 8px;
}

article p
{
    font-size: 0.8em;
}

aside
{
    flex: 1.2;
    position: relative;
    background-color: #706b64;
    box-shadow: 0px 2px 5px #1c1a19;
    border-radius: 5px;
    padding: 10px;
    color: white;
    font-size: 0.9em;
}

#fleche_bulle
{
    position: absolute;
    top: 100px;
    left: -12px;
}

#photo_zozor
{
    text-align: center;
}

#photo_zozor img
{
    border: 1px solid #181818;
}

aside img
{
    margin-right: 5px;
}

/* Footer */

footer
{
    display: flex;
    background:  url('images/ico_top.png') no-repeat top center, url('images/separateur.png') repeat-x top, url('images/ombre.png') repeat-x top;
    padding-top: 25px;
}

footer p, footer ul
{
    font-size: 0.8em;
}

footer h1
{
    font-size: 1.1em;
}


#tweet
{
    width: 28%;
}

#mes_photos
{
    width: 35%;
}

#mes_amis
{
    width: 31%;
}

#mes_photos img
{
    border: 1px solid #181818;
    margin-right: 2px;
}

#listes_amis
{
    display: flex;
    justify-content: space-between;
    margin-top: 0;
}

#mes_amis ul
{
    list-style-image: url('images/ico_liensexterne.png');
    padding-left: 2px;
}

#mes_amis a
{
    text-decoration: none;
    color: #760001;
}
