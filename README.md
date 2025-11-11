# Simple-Python
# main_script.py

import time
import datetime

def perform_task():
    """Simulates performing a scheduled task."""
    current_time = datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
    print(f"Task executed at: {current_time} - Status: OK")

def main():
    """Main loop for the simple task scheduler."""
    print("Starting Simple Task Scheduler...")
    try:
        while True:
            perform_task()
            # Wait for 5 seconds before the next task execution
            time.sleep(5)
    except KeyboardInterrupt:
        print("\nScheduler stopped manually.")

if __name__ == "__main__":
    main()
