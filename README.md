<!DOCTYPE html>
<html lang="pt">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>BoardGameHub</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <h1>BoardGameHub</h1>
        <nav>
            <ul>
                <li><a href="#">Início</a></li>
                <li><a href="#">Jogos</a></li>
                <li><a href="#">Resenhas</a></li>
                <li><a href="#">Contato</a></li>
            </ul>
        </nav>
    </header>
    <main>
        <h2>Bem-vindo ao BoardGameHub!</h2>
        <p>Descubra os melhores jogos de tabuleiro e compartilhe sua experiência.</p>
    </main>
    <footer>
        <p>&copy; 2025 BoardGameHub. Todos os direitos reservados.</p>
    </footer>
</body>
</html>
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f4f4f4;
    text-align: center;
}

header {
    background-color: #333;
    color: white;
    padding: 15px;
}

nav ul {
    list-style: none;
    padding: 0;
}

nav ul li {
    display: inline;
    margin: 0 15px;
}

nav ul li a {
    color: white;
    text-decoration: none;
}

footer {
    margin-top: 20px;
    background-color: #333;
    color: white;
    padding: 10px;
}
document.addEventListener("DOMContentLoaded", function() {
    let jogos = ["Catan", "Dixit", "Ticket to Ride", "Azul"];
    let index = 0;

    function mostrarJogo() {
        document.getElementById("jogo-destaque").textContent = jogos[index];
        index = (index + 1) % jogos.length;
    }

    setInterval(mostrarJogo, 3000);
});
