# HTML6VRAI
<!DOCTYPE html>
<html lang="fr">

<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <!-- Le titre de la page  -->
  <title>Cours HTML</title>
  <!-- Icone de l'onglet -->
  <link rel="shortcut icon" href="html-logo.png" />
  <link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.8.2/css/all.css" />
</head>

<body>
  <header>
    <h1>Texte - Titre H1</h1>
    <p>
      <em>em pour mettre en italique</em>,
      <strong>strong pour mettre en gras</strong>
      <span>L'élement en span ne revient pas à la ligne</span>.
    </p>
    <p>
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Exercitationem
      cumque ratione veniam officiis nulla a debitis at facilis sed
      dignissimos.
    </p>
  </header>

  <section>
    <div>
      <h2>Photo - Titre H2</h2>
      <img src="./img-1.jpg" alt="image-arbre" height="500" />
    </div>

    <div>
      <h3>Liste - Titre H3</h3>
      <ul>
        <li>UL = unordered list</li>
        <li>UL = unordered list</li>
        <li>UL = unordered list</li>
      </ul>
      <ol>
        <li>OL = ordered list</li>
        <li>OL = ordered list</li>
        <li>OL = ordered list</li>
      </ol>
    </div>

    <div>
      <h4>Tableaux - Titre H4</h4>
      <table border="4" cellpadding="10" cellspacing="5" style="text-align: center">
        <thead>
          <tr>
            <th>Pays</th>
            <th>Population</th>
            <th>Superficie</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>France</td> 
            <td>67,75 millions (2021)</td>
            <td>551 695 km²</td>
          </tr>
          <tr>
            <td>Maroc</td>
            <td>37,08 millions (2021)</td>
            <td>710 850 km²</td>
          </tr>            
          
        </tbody>
      </table>
    </div>

    <div>
      <h5><span>&#9814;</span> Liens - Titre H5</h5>
      <a href="https://htmlcheatsheet.com/" target="_blank">HTML Cheatsheet</a>
      <br />
      <a href="https://www.toptal.com/designers/htmlarrows/symbols/" target="_blank">Icones natifs en HTML</a>
    </div>

    <div>
      <h6><i class="fas fa-video"></i> Vidéo - Titre H6</h6>
      <video src="video.mp4" height="500" autoplay loop muted></video>
    </div>
  </section>
  <br />
  <!-- Formulaires en HTML -->
  <section>
    <h2>Formulaire</h2>
    <form action="/action.php" method="post">
      <label for="name">Nom</label>
      <input id="name" type="text" placeholder="Entrez votre nom" /><br />

      <label for="number">Entrez votre age</label>
      <input type="number" id="number-age" value="15" oninput="document.getElementById('range-age').value=this.value">
      <input type="range" id="range-age" min="0" max="100"
        oninput="document.getElementById('number-age').value=this.value"><br />

      <!-- Input select -->
      <label for="gender">Genre</label>
      <select id="gender">
        <option selected="selected" value="Homme">Homme</option>
        <option value="Femme">Femme</option>
      </select><br />

      <!-- Input radio -->
      <div>
        <input type="radio" name="type" id="human" checked />
        <label for="human">Humain</label>

        <input type="radio" name="type" id="dog" />
        <label for="dog">Chien</label>

        <input type="radio" name="type" id="cat" />
        <label for="cat">Chat</label>
      </div>

      <textarea cols="20" rows="5" placeholder="Votre message..."></textarea><br />

      <!-- Input Checkbox -->
      <label><input type="checkbox" />Accepter les CGV</label> <br />
      <input type="submit" value="Submit" />
    </form>
  </section>
  <br />
  <!-- Mail & envoi de fichiers -->
  <footer>
    <a href="mailto:fs@gmail.com">Ecrivez-moi !</a>
    <br />
    <a href="notice.txt" download="nom-du-fichier">Télécharger la notice</a>
    <details>
      <summary>Plus d'infos</summary>
      <p>
        Lorem ipsum dolor, sit amet consectetur adipisicing elit. Harum,
        repellendus.
      </p>
    </details>
  </footer>
</body>

</html>
