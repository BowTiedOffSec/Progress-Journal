# Progress-Journal



## **Learning Progress Update: Solidity Basics and Security**

### **Date: Nov 1 2024

Summary assisted by chat gpt

#### **Topics Covered**

1. **Structs and Arrays**  
   - **Concepts Learned**: 
     - Defined and used `structs` to create custom data types in Solidity (e.g., creating a `Person` or `Pet` struct).  I used the basics from cryptozombies but wasnt understadning certain concepts around structs and arrays so I decided to try to build my own contract and learn that way
     - Created and managed arrays to store multiple instances of a struct type (e.g., `Person[]` and `Pet[]` arrays).
   - **Key Skills Practiced**:
     - Adding new elements to arrays with `.push()`.
     - Using `array.length` to track the size of an array and to assign unique IDs for each element in a list.
   - **Exercise Example**: Built a "Pet Adoption" contract with a `registerPet` function to add pets to an array, demonstrating how to handle custom data and arrays in Solidity.

2. **Typecasting and Pseudo-Random Numbers**
   - **Concepts Learned**:
     - Typecasting in Solidity to convert data types (e.g., `bytes32` to `uint`).
     - Used `keccak256` hashing function combined with `abi.encodePacked` to create pseudo-random numbers.
   - **Key Skills Practiced**:
     - Generated random-like `uint` values from strings using `keccak256`.
     - Applied the modulus operator `%` to limit numbers to a specific range.
   - **Exercise Example**: Created a `_generateRandomDna` function in a "Zombie Factory" example to generate 16-digit DNA numbers from string inputs.

3. **Events in Solidity**
   - **Concepts Learned**:
     - Declared and emitted events to signal when specific actions occur on-chain (e.g., a new zombie creation).
   - **Key Skills Practiced**:
     - Used `emit` to trigger events and logged data that can be read by a front-end or dApp.
     - Structured event functions to notify when state-changing actions occur.
   - **Exercise Example**: Implemented a `NewZombie` event in the Zombie Factory, enabling a front-end to listen for and display new zombies in real-time.

4. **Security-Focused Development in Solidity**
   - **Concepts Learned**:
     - Reviewed Solidity code with a security mindset, focusing on common vulnerabilities and best practices.
   - **Security Considerations**:
     - **Unrestricted Array Growth**: Discussed potential gas implications with large arrays and explored ways to manage array size effectively.
     - **Input Validation**: Understood the importance of validating user inputs to maintain data integrity.
     - **Access Controls**: Recognized when to restrict function visibility and considered using modifiers (like `onlyOwner`) to limit access where necessary.
     - **Lifecycle Management**: Planned for functions to remove or update elements in arrays to prevent data bloat and keep contracts efficient.
   - **Takeaway Skills**:
     - Developed awareness of the **gas costs** associated with data storage in arrays.
     - Practiced identifying points where **access control** should be implemented.
     - Gained insight into array management strategies and best practices for maintaining contract data efficiently.

---

### **Next Steps**
- **More Practice**: Continue building small contracts to reinforce concepts of struct/array management, input validation, and typecasting.  I am finding I work well when doing things hands-on.  Going forward I think I will also analyze any online exercises or contracts from a securityy standpoint
- **Security Deep Dive**: Start exploring common Solidity security vulnerabilities in greater depth, including reentrancy, overflow/underflow, and gas optimization.
- **Documentation**: Regularly update this README with further insights and code examples to track progress and showcase learning milestones.



