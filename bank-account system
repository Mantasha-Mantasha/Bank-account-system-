class BankAccount:
    def __init__(self, account_number, holder_name, balance=0):
        self.account_number = account_number
        self.holder_name = holder_name
        self.balance = balance

    def deposit(self, amount):
        if amount > 0:
            self.balance += amount
            print(f"Deposited {amount} successfully. New balance: {self.balance}")
        else:
            print("Deposit amount must be greater than zero.")

    def withdraw(self, amount):
        if amount <= 0:
            print("Withdrawal amount must be greater than zero.")
        elif amount > self.balance:
            print("Insufficient balance for this withdrawal.")
        else:
            self.balance -= amount
            print(f"Withdrawn {amount} successfully. Remaining balance: {self.balance}")

    def check_balance(self):
        print(f"Account balance: {self.balance}")

# Example usage
if __name__ == "__main__":
    account = BankAccount("123456789", "Alice", 500)

    # Check initial balance
    account.check_balance()

    # Deposit money
    account.deposit(200)

    # Attempt to withdraw more than balance
    account.withdraw(800)

    # Withdraw money
    account.withdraw(300)

    # Check balance after transactions
    account.check_balance()
