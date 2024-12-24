<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>RSVP - Aniversário na Praia</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background: url('https://source.unsplash.com/1600x900/?beach') no-repeat center center/cover;
        }
        .form-container {
            background-color: rgba(255, 255, 255, 0.8);
            padding: 2rem;
            border-radius: 10px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
            width: 90%;
            max-width: 500px;
        }
        h1 {
            text-align: center;
            color: #333;
        }
        label {
            display: block;
            margin-top: 1rem;
            color: #555;
        }
        input, select, textarea {
            width: 100%;
            padding: 0.8rem;
            margin-top: 0.5rem;
            border: 1px solid #ccc;
            border-radius: 5px;
            font-size: 1rem;
        }
        button {
            margin-top: 2rem;
            width: 100%;
            padding: 1rem;
            background-color: #007BFF;
            color: white;
            border: none;
            border-radius: 5px;
            font-size: 1rem;
            cursor: pointer;
            transition: background-color 0.3s;
        }
        button:hover {
            background-color: #0056b3;
        }
    </style>
</head>
<body>
    <div class="form-container">
        <h1>Confirme sua Presença</h1>
        <form action="https://formspree.io/f/mvoeydbd" method="POST">
            <label for="name">Nome Completo:</label>
            <input type="text" id="name" name="name" required>

            <label for="days">Vai participar:</label>
            <select id="days" name="days" required>
                <option value="semana toda">Semana toda</option>
                <option value="alguns dias">Alguns dias</option>
            </select>

            <label for="food">O que pretende levar de comida?</label>
            <textarea id="food" name="food" rows="3"></textarea>

            <label for="carpool">Precisa de carona?</label>
            <select id="carpool" name="carpool" required>
                <option value="nao">Não</option>
                <option value="sim">Sim</option>
            </select>

            <button type="submit">Enviar RSVP</button>
        </form>
    </div>
</body>
</html>

