Hi 👋, I'm Md Imran Nazir Udoy
🚀 Web Developer | 📊 Data Science Learner | 🎮 Gamer | 📹 Video Editor | 📈 Competitive Programmer

🧠 About Me

🔭 I’m currently working on Full Stack Web Development
🌱 I’m currently learning Data Science and Competitive Programming
👯 I’m looking to collaborate on Open Source Projects
📫 Reach me: udoyofficial@gmail.com
💬 Ask me about React, Node.js, Express, C++, Python, Editing, Motion Graphics


🔗 Connect with Me


📈 GitHub Stats


📊 Contribution Activity
Toggle Contribution Views

  Weekly (Default)
  ![Udoy's Weekly GitHub Activity Graph](https://github-readme-activity-graph.vercel.app/graph?username=udoydev&theme=react-dark&area=true&hide_border=true)



  Daily (May 1 - May 11, 2025)
  ![Udoy's Daily GitHub Activity Graph](https://github-readme-activity-graph.vercel.app/graph?username=udoydev&from=2025-05-01&to=2025-05-11&theme=dracula&area=true&hide_border=true)



  Monthly (May 1 - May 31, 2025)
  ![Udoy's Monthly GitHub Activity Graph](https://github-readme-activity-graph.vercel.app/graph?username=udoydev&from=2025-05-01&to=2025-05-31&theme=merko&area=true&hide_border=true)



  Yearly (Jan 1 - Dec 31, 2024)
  ![Udoy's Yearly GitHub Activity Graph](https://github-readme-activity-graph.vercel.app/graph?username=udoydev&from=2024-01-01&to=2024-12-31&theme=rogue&area=true&hide_border=true)



💻 Sample Code
Here’s a Python script to fetch and visualize your GitHub contribution data using the GitHub API:
import requests
import matplotlib.pyplot as plt

# Replace with your GitHub username and a personal access token
username = "udoydev"
token = "your_personal_access_token"  # Generate from GitHub settings

# GitHub API endpoint for contributions
url = f"https://api.github.com/users/{username}/events"
headers = {"Authorization": f"token {token}"}

# Fetch data
response = requests.get(url, headers=headers)
events = response.json()

# Count contributions (simplified example)
contributions = {}
for event in events:
    date = event['created_at'][:10]  # Get date (YYYY-MM-DD)
    contributions[date] = contributions.get(date, 0) + 1

# Plot
dates = list(contributions.keys())
counts = list(contributions.values())
plt.bar(dates, counts)
plt.xlabel("Date")
plt.ylabel("Contributions")
plt.title("Udoy's GitHub Contributions")
plt.xticks(rotation=45)
plt.tight_layout()
plt.show()

Note: You need a GitHub personal access token with repo scope. Install matplotlib (pip install matplotlib) to run this. This is a basic example—expand it for weekly/monthly/yearly views.

🧠 Motivation Tip (Updated Daily by Mentor)

“Discipline is choosing between what you want now and what you want most.”👉 Stay consistent. Keep learning. Earn your transformation.

