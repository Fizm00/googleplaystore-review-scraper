# Google Play Store Review Scraper - Tokopedia

![Tokopedia Logo](tokopedia-seeklogo.png)

## 📱 Project Description

This project is a Python script designed to collect and analyze user reviews from the Tokopedia app on the Google Play Store. The scraper fetches recent reviews along with key information such as rating, username, review content, and posting time, and presents them in a structured dataset with insightful visualizations.

## ✨ Features

- Retrieves up to 25,000 latest reviews (configurable)
- Saves complete data in CSV format
- Visualizes rating distribution with a histogram
- Analyzes monthly rating trends using line charts
- Includes a progress bar to monitor scraping status
- Supports language and country configuration

## 🛠️ Installation & Usage

### Prerequisites

Ensure Python (version 3.6 or higher) is installed on your system. (In this project, we use Python 3.12.7)

### Step 1: Clone the Repository

```bash
git clone https://github.com/username/tokopedia-review-scraper.git
cd tokopedia-review-scraper
```

### Step 2: Install Required Libraries

```bash
pip install -r requirements.txt
```

### Step 3: Run the Script

```bash
python tokopedia_review_scraper.py
```

## 📊 Output

This script generates the following output:

1. `tokopedia_reviews_full.csv` - Complete dataset from scraping
2. `tokopedia_ratings_distribution.png` - Rating distribution visualization
3. `tokopedia_monthly_ratings.png` - Monthly rating trend chart

## 📋 Data Structure

The scraped dataset contains the following columns:

| Column | Description |
|-------|-----------|
| reviewId | Unique review ID |
| userName | Name of the user who wrote the review |
| content | Review content |
| score | Rating (1-5) |
| thumbsUpCount | Number of likes/thumbs up on the review |
| reviewCreatedVersion | App version when the review was made |
| at | Timestamp when the review was posted |
| appVersion | Current version of the app |

## 🔧 Configuration

You can modify several parameters in the code:

```python
# Configuration
output_folder = r"D:\Code\Data Mining\Kuliah Data Mining\Praktikum10"  # Change to your desired folder path
app_id = "com.tokopedia.tkpd"  # App ID on Play Store
reviews_count = 25000          # Number of reviews to fetch
```

## ⚠️ Limitations

- Google Play Store rate limiting may affect scraping speed
- Scraping large amounts of data may take time
- Ensure compliance with the Google Play Store Terms of Service

## 📚 References

- [Google Play Scraper Documentation](https://github.com/JoMingyu/google-play-scraper)
- [Pandas Documentation](https://pandas.pydata.org/docs/)
- [Matplotlib Documentation](https://matplotlib.org/stable/contents.html)

## 📄 Lisensi

This project is licensed under the [MIT License](LICENSE)

---

*Created for academic purposes as part of a Data Mining course*
