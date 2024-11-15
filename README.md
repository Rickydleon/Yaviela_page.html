<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Un Viaje de Momentos Especiales</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f0f0f0;
            color: #333;
            margin: 0;
            padding: 0;
            text-align: center;
        }
        h1 {
            color: #333;
            margin-top: 50px;
        }
        p {
            width: 80%;
            margin: 0 auto;
            font-size: 18px;
            line-height: 1.6;
        }
        .question {
            font-size: 24px;
            color: #4a4a4a;
            margin-top: 30px;
        }
        .buttons {
            margin-top: 20px;
        }
        .buttons button {
            background-color: #333;
            color: white;
            border: none;
            padding: 10px 20px;
            font-size: 18px;
            border-radius: 5px;
            cursor: pointer;
            margin: 10px;
        }
        .buttons button:hover {
            background-color: #555;
        }
    </style>
    <script>
        function showMemory1() {
            document.getElementById("initialText").style.display = "none";
            document.getElementById("memory1").style.display = "block";
        }

        function showMemory2() {
            document.getElementById("memory1").style.display = "none";
            document.getElementById("memory2").style.display = "block";
        }

        function showMemory3() {
            document.getElementById("memory2").style.display = "none";
            document.getElementById("memory3").style.display = "block";
        }

        function revealQuestion() {
            document.getElementById("memory3").style.display = "none";
            document.getElementById("questionText").style.display = "block";
        }

        function positiveResponse() {
            alert('Sabía que dirías que sí! 😊 Aquí comienza nuestro siguiente capítulo.');
        }

        function funnyResponse1() {
            alert('¿De verdad lo dudaste? 😜 Me parece que ya sabías la respuesta.');
        }

        function funnyResponse2() {
            alert('Si esto fuera un examen de opciones, marcaría “Sí” y pondría un corazón al lado ❤');
        }

        function playfulResponse() {
            alert('Esa es una respuesta con truco… pero la acepto 😉');
        }

        function friendZoneResponse() {
            alert('Ouch, eso dolió 😅 Pero seguiré siendo optimista, porque me caes demasiado bien.');
        }
    </script>
</head>
<body>
    <h1>Un Viaje de Momentos Especiales</h1>
    <p id="initialText">Te preparé algo que creo que te gustará… toca el botón cuando estés lista para comenzar.</p>
    
    <button onclick="showMemory1()" style="background-color: #4a90e2; color: white; padding: 10px 25px; border: none; font-size: 18px; border-radius: 5px; cursor: pointer; margin-top: 20px;">
        Comenzar el viaje
    </button>

    <div id="memory1" style="display: none;">
        <p class="question">📅 7 de noviembre</p>
        <p>Ese día fue el primer beso. ¿Te acuerdas? Fue tan inesperado y perfecto que no dejo de pensar en eso. Parece que ese día marcó el inicio de algo grande.</p>
        <button onclick="showMemory2()">Siguiente</button>
    </div>

    <div id="memory2" style="display: none;">
        <p class="question">📍 La Distancia</p>
        <p>Aunque estamos lejos, siento que cada día nos conectamos más. Y, bueno, no voy a mentir… te extraño bastante. Cada llamada, cada mensaje hace que me sienta un poquito más cerca de ti.</p>
        <button onclick="showMemory3()">Siguiente</button>
    </div>

    <div id="memory3" style="display: none;">
        <p class="question">🤭 Algo que aún no te he dicho...</p>
        <p>Aunque en nuestra última despedida no tuve tiempo de decírtelo, quiero preguntarte algo importante. Sé que esto puede sonar un poco directo, pero...</p>
        <button onclick="revealQuestion()">Dímelo ya</button>
    </div>

    <div id="questionText" style="display: none;">
        <p class="question">¿Quieres ser mi novia?</p>
        <p>Responde con sinceridad y sin presiones… pero quiero saber si te gustaría dar este paso conmigo.</p>
        <div class="buttons">
            <button onclick="positiveResponse()">Sí, claro que sí</button>
            <button onclick="funnyResponse1()">No estaba segura, pero ahora… ¡Sí!</button>
            <button onclick="funnyResponse2()">¿Por qué no? ¡Me encantan los riesgos! 😜</button>
            <button onclick="playfulResponse()">Depende… ¿Vas a invitarme a cenar primero? 😆</button>
            <button onclick="friendZoneResponse()">Solo como amigos, pero con cariño</button>
        </div>
    </div>
</body>
</html>
