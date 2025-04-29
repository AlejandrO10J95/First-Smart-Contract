📈 Smart Calculator - Solidity Smart Contract
📋 Overview
The Smart Calculator is a blockchain-based smart contract developed in Solidity, designed to perform basic mathematical operations (addition, subtraction, and multiplication) in a secure and auditable way.
This project showcases best practices in smart contract development, including security modifiers, event emissions for transparency, and modular design.

Built and tested using Remix IDE with Solidity 0.8.24.

✨ Features
➕ Addition: Adds two numbers.

➖ Subtraction: Subtracts two numbers (both uint256 and int256 versions).

✖️ Multiplication: Multiplies the stored result by a given number.

🔒 Security Modifier: checkNumber ensures validated input for critical operations.

🧩 Events: Addition and Substraction events provide full transaction transparency.

🧠 Smart Contract Details
🔹 Main Functions

Function	Description	Visibility	Returns
addition(uint256 num1_, uint256 num2_)	Adds two unsigned integers.	public	uint256
substraction(uint256 num1_, uint256 num2_)	Subtracts two unsigned integers.	public	uint256
substraction2(int256 num1_, int256 num2_)	Subtracts two signed integers.	public	int256
multiplier(uint256 num1_)	Multiplies the result by a given number.	public	-
multiplier2(uint256 num1_)	Multiplies the result by a number (only if num1_ == 10).	public	-
🔹 Events

Event	Parameters	Description
Addition(uint256 number1, uint256 number2, uint256 result)	Emitted upon successful addition.	
Substraction(uint256 number1, uint256 number2, uint256 result)	Emitted upon successful subtraction.	
🛠️ Tools Used
Solidity: 0.8.24

Remix IDE: Remix Ethereum IDE

Solidity Compiler: Version 0.8.24

Testing Environment: Remix VM (Cancún)

🚀 Deployment and Testing Steps
1. Open Remix IDE
Visit Remix IDE.

2. Create the Contract File
Create a new file Calculadora.sol and paste the smart contract code.

3. Compile
Go to the Solidity Compiler tab.

Select compiler version 0.8.24.

Click Compile Calculadora.sol.

4. Deploy
Go to Deploy & Run Transactions tab.

Select Remix VM (Cancún) as the environment.

Click Deploy.

5. Interact
Use the deployed interface to call functions like addition, substraction, multiplier, and more.

✅ Contract Testing
🧪 Functional Tests
Basic Addition: addition(5, 7) → expected result: 12.

Basic Subtraction: substraction(10, 3) → expected result: 7.

Multiplication: multiplier(2) → doubles the current result.

🛡️ Security Tests
Input Validation in multiplier2: Only multiplies if input is 10, otherwise transaction reverts.

Event Emissions: Each successful operation emits a corresponding event.

🧪 Edge Cases
Large Numbers: Test operations with values close to 2**256-1.

Zero Inputs: Validate behavior when one or both numbers are 0.

Negative Numbers: Use substraction2 with int256 inputs to handle negatives correctly.

🖼️ Visual Diagram
Here is a simple flowchart showcasing the core contract functions:


(Tip: If you upload the diagram to your own repo, use a relative path like /docs/diagram.png)

🔮 Future Improvements
Add descriptive require error messages for more clarity.

Expand operations to include division, modulus, and exponentiation.

Add multi-role access control (e.g., only owner can call multiplier2).

Integrate front-end interaction (e.g., React.js dApp frontend).

📜 License
This project is licensed under LGPL-3.0-only.

👨‍💻 Author
Blockchain Developer: [Your Name or Nickname]

GitHub: [Your GitHub Profile]

LinkedIn: [Your LinkedIn Profile]

🚀 Thanks for visiting this project! Open for collaborations and Blockchain opportunities!
🔥 Short Description for GitHub About
Solidity smart contract for basic secure math operations. Developed with best practices in Solidity 0.8.24 and deployed on Remix IDE. Events and modifiers ensure transparent and safe operations.
