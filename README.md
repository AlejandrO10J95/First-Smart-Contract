📈 Smart Calculator - Solidity Smart Contract
📋 Summary
The Smart Calculator is a blockchain-based smart contract, developed in Solidity, designed to perform basic mathematical operations (addition, subtraction, and multiplication) securely and auditable. This project showcases best practices in smart contract development, including security modifiers, event emissions for greater transparency, and modular design.

Built and tested with Remix IDE using Solidity 0.8.24.

✨ Features
➕ Addition: Adds two numbers.

➖ Subtraction: Subtracts two numbers (both in uint256 and int256).

✖️ Multiplication: Multiplies the stored result by a given number.

🔒 Security Modifier: checkNumber ensures validated input for critical operations.

🧩 Events: Addition and subtraction events provide full transparency in transactions.

🧠 Smart Contract Details
🔹 Main Functions

Function	Description	Visibility	Returns
addition(uint256 num1_, uint256 num2_)	Adds two unsigned integers.	public	uint256
substraction(uint256 num1_, uint256 num2_)	Subtracts two unsigned integers.	public	uint256
substraction2(int256 num1_, int256 num2_)	Subtracts two signed integers.	public	int256
multiplier(uint256 num1_)	Multiplies the result by a given number.	public	-
multiplier2(uint256 num1_)	Multiplies the result by a number only if num1_ == 10.	public	-
🔹 Events

Event	Parameters	Description
Addition	uint256 number1, uint256 number2, uint256 result	Emitted when addition is successful.
Subtraction	uint256 number1, uint256 number2, uint256 result	Emitted when subtraction is successful.
🛠️ Tools Used
Solidity: 0.8.24

IDE: Remix IDE (Ethereum)

Solidity Compiler: version 0.8.24

Testing Environment: Remix VM (Cancún)

🚀 Implementation and Testing Steps
Open Remix IDE: Visit Remix IDE.

Create the contract file: Create a new file Calculator.sol and paste the smart contract code.

Compile: Go to the Solidity Compiler tab, select version 0.8.24, and click "Compile Calculator.sol".

Deploy: Go to the "Deploy & Run Transactions" tab, select "Remix VM (Cancún)" as the environment, and click "Deploy".

Interact: Use the deployed interface to call functions like addition, subtraction, multiplication, etc.

✅ Contract Tests
🧪 Functional Tests
Basic Addition: addition(5, 7) → expected result: 12.

Basic Subtraction: substraction(10, 3) → expected result: 7.

Multiplication: multiplier(2) → doubles the current result.

🛡️ Security Tests
Input Validation in multiplier2: Only multiplies if the input is 10, otherwise, the transaction reverts.

Event Emissions: Each successful operation emits the corresponding event.

🧪 Edge Cases
Large Numbers: Test operations with values close to 2**256-1.

Zero Inputs: Validates behavior when one or both numbers are 0.

Negative Numbers: Uses substraction2 with int256 inputs to correctly handle negative numbers.

🖼️ Visual Diagram
Here’s a simple flowchart that shows the main functions of the contract:

(Suggestion: If you upload the diagram in your repository, use a relative path like /docs/diagram.png).

🔮 Future Improvements
Add descriptive error messages for greater clarity.

Extend operations to include division, modulus, and exponentiation.

Add multi-role access control (e.g., only the owner can call multiplier2).

Integrate frontend interaction (e.g., React.js dApp frontend).

📜 License
This project is licensed under LGPL-3.0 only.

👨‍💻 Author
Blockchain Developer: [Your Name or Nickname]
GitHub: [Your GitHub Profile]
LinkedIn: [Your LinkedIn Profile]

Thank you for visiting this project! Open to collaborations and blockchain opportunities! 🔥

This structured and professional format will make your project more attractive and accessible to blockchain recruiters. The clear separation of sections and emphasis on functionality, testing, and future improvements is a perfect setup to impress a recruiter!








