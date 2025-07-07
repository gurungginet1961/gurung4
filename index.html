// Main.java
public class Main {
    public static void main(String[] args) {
        StockTradingApp app = new StockTradingApp();
        app.start();
    }
}

// User.java
import java.util.ArrayList;

public class User {
    private String username;
    private String password;
    private Portfolio portfolio;

    public User(String username, String password) {
        this.username = username;
        this.password = password;
        this.portfolio = new Portfolio();
    }

    public String getUsername() {
        return username;
    }

    public String getPassword() {
        return password;
    }

    public Portfolio getPortfolio() {
        return portfolio;
    }
}

// Stock.java
public class Stock {
    private String name;
    private double price;

    public Stock(String name, double price) {
        this.name = name;
        this.price = price;
    }

    public String getName() {
        return name;
    }

    public double getPrice() {
        return price;
    }
}

// Portfolio.java
import java.util.HashMap;

public class Portfolio {
    private HashMap<String, Integer> stocks;

    public Portfolio() {
        stocks = new HashMap<>();
    }

    public void buyStock(String stockName, int quantity) {
        stocks.put(stockName, stocks.getOrDefault(stockName, 0) + quantity);
    }

    public void sellStock(String stockName, int quantity) {
        if (stocks.containsKey(stockName) && stocks.get(stockName) >= quantity) {
            stocks.put(stockName, stocks.get(stockName) - quantity);
            if (stocks.get(stockName) == 0) {
                stocks.remove(stockName);
            }
        } else {
            System.out.println("Not enough stocks to sell.");
        }
    }

    public void displayPortfolio() {
        System.out.println("Your Portfolio:");
        for (String stock : stocks.keySet()) {
            System.out.println(stock + ": " + stocks.get(stock));
        }
    }
}

// StockTradingApp.java
import java.util.ArrayList;
import java.util.Scanner;

public class StockTradingApp {
    private ArrayList<User> users;
    private ArrayList<Stock> availableStocks;
    private User loggedInUser ;

    public StockTradingApp() {
        users = new ArrayList<>();
        availableStocks = new ArrayList<>();
        initializeStocks();
    }

    private void initializeStocks() {
        availableStocks.add(new Stock("Apple", 150.00));
        availableStocks.add(new Stock("Google", 2800.00));
        availableStocks.add(new Stock("Amazon", 3400.00));
    }

    public void start() {
        Scanner scanner = new Scanner(System.in);
        while (true) {
            System.out.println("1. Register");
            System.out.println("2. Login");
            System.out.println("3. Exit");
            int choice = scanner.nextInt();
            scanner.nextLine(); // Consume newline

            switch (choice) {
                case 1:
                    registerUser (scanner);
                    break;
                case 2:
                    loginUser (scanner);
                    break;
                case 3:
                    System.out.println("Exiting...");
                    return;
                default:
                    System.out.println("Invalid choice. Please try again.");
            }
        }
    }

    private void registerUser (Scanner scanner) {
        System.out.print("Enter username: ");
        String username = scanner.nextLine();
        System.out.print("Enter password: ");
        String password = scanner.nextLine();
        users.add(new User(username, password));
        System.out.println("User  registered successfully!");
    }

    private void loginUser (Scanner scanner) {
        System.out.print("Enter username: ");
        String username = scanner.nextLine();
        System.out.print("Enter password: ");
        String password = scanner.nextLine();

        for (User  user : users) {
            if (user.getUsername().equals(username) && user.getPassword().equals(password)) {
                loggedInUser  = user;
                System.out.println("Login successful!");
                userMenu(scanner);
                return;
            }
        }
        System.out.println("Invalid username or password.");
    }

    private void userMenu(Scanner scanner) {
        while (true) {
            System.out.println("1. View Available Stocks");
            System.out.println("2. Buy Stock");
            System.out.println("3. Sell Stock");
            System.out.println("4. View Portfolio");
            System.out.println("5. Logout");
            int choice = scanner.nextInt();
            scanner.nextLine(); // Consume newline

            switch (choice) {
                case 1:
                    viewAvailableStocks();
                    break;
                case 2:
                    buyStock(scanner);
                    break;
                case 3:
                    sellStock(scanner);
                    break;
                case 4:
                    loggedInUser .getPortfolio().displayPortfolio();
                    break;
                case 5:
                    loggedInUser  = null;
                    System.out.println("Logged out successfully.");
                    return;
                default:
                    System.out.println("Invalid choice. Please try again.");
            }
        }
    }

    private void viewAvailableStocks() {
        System.out.println("Available Stocks:");
        for (Stock stock : availableStocks) {
            System.out.println(stock.getName() + ": $" + stock.getPrice());
        }
    }

    private void buyStock(Scanner scanner) {
        System.out.print("Enter stock name: ");
        String stockName = scanner.nextLine();
        System.out.print("Enter quantity: ");
        int quantity = scanner.nextInt();
        scanner.nextLine(); // Consume newline

        for (Stock stock : availableStocks) {
            if (stock.getName().equalsIgnoreCase(stockName)) {
                loggedInUser .getPortfolio().buyStock(stockName, quantity);
                System.out.println("Bought " + quantity + " shares of " + stockName);
                return;
            }
        }
        System.out.println("Stock not found.");
    }

    private void sellStock(Scanner scanner) {
        System.out.print("Enter stock name: ");
        String stockName = scanner.nextLine();
        System.out.print("Enter quantity: ");
        int quantity = scanner.nextInt();
        scanner.nextLine(); // Consume newline

        loggedInUser .getPortfolio().sellStock(stockName, quantity);
        System.out.println("Sold " + quantity + " shares of " + stockName);
    }
}
