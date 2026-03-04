<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<title>EXANI-II Competencia 50 Reactivos</title>
<style>
body{font-family:Arial;background:#eef2f7;text-align:center;}
.container{background:white;width:90%;margin:auto;padding:20px;border-radius:12px;box-shadow:0 0 12px gray;}
button{display:block;width:60%;margin:8px auto;padding:10px;border:none;border-radius:6px;background:#2563eb;color:white;cursor:pointer;}
button:hover{background:#1e40af;}
.score{font-size:18px;margin:10px;}
h2{color:#1e3a8a;}
</style>
</head>
<body>

<div class="container">
<h2>🎮 EXANI-II Competencia por Equipos (50 Reactivos)</h2>

<div class="score">
🔴 Equipo Rojo: <span id="scoreRed">0</span> |
🔵 Equipo Azul: <span id="scoreBlue">0</span>
</div>

<h3 id="turno">Turno: Equipo Rojo 🔴</h3>
<div id="quiz"></div>
<button onclick="nextQuestion()">Siguiente</button>
<h3 id="final"></h3>
</div>

<script>

const questions = [

/* 1-15 Matemáticas */
{q:"1. 15% de 200 =", options:["20","25","30","35"], answer:2},
{q:"2. 7 x 8 =", options:["54","56","64","48"], answer:1},
{q:"3. 144 ÷ 12 =", options:["10","11","12","13"], answer:2},
{q:"4. Raíz cuadrada de 64 =", options:["6","7","8","9"], answer:2},
{q:"5. 3/5 equivale a:", options:["6/10","9/10","5/6","4/5"], answer:0},
{q:"6. Área de cuadrado lado 6 =", options:["12","24","36","30"], answer:2},
{q:"7. 9² =", options:["81","72","99","79"], answer:0},
{q:"8. 5x=35 x=", options:["5","6","7","8"], answer:2},
{q:"9. Promedio de 2,4,6 =", options:["3","4","5","6"], answer:1},
{q:"10. 250 - 75 =", options:["150","175","180","200"], answer:1},
{q:"11. 8³ =", options:["512","256","64","128"], answer:0},
{q:"12. 20% de 50 =", options:["5","10","15","20"], answer:1},
{q:"13. 6+4×2 =", options:["20","14","16","18"], answer:1},
{q:"14. 18 ÷ 3 =", options:["5","6","7","8"], answer:1},
{q:"15. 2x=18 x=", options:["8","9","10","7"], answer:1},

/* 16-30 Comprensión */
{q:"16. Texto narrativo:", options:["Cuenta hechos","Explica","Convence","Enumera"], answer:0},
{q:"17. Sinónimo de grande:", options:["Pequeño","Amplio","Corto","Débil"], answer:1},
{q:"18. Antónimo de frío:", options:["Helado","Caliente","Fresco","Tibio"], answer:1},
{q:"19. Idea principal:", options:["Detalle","Tema central","Ejemplo","Título"], answer:1},
{q:"20. 'Sin embargo' expresa:", options:["Causa","Tiempo","Contraste","Orden"], answer:2},
{q:"21.
