

# 🏧 ATM Machine using Java & JDBC

## 📌 Project Description

This project is a **console-based ATM Machine application** developed using **Java** and **JDBC (Java Database Connectivity)**.
It allows users to log in using credentials stored in a **MySQL database** and perform basic ATM operations such as:

* Withdraw money
* Deposit money
* Check account balance
* Exit the system

The project demonstrates **database connectivity**, **user authentication**, and **menu-driven programming** in Java.

---

## 🛠️ Technologies Used

* **Java**
* **JDBC**
* **MySQL**
* **MySQL Connector/J**
* **Eclipse / IntelliJ / VS Code**
* **Command Line Interface**

---

## 🗄️ Database Details

### Database Name

```
pydb
```

### Table Name

```
atm
```

### Table Structure

```sql
CREATE TABLE atm (
    loginid VARCHAR(50),
    pin VARCHAR(10)
);
```

### Sample Data

```sql
INSERT INTO atm VALUES ('user1', '1234');
INSERT INTO atm VALUES ('user2', '5678');
```

---

## ⚙️ Features

* Secure login using **login ID and PIN**
* Withdraw amount with balance validation
* Deposit amount
* Check available balance
* Menu-driven loop until user exits
* Exception handling for database and input errors

---

## ▶️ How to Run the Project

### Step 1: Install Requirements

* Install **Java JDK**
* Install **MySQL Server**
* Download **MySQL Connector/J (JDBC Driver)**

### Step 2: Setup Database

1. Open MySQL
2. Create database and table
3. Insert user credentials

### Step 3: Configure JDBC

Update the connection string in the code:

```java
DriverManager.getConnection(
    "jdbc:mysql://localhost:3306/pydb",
    "root",
    "Aakash@1"
);
```

⚠️ Replace username and password as per your system.

### Step 4: Compile & Run

```bash
javac AtmMachine.java
java AtmMachine
```

---

## 🖥️ Application Flow

1. User enters **login ID and PIN**
2. System validates credentials from MySQL
3. Displays ATM menu
4. Performs selected operation
5. Continues until user exits

---

## 📂 Project Structure

```
AtmMachine.java
README.md
```


## 🚀 Future Enhancements

* Store balance in database
* Encrypt PIN for security
* Add transaction history
* Multi-user account support
* GUI using Java Swing / JavaFX

---

## 👩‍💻 Author

**Meghana Kongara**
B.Tech CSE (AI)
Srivasavi Engineering College

---

## 📜 License

This project is for **educational purposes only**.


