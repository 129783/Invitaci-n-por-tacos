# Invitaci-n-por-tacos
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>Broma de Tacos</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      text-align: center;
      margin-top: 100px;
    }

    h1 {
      font-size: 24px;
    }

    .opciones {
      margin-top: 30px;
    }

    .btn {
      padding: 10px 20px;
      margin: 10px;
      font-size: 16px;
      cursor: pointer;
      transition: 0.2s;
    }
  </style>
</head>
<body>
  <h1>Te invito a los tacos, tú pagas, ¿aceptas?</h1>
  <div class="opciones">
    <button class="btn" onclick="respuestaCorrecta()">
      Claro, yo encantada de pagar todos los tacos que te comas
    </button>

    <button class="btn" onclick="respuestaIncorrecta()">
      En vez de que tú pagues
    </button>

    <button class="btn" onclick="respuestaIncorrecta()">
      A ver, mejor yo te invito y tú pagas
    </button>
  </div>

  <script>
    let intentos = 0;

    function respuestaCorrecta() {
      alert("¡Sabía que dirías que sí! 🌮😁");
    }

    function respuestaIncorrecta() {
      intentos++;

      if (intentos === 1) {
        alert("Error al escoger su respuesta 😅");
      } else if (intentos === 2) {
        alert("¿No me quieres invitar a los tacos? 😢");
      } else {
        alert("Te vas a hacer viejilla, mejor invítame los tacos 😜");
      }
    }
  </script>
</body>
</html>
