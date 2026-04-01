import random

def get_heart_rate():
    # Simulate heart rate (beats per minute)
    return random.randint(50, 120)

def analyze_heart_rate(hr):
    if hr < 60:
        return "Low Heart Rate"
    elif 60 <= hr <= 100:
        return "Normal Heart Rate"
    else:
        return "High Heart Rate"

def main():
    heart_rate = get_heart_rate()
    status = analyze_heart_rate(heart_rate)

    print("=== Biometric Health Monitor ===")
    print(f"Heart Rate: {heart_rate} BPM")
    print(f"Status: {status}")

if __name__ == "__main__":
    main()