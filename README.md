# 📊 GitHub Trending Repositories Scraper

A simple Python script to scrape the top trending repositories from GitHub based on a specified programming language and number of results.

---

## 🌐 Description

This project performs **web scraping** on GitHub to collect the most starred repositories for a specific language (e.g., Python, JavaScript). It saves the output to a local `.txt` file.

> ⚠️ Note: Direct HTML scraping may break if GitHub's layout changes. Consider using the [GitHub REST API](https://docs.github.com/en/rest).

---

## 🧰 Technologies Used

- `requests`
- `json`
- `pprint`

---

## 🏁 Getting Started

### 🔧 Prerequisites

- Python 3.7+
- `requests` module (install with pip if needed)

### ▶️ How to Run

```bash
python gwscr.py
```

You will be prompted to enter:

- Programming language (e.g., Python)

- Number of repositories to fetch

---

## 📂 Output
Results will be saved in a file named like:

```
trending_python_repositories.txt
```
Each entry contains:

- Repository name

- Description

- Direct URL to the repo

---

##🚀 Example GitHub API Usage
Replace the URL with this if you want to use GitHub API:

```
url = f"https://api.github.com/search/repositories?q=language:{language}&sort=stars&order=desc&per_page=100&page={page}"
And then parse response.json()['items'].
```

---

## 🧑‍💻 Author
Bardia Javadi
Data Science Enthusiast | Python Developer
GitHub: @bardiw
