# 💳 Personal Finance Management System

A console‑based application developed in Java to manage credit cards, track different types of purchases (one‑time, installments, recurring), generate monthly statements and send credit‑limit alerts.

## 📌 Features

- ✅ One‑time purchase registration  
- ✅ Installment purchase registration  
- ✅ Recurring purchase registration (e.g., subscriptions)  
- ✅ Detailed monthly statement generation  
- ✅ Credit‑card closing‐date configuration  
- ✅ Credit‑limit alert functionality  
- ✅ Interactive text‐menu interface with looped operations  

## 🛠 Technologies Used

- Java (JDK 8+)  
- Object‑Oriented Programming  
- Console / Terminal‐based UI  
- SQL‑style in‑memory/backed data management (if applicable)  

## 🧩 Project Structure

| File / Class | Responsibility |
|-------------|----------------|
| `Main.java` | Entry point of the application |
| `CartaoCredito.java` | Holds credit‑card data: limit, current balance, list of purchases |
| `Compra.java` | Abstract base class for purchase types |
| `CompraAVista.java` | Implements one‑time purchases |
| `CompraParcelada.java` | Manages purchases split across multiple installments |
| `CompraRecorrente.java` | Represents monthly recurring payments (subscriptions) |
| `Fatura.java` | Generates the monthly summary of purchases based on closing date |
| `Menu.java` | Handles user interaction via terminal menu system |

## 🚀 How to Run

1. Clone the repository  
   ```bash
   git clone https://github.com/matheusbaeta/GerenciamentoDeFinancas.git
   ```  
2. Navigate into the project folder  
   ```bash
   cd GerenciamentoDeFinancas
   ```  
3. Compile the Java sources (assuming JDK is installed)  
   ```bash
   javac src/*.java
   ```  
4. Run the application  
   ```bash
   java src.Main
   ```  
(Adjust paths as needed depending on your folder structure.)

## 💡 Usage Example

```text
======= MENU =======
1. Register one‑time purchase  
2. Register installment purchase  
3. Register recurring purchase  
4. Generate current invoice  
5. View available credit limit  
6. Exit  
=====================
Choose an option:
```

## 🧭 Future Improvements

- [ ] Add persistent data storage (e.g., file system, SQLite, or other DB) to retain data across runs  
- [ ] Add user account support (multi‑card/multi‑user)  
- [ ] Add a GUI (Swing / JavaFX) version for improved usability  
- [ ] Add detailed analytics (e.g., monthly spending breakdown, category filtering)  
- [ ] Add unit tests and continuous integration  
- [ ] Add input validation, error‑handling and a richer UI menu experience  

## 📝 License

This project is licensed under the MIT License – see the [LICENSE](LICENSE) file for details.

---
