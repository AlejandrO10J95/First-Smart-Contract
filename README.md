📈 Calculadora Inteligente - Contrato Inteligente en Solidity

📋 Resumen del Proyecto

La Calculadora Inteligente es un contrato inteligente basado en blockchain, desarrollado en Solidity, diseñado para realizar operaciones matemáticas esenciales (suma, resta y multiplicación) de forma segura y transparente. Este proyecto sigue las mejores prácticas en el desarrollo de contratos inteligentes, incluyendo el uso de modificadores de seguridad, emisiones de eventos para mayor transparencia y diseño modular.

Construido y probado con Remix IDE usando Solidity 0.8.24.

✨ Características Clave


➕ Suma: Suma dos números.


➖ Resta: Resta dos números (soporta tanto uint256 como int256).


✖️ Multiplicación: Multiplica el resultado almacenado por un número dado.


🔒 Modificador de Seguridad: checkNumber asegura la validación de entradas para operaciones críticas.


🧩 Eventos: Los eventos de suma y resta garantizan transparencia total en las transacciones.


🧠 Detalles del Contrato Inteligente

🔹 Funciones Principales

Función	                                         Descripción	                                                        Visibilidad	              Retorna

addition(uint256 num1_, uint256 num2_)	         Suma dos enteros sin signo.	                                          pública	                uint256 

substraction(uint256 num1_, uint256 num2_)	     Resta dos enteros sin signo.	                                          pública	                uint256 

substraction2(int256 num1_, int256 num2_)	       Resta dos enteros con signo.	                                          pública	                int256 

multiplier(uint256 num1_)	                       Multiplica el resultado por un número dado.	                          pública	                  -

multiplier2(uint256 num1_)	                     Multiplica el resultado por un número solo si num1_ == 10.	            pública	                  -


🔹 Eventos

Evento	                    Parámetros	                                            Descripción
Addition	                  uint256 number1, uint256 number2, uint256 result	      Emitido cuando la suma es exitosa.
Subtraction	                uint256 number1, uint256 number2, uint256 result	      Emitido cuando la resta es exitosa.


🛠️ Tecnologías Utilizadas

Solidity: 0.8.24

IDE: Remix IDE (Ethereum)

Compilador de Solidity: versión 0.8.24

Entorno de Pruebas: Remix VM (Cancún)


🚀 Pasos de Implementación y Pruebas

Abrir Remix IDE: Visita Remix IDE.

Crear el Archivo del Contrato: Crea un nuevo archivo Calculator.sol y pega el código del contrato.

Compilar el Contrato: Ve a la pestaña del Compilador de Solidity, selecciona la versión 0.8.24 y haz clic en "Compilar Calculator.sol".

Desplegar el Contrato: En la pestaña "Deploy & Run Transactions", selecciona "Remix VM (Cancún)" y haz clic en "Deploy".

Interactuar con el Contrato: Usa la interfaz desplegada para llamar a funciones como suma, resta, multiplicación, etc.


✅ Pruebas del Contrato

🧪 Pruebas Funcionales

Suma Básica: addition(5, 7) → resultado esperado: 12.

Resta Básica: substraction(10, 3) → resultado esperado: 7.

Multiplicación: multiplier(2) → duplica el resultado actual.


🛡️ Pruebas de Seguridad

Validación de Entrada en multiplier2: La transacción se revierte a menos que la entrada sea 10.

Emisión de Eventos: Las operaciones exitosas emiten los eventos correspondientes.


🧪 Pruebas de Casos Límite

Números Grandes: Prueba con valores cercanos a 2**256-1.

Entradas Cero: Valida el comportamiento cuando uno o ambos números son 0.

Números Negativos: Maneja números negativos utilizando substraction2 con entradas int256.


🔮 Mejoras Futuras

Agregar mensajes de error descriptivos para mayor claridad.

Ampliar la funcionalidad para incluir división, módulo y exponenciación.

Implementar control de acceso con múltiples roles (por ejemplo, solo el propietario puede llamar a multiplier2).

Integrar interacción con el frontend (por ejemplo, frontend dApp en React.js).


📜 Licencia
Este proyecto está licenciado bajo LGPL-3.0 únicamente.


👨‍💻 Autor
Desarrollador Blockchain: [Alejandro Gómez]
GitHub: [Alejandro10J95]
LinkedIn: [www.linkedin.com/in/alejandro-gómez-martínez-123404259]

¡Gracias por visitar este proyecto! Abierto a colaboraciones y oportunidades en blockchain! 🔥
