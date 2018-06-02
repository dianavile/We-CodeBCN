#JavaScript in 1 dia

## [Visual Studio Code](https://code.visualstudio.com/)
Use a code editor

Webpage
- __HTML__: Hypertext MArkup Language (structure and content of page)
- __CSS__: Cascading Style Sheets (graphic design: layout & position of elements)
- __JavaScript__: Interaction of page (buttons)
__NOTE__: Both HTML and CSS are not a programmming language.

A webpage consist of a BOX model. 
Everything you see on a website consists of boxes.
Open web Dev (F12)

[Place holder](https://placeimg.com/)

- Content: the content
- Padding: limit between content and border
- Border: the border
- Margen: difference between the border and space outside

WE/CODE
HTML Exemplo
Index.html
```
<!DOCTYPE html>
<html lang="en">
<head>
 <meta charset="UTF-8">
 <meta name="viewport" content="width=device-width, initial-scale=1.0">
 <meta http-equiv="X-UA-Compatible" content="ie=edge">
 <title>IronGames</title>
 <link rel="stylesheet" href="styles.css">
</head>
<body>
 <!-- Header -->
 <header class="header-like">
   <h1><strong>Iron</strong>Games</h1>
 </header>

 <!-- Content -->
 <section class="games-section">
   <h2 class="games-title">¡Prueba nuestros apasionantes juegos!</h2>
   <div class="games-container">
     <article class="game-card">
         <a href="game.html"><img src="https://picsum.photos/300" alt="Imagen del juego"></a>
       <h3 class="game-card-text">Otra carta, por favor</h3>
       <p class="game-card-text">¿Eres capaz de ver el futuro? Demuéstralo... ¡si te atreves!</p>
     </article>
     <article class="game-card">
       <img src="https://picsum.photos/300" alt="Imagen del juego">
       <h3 class="game-card-text">El ahorcado</h3>
       <p class="game-card-text">El destino de un hombre yace en tus manos, ¿podrás salvarlo?</p>
     </article>
     <article class="game-card">
         <img src="https://picsum.photos/300" alt="Imagen del juego">
       <h3 class="game-card-text">¡Piedra, papel o tijera!</h3>
       <p class="game-card-text">Tres enemigos irreconciliables se enfrentan en una batalla eterna.</p>
     </article>
   </div>
 </section>

 <!-- Footer -->
 <footer class="footer-like">
   <p>Creado con orgullo por <strong>Iron</strong>hack</p>
 </footer>
</body>
</html>
```

Styles.css
```
//Esto primero es el css reset
* {
 margin: 0;
 padding: 0;
 font-family: sans-serif;
}

body {
 background-color: #F4F4F4;
 color: #2E3248;
 text-align: center;
 min-height: 100vh;
}

.header-like {
 padding-top: 2em;
 padding-bottom: 2em;
 width: 100%;
 position: relative;
 background-color: #2E3248;
 color: white;
 text-align: center;
}

.footer-like {
 padding-top: 2em;
 padding-bottom: 2em;
 position: absolute;
 width: 100%;
 bottom: 0;
 background-color: #2E3248;
 color: white;
 text-align: center;
}

.games-section {
 padding-top: 2em;
 padding-bottom: 2em;
}

.games-title {
 margin: 30px;
}

.games-container {
 display: flex;
 justify-content: space-evenly;
}

.game-card {
 width: 300px;
 margin-bottom: 2em;
 background-color: #FFF;
 border: 3px solid #2E3248;
 border-radius: 5px;
}

.game-card-text {
 margin: 10px;
}

#hint,
#mistery {
 font-size: 30px;
 border: 5px solid #2E3248;
 border-radius: 10%;
 padding: 10px;
 width: 60px;
}

.guess-section {
 width: 600px;
 margin: 150px auto;
 border: 5px solid #2E3248;
 border-radius: 5px;
 padding: 6px;
}

.game-board {
 display: flex;
 justify-content: space-around;
 align-items: center;
}

.buttons {
 display: flex;
 flex-direction: column;
}

button {
 margin: 3px;
}

#result {
 margin: 12px;
}
```
