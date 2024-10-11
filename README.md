# 30 Java Projects to Learn Java for Minecraft Plugin Development

## Beginner Projects (1-10)

### 1. Hello World
- **Description**: Create a simple Java program that prints "Hello, World!" to the console.
- **New**: Basic Java structure (`main()` method).
  ```java
  public static void main(String[] args) {
      System.out.println("Hello, World!");
  }

### 2. Simple Calculator
- **Description**: Make a basic calculator that can add, subtract, multiply, and divide two numbers from user input.
- **New**: Basic operators and user input (`Scanner` class).
  ```java
  Scanner scanner = new Scanner(System.in);
  int sum = num1 + num2;
  ```

### 3. Number Guessing Game
- **Description**: Write a game that generates a random number and lets the user guess the number.
- **New**: Random number generation (`Random` class), `if-else` statements.
  ```java
  Random rand = new Random();
  int number = rand.nextInt(100);
  ```

### 4. Basic Bank Account
- **Description**: Create a bank account class with methods to deposit, withdraw, and check the balance.
- **New**: Object-oriented programming (OOP) with classes and methods.
  ```java
  class BankAccount {
      double balance;
      void deposit(double amount) { balance += amount; }
  }
  ```

### 5. Palindrome Checker
- **Description**: Check if a given string is a palindrome (reads the same forward and backward).
- **New**: String manipulation and loops (`for` loop for iteration).
  ```java
  for (int i = 0; i < str.length() / 2; i++) { ... }
  ```

### 6. Tic-Tac-Toe
- **Description**: Implement a text-based Tic-Tac-Toe game where two players can play against each other.
- **New**: Arrays and basic game logic using a 2D array.
  ```java
  char[][] board = new char[3][3];
  ```

### 7. Prime Number Checker
- **Description**: Create a program that checks if a number is prime.
- **New**: Modulo operator and loop optimization (`break` in loops).
  ```java
  for (int i = 2; i < n; i++) { if (n % i == 0) break; }
  ```

### 8. Student Grades System
- **Description**: Develop a system that can store and calculate student grades, including averages and class rank.
- **New**: Array manipulation and basic statistics (finding max/min).
  ```java
  double[] grades = {85.0, 90.0, 78.0};
  ```

### 9. Factorial Calculator
- **Description**: Write a program to compute the factorial of a number using recursion.
- **New**: Recursion (calling a method within itself).
  ```java
  int factorial(int n) { return (n == 1) ? 1 : n * factorial(n - 1); }
  ```

### 10. Temperature Converter
- **Description**: Build a temperature converter to switch between Celsius and Fahrenheit.
- **New**: Simple mathematical formulas in methods.
  ```java
  double toFahrenheit(double celsius) { return celsius * 9/5 + 32; }
  ```

## Intermediate Projects (11-20)

### 11. Library System
- **Description**: Create a library management system that can store books and manage check-ins and check-outs.
- **New**: Collections (`ArrayList`) to store and manage objects.
  ```java
  ArrayList<Book> library = new ArrayList<>();
  ```

### 12. Shopping Cart
- **Description**: Create an e-commerce shopping cart where users can add, remove, and view items.
- **New**: Class relationships (has-a relationship between `Cart` and `Product`).
  ```java
  class Cart { ArrayList<Product> products = new ArrayList<>(); }
  ```

### 13. To-Do List
- **Description**: Build a simple to-do list application with persistent storage.
- **New**: File I/O for persistent storage (`BufferedWriter` and `BufferedReader`).
  ```java
  BufferedWriter writer = new BufferedWriter(new FileWriter("todo.txt"));
  ```

### 14. Basic Text Editor
- **Description**: Make a basic text editor that allows users to type and save text to a file.
- **New**: Handling user input and saving files using file I/O.
  ```java
  writer.write("Save this text.");
  ```

### 15. Chat Application (Single User)
- **Description**: Create a simple chat application where a single user can send and receive messages locally.
- **New**: Networking basics (`Socket` and `ServerSocket` classes).
  ```java
  ServerSocket server = new ServerSocket(1234);
  Socket client = server.accept();
  ```

### 16. Maze Generator
- **Description**: Develop a program that generates a random maze using a depth-first search algorithm.
- **New**: Algorithm implementation (depth-first search, backtracking).
  ```java
  boolean dfs(int x, int y) { ... }
  ```

### 17. Banking System with Multiple Accounts
- **Description**: Expand on the basic bank account by adding support for multiple accounts and transactions.
- **New**: Handling multiple objects using `HashMap`.
  ```java
  HashMap<String, BankAccount> accounts = new HashMap<>();
  ```

### 18. Password Manager
- **Description**: Create a basic password manager with encryption for storing credentials securely.
- **New**: Security and encryption (`Cipher` class for encryption).
  ```java
  Cipher cipher = Cipher.getInstance("AES");
  ```

### 19. Weather Application
- **Description**: Build a weather app that fetches weather data from an external API and displays it.
- **New**: External API calls (`HttpURLConnection` to fetch data).
  ```java
  HttpURLConnection connection = (HttpURLConnection) url.openConnection();
  ```

### 20. Currency Converter
- **Description**: Create a currency converter that fetches exchange rates from an API and converts values.
- **New**: JSON parsing and external libraries (using `Gson` or `Jackson`).
  ```java
  JsonParser parser = new JsonParser();
  JsonObject json = parser.parse(reader).getAsJsonObject();
  ```

## Advanced Projects (21-30)

### 21. GUI Calculator
- **Description**: Develop a graphical user interface (GUI) calculator using Java Swing.
- **New**: Graphical User Interface (GUI) with Java Swing.
  ```java
  JFrame frame = new JFrame();
  ```

### 22. Simple Text-Based RPG
- **Description**: Create a simple role-playing game (RPG) where a player can fight enemies, gain experience, and level up.
- **New**: Inheritance and polymorphism (`Player` and `Enemy` classes).
  ```java
  class Player extends Character { ... }
  ```

### 23. Chat Application with Multiple Users
- **Description**: Extend the single-user chat to support multiple users by using multi-threading.
- **New**: Multi-threading for handling multiple users.
  ```java
  new Thread(() -> handleClient(clientSocket)).start();
  ```

### 24. Mini Twitter Clone
- **Description**: Build a simplified version of Twitter where users can post, follow, and see a timeline.
- **New**: Simulating social media with a simple backend using OOP principles.
  ```java
  class Post { String content; User author; }
  ```

### 25. Simple Notepad Application
- **Description**: Create a basic notepad application using JavaFX, allowing users to write and save files.
- **New**: JavaFX for richer GUI development.
  ```java
  TextArea textArea = new TextArea();
  ```

### 26. Basic FTP Client
- **Description**: Build a basic FTP client that can upload and download files from an FTP server.
- **New**: Advanced networking, handling file uploads and downloads.
  ```java
  FTPClient ftpClient = new FTPClient();
  ```

### 27. Pacman Game
- **Description**: Create a Pacman game with ghosts, walls, and collectible dots.
- **New**: Game loop and animations with collision detection.
  ```java
  Timer timer = new Timer(50, e -> gameLoop());
  ```

### 28. Minecraft Plugin - Basic Commands
- **Description**: Start creating a Minecraft plugin by adding basic command functionality.
- **New**: Spigot/Bukkit API, creating a plugin and handling commands.
  ```java
  public boolean onCommand(CommandSender sender, Command command, String label, String[] args) { ... }
  ```

### 29. Minecraft Plugin - Custom Items
- **Description**: Create a custom item in Minecraft and handle events related to it.
- **New**: Custom item creation and event handling.
  ```java
  ItemStack customItem = new ItemStack(Material.DIAMOND);
  ```

### 30. Minecraft Plugin - Economy System
- **Description**: Develop an economy system for Minecraft using databases to store player balances.
- **New**: Using databases (