📈 Calculadora Inteligente - Contrato Inteligente en Solidity

📋 Resumen del Proyecto

La Calculadora Inteligente es un contrato inteligente basado en blockchain, desarrollado en Solidity, diseñado para realizar operaciones matemáticas esenciales (suma, resta y multiplicación) de forma segura y transparente.
Este proyecto sigue buenas prácticas de desarrollo en contratos inteligentes, incluyendo modificadores de seguridad, emisión de eventos y diseño modular.

Construido y probado con Remix IDE usando Solidity 0.8.24.

✨ Características Clave

➕ Suma: Suma dos números.

➖ Resta: Resta dos números (uint256 e int256).

✖️ Multiplicación: Multiplica el resultado almacenado por un número dado.

🔒 Modificador de Seguridad: checkNumber para validar entradas críticas.

🧩 Eventos: Emite eventos en cada operación para garantizar transparencia.



🧠 Detalles del Contrato Inteligente
🔹 Funciones Principales
add(uint256 num1_, uint256 num2_): Suma dos números enteros sin signo.

resta(uint256 num1_, uint256 num2_): Resta dos números enteros sin signo.

resta2(int256 num1_, int256 num2_): Resta dos números enteros con signo.

multiplicador(uint256 num1_): Multiplica el resultado almacenado por el número proporcionado.

multiplicador2(uint256 num1_): Multiplica el resultado solo si el número proporcionado es exactamente 10.

🔹 Eventos
Suma(uint256 numero1, uint256 numero2, uint256 resultado): Emitido al realizar una suma exitosa.

Resta(uint256 numero1, uint256 numero2, uint256 resultado): Emitido al realizar una resta exitosa.

🛠️ Tecnologías Utilizadas
Solidity: 0.8.24

IDE: Remix IDE (Ethereum)

Compilador de Solidity: versión 0.8.24

Entorno de Pruebas: Remix VM (Cancún)

🚀 Pasos de Implementación y Pruebas
Abrir Remix IDE y acceder a https://remix.ethereum.org/.

Crear el archivo Calculator.sol y pegar el código del contrato.

Compilar el contrato usando la versión 0.8.24 de Solidity.

Desplegar el contrato seleccionando Remix VM (Cancún) en "Deploy & Run Transactions".

Interactuar con las funciones desplegadas: suma, resta, multiplicación, etc.

✅ Pruebas del Contrato
🧪 Pruebas Funcionales
Suma básica: add(5, 7) → Resultado esperado: 12.

Resta básica: resta(10, 3) → Resultado esperado: 7.

Multiplicación: multiplicador(2) → Duplica el resultado almacenado.

🛡️ Pruebas de Seguridad
Validación en multiplicador2: Rechaza transacciones si el número no es exactamente 10.

Eventos: Cada operación correcta emite su evento correspondiente.

🧪 Pruebas de Casos Límite
Números grandes: Probar valores cercanos a 2**256 - 1.

Entradas de cero: Validar cuando uno o ambos números son 0.

Números negativos: Usar resta2 para manejar valores int256.

🔮 Mejoras Futuras
Agregar mensajes de error personalizados.

Ampliar operaciones: división, módulo, exponenciación.

Control de acceso con múltiples roles (por ejemplo, que solo el propietario use multiplicador2).

Crear un frontend de interacción (por ejemplo, dApp en React.js).

📜 Licencia
Este proyecto está licenciado bajo LGPL-3.0 únicamente.

👨‍💻 Autor
Desarrollador Blockchain: Alejandro Gómez


GitHub: Alejandro10J95


LinkedIn: Alejandro Gómez Martínez


¡Gracias por visitar este proyecto!
Abierto a colaboraciones y oportunidades en Blockchain 🚀🔥
