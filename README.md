# github-final-project
def calculate_simple_interest(principal, rate_of_interest, time_period):
    try:
        # Convert rate_of_interest to a decimal (e.g., 5% will become 0.05)
        rate_of_interest = rate_of_interest / 100.0

        # Calculate simple interest
        simple_interest = principal * rate_of_interest * time_period

        return simple_interest
    except Exception as e:
        return str(e)

# Example usage:
principal_amount = float(input("Enter the principal amount: "))
annual_rate_of_interest = float(input("Enter the annual rate of interest (%): "))
time_in_years = float(input("Enter the time period in years: "))

result = calculate_simple_interest(principal_amount, annual_rate_of_interest, time_in_years)
print(f"The simple interest is: {result:.2f}")
