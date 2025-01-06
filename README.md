# Creación de una página web básica para Tezla Wash utilizando HTML y CSS.

# Código HTML y CSS estructurado como archivo único.
html_code = """
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tezla Wash</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #1a1a1a;
            color: white;
        }
        header {
            background-color: #000;
            padding: 20px;
            text-align: center;
        }
        header h1 {
            color: #00aaff;
        }
        nav {
            display: flex;
            justify-content: center;
            background-color: #222;
            padding: 10px 0;
        }
        nav a {
            color: white;
            text-decoration: none;
            margin: 0 15px;
            font-size: 16px;
        }
        nav a:hover {
            color: #ff0000;
        }
        .container {
            padding: 20px;
        }
        .services, .about, .contact, .booking {
            margin: 30px 0;
        }
        h2 {
            color: #ff0000;
            text-align: center;
        }
        .service-table {
            width: 100%;
            margin: 20px 0;
            border-collapse: collapse;
        }
        .service-table th, .service-table td {
            border: 1px solid #444;
            padding: 10px;
            text-align: center;
        }
        .service-table th {
            background-color: #333;
        }
        .service-table td {
            background-color: #222;
        }
        .button {
            display: inline-block;
            background-color: #ff0000;
            color: white;
            padding: 10px 20px;
            text-align: center;
            text-decoration: none;
            border-radius: 5px;
            font-size: 16px;
        }
        .button:hover {
            background-color: #cc0000;
        }
        footer {
            text-align: center;
            padding: 20px;
            background-color: #000;
            color: #aaa;
            font-size: 14px;
        }
    </style>
</head>
<body>
    <header>
        <h1>Tezla Wash</h1>
        <p>Lavados de autos a domicilio, donde quiera que estés</p>
    </header>
    <nav>
        <a href="#services">Servicios</a>
        <a href="#booking">Reservas</a>
        <a href="#about">Sobre Nosotros</a>
        <a href="#contact">Contacto</a>
    </nav>
    <div class="container">
        <section id="services" class="services">
            <h2>Servicios</h2>
            <table class="service-table">
                <tr>
                    <th>Servicio</th>
                    <th>Precio</th>
                </tr>
                <tr>
                    <td>Lavado Básico (Sedán)</td>
                    <td>$35</td>
                </tr>
                <tr>
                    <td>Lavado Básico (SUV)</td>
                    <td>$40</td>
                </tr>
                <tr>
                    <td>Lavado Básico (Camioneta)</td>
                    <td>$55</td>
                </tr>
                <tr>
                    <td>Brillo a mano</td>
                    <td>Desde $35</td>
                </tr>
                <tr>
                    <td>Secado en cerámica</td>
                    <td>Desde $10</td>
                </tr>
                <tr>
                    <td>Eliminación de mal olor</td>
                    <td>Desde $15</td>
                </tr>
                <tr>
                    <td>Detallado interior</td>
                    <td>Desde $20</td>
                </tr>
                <tr>
                    <td>Remoción de manchas (por asiento)</td>
                    <td>Desde $15</td>
                </tr>
            </table>
        </section>
        <section id="booking" class="booking">
            <h2>Reservas</h2>
            <form action="#" method="post">
                <label for="vehicle">Selecciona tu vehículo:</label><br>
                <select id="vehicle" name="vehicle" required>
                    <option value="sedan">Sedán</option>
                    <option value="suv">SUV</option>
                    <option value="truck">Camioneta</option>
                </select><br><br>
                <label for="services">Selecciona servicios adicionales:</label><br>
                <input type="checkbox" name="additional" value="brillo"> Brillo a mano<br>
                <input type="checkbox" name="additional" value="ceramica"> Secado en cerámica<br>
                <input type="checkbox" name="additional" value="mal-olor"> Eliminación de mal olor<br>
                <input type="checkbox" name="additional" value="detallado"> Detallado interior<br>
                <input type="checkbox" name="additional" value="manchas"> Remoción de manchas<br><br>
                <label for="date">Fecha:</label><br>
                <input type="date" id="date" name="date" required><br><br>
                <label for="contact">Tu información:</label><br>
                <input type="text" id="name" name="name" placeholder="Nombre" required><br><br>
                <input type="text" id="phone" name="phone" placeholder="Teléfono" required><br><br>
                <input type="email" id="email" name="email" placeholder="Email" required><br><br>
                <button type="submit" class="button">Reservar</button>
            </form>
        </section>
        <section id="about" class="about">
            <h2>Sobre Nosotros</h2>
            <p>Tezla Wash nació como un concepto innovador: un Tesla Model 3 diseñado para ofrecer servicios de lavado de autos a domicilio. Combinamos tecnología, calidad y conveniencia para cuidar de tu vehículo.</p>
        </section>
        <section id="contact" class="contact">
            <h2>Contacto</h2>
            <p>Ian Rodríguez</p>
            <p>Teléfono: 787-710-6170</p>
            <p>Email: <a href="mailto:sito9120@hotmail.com" style="color: #00aaff;">sito9120@hotmail.com</a></p>
        </section>
    </div>
    <footer>
        <p>&copy; 2025 Tezla Wash. Todos los derechos reservados.</p>
    </footer>
</body>
</html>
"""

# Guardar el código como un archivo HTML.
file_path = "/mnt/data/Tezla_Wash.html"
with open(file_path, "w") as file:
    file.write(html_code)

file_path