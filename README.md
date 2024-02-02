# fuzzy-octo-engine
My resolutions are bank amount withdrawal jdbc, everytime we withdraw amount it has to update the bank balance


import java.sql.Connection;
import java.sql.DriverManager;
import java.sql.PreparedStatement;
import java.sql.SQLException;

public class BankWithdrawalProgram {
    private static final String JDBC_URL = "jdbc:mysql://localhost:3306/your_database";
    private static final String USERNAME = "your_username";
    private static final String PASSWORD = "your_password";

    public static void main(String[] args) {
        int accountNumber = 123456; // replace with actual account number
        double withdrawalAmount = 50.0; // replace with actual withdrawal amount

        try (Connection connection = DriverManager.getConnection(JDBC_URL, USERNAME, PASSWORD)) {
            // Update the balance in the database
            updateBalance(connection, accountNum…
