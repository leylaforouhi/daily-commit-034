from datetime import datetime

def days_between(date1, date2):
    d1 = datetime.strptime(date1, "%Y-%m-%d")
    d2 = datetime.strptime(date2, "%Y-%m-%d")
    return abs((d2 - d1).days)

if __name__ == "__main__":
    print(f"Days between 2025-01-01 and today: {days_between('2025-01-01', datetime.now().strftime('%Y-%m-%d'))}")
