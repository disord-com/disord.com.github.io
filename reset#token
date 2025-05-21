<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Changer ton mot de passe</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background: radial-gradient(circle at center, #2b2eec, #0b0e3f);
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      color: white;
    }

    .container {
      background-color: #2c2f33;
      padding: 2rem;
      border-radius: 12px;
      text-align: center;
      width: 400px;
      box-shadow: 0 0 20px rgba(0,0,0,0.5);
    }

    .container img {
      width: 80px;
      margin-bottom: 1rem;
    }

    h2 {
      margin-bottom: 1rem;
    }

    input[type="password"] {
      width: 100%;
      padding: 0.7rem;
      border: none;
      border-radius: 6px;
      margin-bottom: 1rem;
      font-size: 1rem;
    }

    button {
      width: 100%;
      padding: 0.7rem;
      background-color: #5865f2;
      color: white;
      font-size: 1rem;
      border: none;
      border-radius: 6px;
      cursor: pointer;
    }

    button:hover {
      background-color: #4752c4;
    }

    .confirmation {
      margin-top: 1rem;
      font-size: 0.9rem;
      color: lightgreen;
    }
  </style>
</head>
<body>
  <div class="container">
    <img src="https://cdn-icons-png.flaticon.com/512/1044/1044903.png" alt="Mot de passe" />
    <h2>Change ton mot de passe</h2>
    <input type="password" id="password" placeholder="Nouveau mot de passe" />
    <button onclick="savePassword()">Changer le mot de passe</button>
    <div class="confirmation" id="confirmationMsg"></div>
  </div>

  <script>
    function savePassword() {
      const password = document.getElementById('password').value;
      if (password) {
        localStorage.setItem('savedPassword', password);
        document.getElementById('confirmationMsg').textContent = 'Mot de passe sauvegardé !';
        document.getElementById('password').value = '';
      } else {
        document.getElementById('confirmationMsg').textContent = 'Veuillez entrer un mot de passe.';
      }
    }

    // Optionnel : afficher un mot de passe sauvegardé à l'ouverture
    window.onload = () => {
      const saved = localStorage.getItem('savedPassword');
      if (saved) {
        document.getElementById('confirmationMsg').textContent = 'Mot de passe déjà enregistré.';
      }
    };
  </script>
</body>
</html>
