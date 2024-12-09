To run the Number Guessing Game client-server Java application, follow these instructions:

---

### Prerequisites
1. **Java Development Kit (JDK):** Ensure that the JDK is installed on your system.
   - Check installation: `java -version` and `javac -version`
   - If not installed, download and install from [Oracle JDK](https://www.oracle.com/java/technologies/javase-downloads.html) or use OpenJDK.

2. **Integrated Development Environment (IDE) (Optional):** You can use an IDE like IntelliJ IDEA, Eclipse, or NetBeans, or work directly from the command line.

3. **Networking Setup:** The server and client must run on the same network.
   - Use `localhost` if running on the same machine.
   - Use the server's IP address if running on different machines.

---

### Steps to Run the Code

#### 1. **Save the Code**
- Create a directory named `javasocket`.
- Save the server code as `Server.java` in the `javasocket` directory.
- Save the client code as `Client.java` in the same directory.

#### 2. **Compile the Code**
Open a terminal or command prompt and navigate to the `javasocket` directory.

Run the following command to compile the code:
```bash
javac Server.java Client.java
```
This will generate `Server.class` and `Client.class` files.

#### 3. **Run the Server**
- Start the server first to allow it to listen for client connections.
- Run the following command:
```bash
java Server
```
You should see:
```
Server is waiting for connection...
```

#### 4. **Run the Client**
- Open another terminal or command prompt, navigate to the same `javasocket` directory, and run the client:
```bash
java Client
```
- If the server is on another machine, replace `localhost` in the `Client.java` code with the server's IP address before compiling and running.

#### 5. **Play the Game**
- The client will display instructions from the server.
- Enter your guesses when prompted.
- The server will respond with feedback until the correct number is guessed.

---

### Example Interaction

#### **On the Server Console:**
```
Server is waiting for connection...
Client connected!
```

#### **On the Client Console:**
```
Welcome to the Number Guessing Game! I have selected a number between 1 and 100. Try to guess it.
Enter your guess: 50
Too low! Try again.
Enter your guess: 75
Too high! Try again.
Enter your guess: 62
Correct! You've guessed the number in 3 attempts.
```

---

### Notes
- If running on different machines, ensure the server's firewall allows connections on port `9999`.
- You can customize the port or the range of random numbers by modifying the variables in the code.
