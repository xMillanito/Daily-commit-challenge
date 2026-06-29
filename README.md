from datetime import datetime

class ActivityTracker:
    def init(self):
        self.created_at = datetime.now()

    def status(self):
        return {
            "project": "GitHub Activity",
            "status": "Active",
            "last_update": self.created_at.strftime("%Y-%m-%d %H:%M:%S")
        }

def main():
    tracker = ActivityTracker()

    for key, value in tracker.status().items():
        print(f"{23}: {value}")

if name == "main":
    main()
