<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Motos Deportivas Yamaha, Kawasaki, BMW y Ducati</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
            color: #333;
            line-height: 1.6;
        }
        header {
            background-color: #333;
            color: white;
            padding: 1em 0;
            text-align: center;
        }
        nav {
            background-color: #444;
            color: white;
            padding: 0.5em 0;
            text-align: center;
        }
        nav a {
            color: white;
            text-decoration: none;
            padding: 0.7em 1.5em;
            display: inline-block;
        }
        nav a:hover {
            background-color: #555;
        }
        .container {
            max-width: 960px;
            margin: 20px auto;
            padding: 20px;
            background-color: white;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        .moto {
            border: 1px solid #ddd;
            margin-bottom: 20px;
            padding: 15px;
            border-radius: 6px;
            display: flex;
            gap: 20px;
            align-items: center;
            background-color: #f9f9f9;
        }
        .moto img {
            max-width: 200px;
            border-radius: 4px;
        }
        .moto-info {
            flex-grow: 1;
        }
        .moto-info h2 {
            margin-top: 0;
            color: #333;
        }
        .moto-info p {
            color: #666;
            margin-bottom: 5px;
        }
        .botones-moto {
            margin-top: 10px;
        }
        .comprar-btn {
            background-color: #007bff;
            color: white;
            padding: 10px 15px;
            text-decoration: none;
            border-radius: 5px;
            border: none;
            cursor: pointer;
            font-size: 0.9em;
            transition: background-color 0.3s ease;
            display: inline-block;
        }
        .comprar-btn:hover {
            opacity: 0.8;
        }
        .modal {
            display: none;
            position: fixed;
            z-index: 2; /* Asegura que esté por encima del primer modal */
            left: 0;
            top: 0;
            width: 100%;
            height: 100%;
            overflow: auto;
            background-color: rgba(0, 0, 0, 0.4);
        }
        .modal-content {
            background-color: #fefefe;
            margin: 15% auto;
            padding: 20px;
            border: 1px solid #888;
            width: 80%;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }
        .close {
            color: #aaa;
            float: right;
            font-size: 28px;
            font-weight: bold;
        }
        .close:hover,
        .close:focus {
            color: black;
            text-decoration: none;
            cursor: pointer;
        }
        .formulario-compra label {
            display: block;
            margin-bottom: 5px;
            font-weight: bold;
        }
        .formulario-compra input[type="text"],
        .formulario-compra input[type="email"],
        .formulario-compra input[type="tel"] {
            width: calc(100% - 12px);
            padding: 10px;
            margin-bottom: 15px;
            border: 1px solid #ccc;
            border-radius: 4px;
            box-sizing: border-box;
            font-size: 1em;
        }
        .formulario-compra select {
            width: calc(100% - 12px);
            padding: 10px;
            margin-bottom: 15px;
            border: 1px solid #ccc;
            border-radius: 4px;
            box-sizing: border-box;
            font-size: 1em;
        }
        .formulario-compra button {
            background-color: #28a745;
            color: white;
            padding: 12px 20px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 1em;
            margin-top: 10px;
            transition: background-color 0.3s ease;
        }
        .formulario-compra button:hover {
            background-color: #218838;
        }
        #graciasMensaje {
            display: none;
            margin-top: 20px;
            padding: 15px;
            background-color: #d4edda;
            color: #155724;
            border: 1px solid #c3e6cb;
            border-radius: 5px;
            text-align: center;
            font-size: 1.1em;
        }
    </style>
</head>
<body>
    <header>
        <h1>Motos Deportivas Yamaha, Kawasaki, BMW y Ducati</h1>
    </header>
    <nav>
        <a href="#">Inicio</a>
        <a href="#">Catálogo</a>
        <a href="#">Contacto</a>
    </nav>
    <div class="container">
        <div class="moto">
            <img src="https://www.motofichas.com/images/phocagallery/yamaha/yzf-r1m-2022/001-yamaha-yzf-r1m-2024-estudio-negro-01.jpg" alt="Yamaha YZF-R1M">
            <div class="moto-info">
                <h2>Yamaha YZF-R1M</h2>
                <p><strong>Precio:</strong> $520,000 MXN</p>
                <p><strong>Motor:</strong> 998cc, 4 cilindros en línea</p>
                <p><strong>Potencia:</strong> 200 HP</p>
                <p><strong>Características:</strong> Suspensión electrónica Öhlins, carrocería de carbono, telemetría.</p>
                <div class="botones-moto">
                    <button class="comprar-btn" onclick="mostrarFormularioCompra('Yamaha YZF-R1M')">Comprar</button>
                </div>
            </div>
        </div>

        <div class="moto">
            <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/f/fe/2009_Yamaha_YZF-R1.jpg/640px-2009_Yamaha_YZF-R1.jpg" alt="Yamaha YZF-R1">
            <div class="moto-info">
                <h2>Yamaha YZF-R1</h2>
                <p><strong>Precio:</strong> $360,000 MXN</p>
                <p><strong>Motor:</strong> 998cc, 4 cilindros en línea</p>
                <p><strong>Potencia:</strong> 200 HP</p>
                <p><strong>Características:</strong> Suspensión KYB, frenos ABS, control de tracción.</p>
                <div class="botones-moto">
                    <button class="comprar-btn" onclick="mostrarFormularioCompra('Yamaha YZF-R1')">Comprar</button>
                </div>
            </div>
        </div>

        <div class="moto">
            <img src="https://upload.wikimedia.org/wikipedia/commons/1/11/Kawasaki_Ninja_ZX-10_ABS_%28KRT_Edition%29_at_the_Tokyo_Motor_Show_2015-2.jpg" alt="Kawasaki Ninja ZX-10R">
            <div class="moto-info">
                <h2>Kawasaki Ninja ZX-10R</h2>
                <p><strong>Precio:</strong> $360,000 MXN</p>
                <p><strong>Motor:</strong> 998cc, 4 cilindros en línea</p>
                <p><strong>Potencia:</strong> 203 HP</p>
                <p><strong>Características:</strong> Suspensión Showa, frenos Brembo, electrónica avanzada.</p>
                <div class="botones-moto">
                    <button class="comprar-btn" onclick="mostrarFormularioCompra('Kawasaki Ninja ZX-10R')">Comprar</button>
                </div>
            </div>
        </div>

        <div class="moto">
            <img src="https://kawasakicapital.com.mx/cdn/shop/files/G1-10.jpg?v=1723244770&width=990" alt="Kawasaki Ninja ZX-6R">
            <div class="moto-info">
                <h2>Kawasaki Ninja ZX-6R</h2>
                <p><strong>Precio:</strong> $210,000 MXN</p>
                <p><strong>Motor:</strong> 636cc, 4 cilindros en línea</p>
                <p><strong>Potencia:</strong> 128 HP</p>
                <p><strong>Características:</strong> Suspensión Showa, frenos Nissin, quickshifter.</p>
                <div class="botones-moto">
                    <button class="comprar-btn" onclick="mostrarFormularioCompra('Kawasaki Ninja ZX-6R')">Comprar</button>
                </div>
            </div>
        </div>

        <div class="moto">
            <img src="https://www.yamahaferbel.com/static/agency-go-virtual/YAMAHA/YZF-R7/2023/YAMAHA-YZF-R7-2022-HERO-VERSION.jpg" alt="Yamaha YZF-R7">
            <div class="moto-info">
                <h2>Yamaha YZF-R7</h2>
                <p><strong>Precio:</strong> $190,000 MXN</p>
                <p><strong>Motor:</strong> 689cc, 2 cilindros en línea</p>
                <p><strong>Potencia:</strong> 72.4 HP</p>
                <p><strong>Características:</strong> Suspensión KYB, frenos Brembo, diseño R-Series.</p>
                <div class="botones-moto">
                    <button class="comprar-btn" onclick="mostrarFormularioCompra('Yamaha YZF-R7')">Comprar</button>
                </div>
            </div>
        </div>

        <div class="moto">
            <img src="https://m.media-amazon.com/images/I/71KROYu8DrL._AC_UF894,1000_QL80_FMwebp_.jpg" alt="BMW M 1000 RR">
            <div class="moto-info">
                <h2>BMW M 1000 RR</h2>
                <p><strong>Precio:</strong> $850,000 MXN</p>
                <p><strong>Motor:</strong> 999cc, 4 cilindros en línea</p>
                <p><strong>Potencia:</strong> 212 HP</p>
                <p><strong>Características:</strong> Suspensión electrónica, frenos Brembo, aerodinámica avanzada.</p>
                <div class="botones-moto">
                    <button class="comprar-btn" onclick="mostrarFormularioCompra('BMW M 1000 RR')">Comprar</button>
                </div>
            </div>
        </div>

        <div class="moto">
            <img src="https://dhqlmcogwd1an.cloudfront.net/images/phocagallery/BMW_Motorrad/m-1000-r-2023/01-bmw-m-1000-r-2023-estudio.jpg" alt="BMW S 1000 RR">
            <div class="moto-info">
                <h2>BMW S 1000 RR</h2>
                <p><strong>Precio:</strong> $450,000 MXN</p>
                <p><strong>Motor:</strong> 999cc, 4 cilindros en línea</p>
                <p><strong>Potencia:</strong> 207 HP</p>
                <p><strong>Características:</strong> Suspensión ajustable, frenos ABS Pro, modos de conducción.</p>
                <div class="botones-moto">
                    <button class="comprar-btn" onclick="mostrarFormularioCompra('BMW S 1000 RR')">Comprar</button>
                </div>
            </div>
        </div>

        <div class="moto">
            <img src="https://dhqlmcogwd1an.cloudfront.net/images/phocagallery/ducati/panigale-v4-2023/01-ducati-panigale-v4-2023-estudio-rojo-01.jpg" alt="Ducati Panigale V4 R">
            <div class="moto-info">
                <h2>Ducati Panigale V4 R</h2>
                <p><strong>Precio:</strong> $900,000 MXN</p>
                <p><strong>Motor:</strong> 998cc, V4</p>
                <p><strong>Potencia:</strong> 240.5 HP</p>
                <p><strong>Características:</strong> Suspensión Öhlins, frenos Brembo Stylema R, aerodinámica de MotoGP.</p>
                <div class="botones-moto">
                    <button class="comprar-btn" onclick="mostrarFormularioCompra('Ducati Panigale V4 R')">Comprar</button>
                </div>
            </div>
        </div>

        <div class="moto">
            <img src="https://ducatimadrid.com/wp-content/uploads/2024/03/PANI-SP2-BLANCA.jpg.webp" alt="Ducati Panigale V4 S">
            <div class="moto-info">
                <h2>Ducati Panigale V4 S</h2>
                <p><strong>Precio:</strong> $650,000 MXN</p>
                <p><strong>Motor:</strong> 1103cc, V4</p>
                <p><strong>Potencia:</strong> 214 HP</p>
                <p><strong>Características:</strong> Suspensión electrónica Öhlins, frenos Brembo Stylema, modos de conducción.</p>
                <div class="botones-moto">
                    <button class="comprar-btn" onclick="mostrarFormularioCompra('Ducati Panigale V4 S')">Comprar</button>
                </div>
            </div>
        </div>
    </div>

    <div id="modalCompra" class="modal">
        <div class="modal-content">
            <span class="close" onclick="cerrarFormularioCompra()">×</span>
            <h2>Información de Compra</h2>
            <p>Por favor, completa el siguiente formulario para realizar la compra de <strong id="nombreMotoCompra"></strong>:</p>
            <form class="formulario-compra" id="formularioCompra">
                <label for="nombre">Nombre:</label>
                <input type="text" id="nombre" required>

                <label for="apellidos">Apellidos:</label>
                <input type="text" id="apellidos" required>

                <label for="telefono">Número de Teléfono:</label>
                <input type="tel" id="telefono" required>

                <label for="email">Correo Electrónico:</label>
                <input type="email" id="email" required>

                <label for="direccionIp">Dirección IP:</label>
                <input type="text" id="direccionIp" readonly>

                <label for="estado">Estado de México:</label>
                <select id="estado" required>
                    <option value="">Seleccionar estado</option>
                    </select>

                <button type="button" onclick="enviarFormularioCompra()">Enviar Formulario</button>
            </form>
        </div>
    </div>

    <div id="graciasMensaje" style="display: none;">
        <h2>¡Gracias por su compra!</h2>
        <p>Su pedido ha sido recibido y será procesado en breve.</p>
    </div>

    <script>
        let motoSeleccionada = "";
        const estadosMexico = [
            "Aguascalientes", "Baja California", "Baja California Sur", "Campeche", "Chiapas", "Chihuahua", "Coahuila",
            "Colima", "Durango", "Estado de México", "Guanajuato", "Guerrero", "Hidalgo", "Jalisco", "Michoacán",
            "Morelos", "Nayarit", "Nuevo León", "Oaxaca", "Puebla", "Querétaro", "Quintana Roo", "San Luis Potosí",
            "Sinaloa", "Sonora", "Tabasco", "Tamaulipas", "Tlaxcala", "Veracruz", "Yucatán", "Zacatecas"
        ].sort();

        document.addEventListener('DOMContentLoaded', function() {
            const estadoSelect = document.getElementById('estado');
            estadosMexico.forEach(estado => {
                const option = document.createElement('option');
                option.value = estado;
                option.textContent = estado;
                estadoSelect.appendChild(option);
            });

            // Obtener la dirección IP del usuario (esto puede no funcionar en todos los entornos debido a CORS)
            fetch('https://api.ipify.org?format=json')
                .then(response => response.json())
                .then(data => {
                    document.getElementById('direccionIp').value = data.ip;
                })
                .catch(error => {
                    console.error('No se pudo obtener la dirección IP', error);
                    document.getElementById('direccionIp').value = 'No disponible';
                });
        });

        function mostrarFormularioCompra(nombreMoto) {
            motoSeleccionada = nombreMoto;
            document.getElementById("nombreMotoCompra").textContent = nombreMoto;
            document.getElementById("modalCompra").style.display = "block";
            document.getElementById("graciasMensaje").style.display = "none"; // Asegurarse de que el mensaje de gracias esté oculto al abrir el formulario
        }

        function cerrarFormularioCompra() {
            document.getElementById("modalCompra").style.display = "none";
        }

        function enviarFormularioCompra() {
            const nombre = document.getElementById("nombre").value;
            const apellidos = document.getElementById("apellidos").value;
            const telefono = document.getElementById("telefono").value;
            const email = document.getElementById("email").value;
            const direccionIp = document.getElementById("direccionIp").value;
            const estado = document.getElementById("estado").value;

            // Aquí puedes agregar la lógica para enviar los datos del formulario (por ejemplo, a un servidor)
            console.log("Datos del formulario:");
            console.log("Nombre:", nombre);
            console.log("Apellidos:", apellidos);
            console.log("Teléfono:", telefono);
            console.log("Email:", email);
            console.log("Dirección IP:", direccionIp);
            console.log("Estado:", estado);
            console.log("Moto Seleccionada:", motoSeleccionada);

            cerrarFormularioCompra();
            document.getElementById("graciasMensaje").style.display = "block";
        }
    </script>
</body>
</html>
