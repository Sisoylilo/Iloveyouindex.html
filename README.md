<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Una pregunta importante 💙</title>

<style>
body{
    margin:0;
    height:100vh;
    display:flex;
    justify-content:center;
    align-items:center;
    background:linear-gradient(135deg,#87CEEB,#4A90E2);
    font-family:Arial,sans-serif;
    overflow:hidden;
}

.caja{
    text-align:center;
    background:white;
    padding:30px;
    border-radius:20px;
    box-shadow:0 0 20px rgba(0,0,0,0.2);
}

h1{
    color:#1E3A8A;
}

button{
    padding:12px 25px;
    font-size:18px;
    border:none;
    border-radius:12px;
    cursor:pointer;
    margin:10px;
}

#si{
    background:#4CAF50;
    color:white;
}

#no{
    background:#E53935;
    color:white;
    position:relative;
}

#mensaje{
    margin-top:20px;
    font-size:24px;
    color:#1E3A8A;
    font-weight:bold;
}
</style>
</head>

<body>

<div class="caja">
    <h1>💙Jeimy mishell ¿Quieres ser mi novia? 🥺💙</h1>

    <button id="si">Sí 💙</button>
    <button id="no">No 😈</button>

    <div id="mensaje"></div>
</div>

<script>
const botonNo = document.getElementById("no");
const botonSi = document.getElementById("si");
const mensaje = document.getElementById("mensaje");

function moverBoton() {
    const x = Math.random() * (window.innerWidth - 120);
    const y = Math.random() * (window.innerHeight - 60);

    botonNo.style.position = "absolute";
    botonNo.style.left = x + "px";
    botonNo.style.top = y + "px";
}

botonNo.addEventListener("mouseover", moverBoton);
botonNo.addEventListener("click", moverBoton);

botonSi.addEventListener("click", () => {
    document.body.innerHTML = `
        <div style="
            display:flex;
            justify-content:center;
            align-items:center;
            height:100vh;
            font-family:Arial;
            background:linear-gradient(135deg,#87CEEB,#4A90E2);
            color:white;
            text-align:center;
            font-size:40px;
            padding:20px;
        ">
            🎉💙 ¡Me hiciste la persona más feliz del mundo Mi amor! 💙🎉
        </div>
    `;
});
</script>

</body>
</html>
