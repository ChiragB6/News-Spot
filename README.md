# News-Spot
NewsSpot is a web application that provides users with the latest news articles and videos from top Indian news channels. It allows users to search for news on specific topics, view related videos ranked by popularity (views), and summarize articles for quick insights.

Features
Search News: Search for the latest news articles and videos by entering a keyword.
Top Articles: Displays the top 5 news articles related to the search query, along with the source and a "Summarize" button.
Article Summarization: Summarize news articles to get concise insights into the content.
Top Videos: Displays the top 5 YouTube videos related to the search query, ranked by views, from prominent Indian news channels.
Responsive Design: Articles and videos are displayed side by side for better usability.
Technologies Used
Backend
Flask: Python web framework for handling API requests and responses.
Newspaper3k: For fetching and parsing article content.
nltk: Natural Language Toolkit for text processing and summarization.
scikit-learn: Used for TF-IDF vectorization in the summarization process.
YouTube Data API v3: Fetches videos and statistics (views, likes) from YouTube.
News API: Fetches news articles from multiple sources.
Frontend
HTML5: Structure of the web application.
CSS3: Styling and layout.
JavaScript: For dynamic content updates and API integration.
Setup Instructions
Prerequisites
Python 3.7 or higher
Flask (pip install flask)
Newspaper3k (pip install newspaper3k)
NLTK (pip install nltk)
scikit-learn (pip install scikit-learn)
API keys for:
YouTube Data API v3
News API
Installation
Clone the repository:

bash
Copy code
git clone https://github.com/your-username/NewsSpot.git
cd NewsSpot
Install dependencies:

bash
Copy code
pip install -r requirements.txt
Set up API keys:

Replace YOUTUBE_API_KEY and NEWS_API_KEY in app.py with your own API keys.
Download NLTK data:

bash
Copy code
python
>>> import nltk
>>> nltk.download('punkt')
>>> exit()
Run the application:

bash
Copy code
python app.py
Open your browser and navigate to:

arduino
Copy code
http://127.0.0.1:5000
Project Structure
php
Copy code
NewsSpot/
├── app.py                # Backend code for Flask server
├── templates/
│   └── index.html        # Frontend HTML file
├── static/
│   ├── css/              # (Optional) CSS styles
│   ├── js/               # (Optional) JavaScript files
├── README.md             # Project documentation
├── requirements.txt      # List of dependencies
API Details
News API
Endpoint: https://newsapi.org/v2/everything
Usage: Fetches news articles based on a search query.
YouTube Data API
Endpoint: https://www.googleapis.com/youtube/v3
Usage: Fetches videos from specified Indian news channels, ranked by views.
How It Works
Search: Enter a keyword in the search bar and press "Enter."
Articles: The app fetches the top 5 articles from trusted Indian news sources.
Videos: Simultaneously, it fetches the top 5 videos from Indian news channels, sorted by views.
Summarize: Click the "Summarize" button under any article to generate a concise summary of the content.
Channels Included
The application fetches videos from the following Indian news channels:

NDTV
Aaj Tak
India Today
ABP News
Zee News
Future Enhancements
Add more regional and local news channels.
Enable user authentication for personalized news preferences.
Include a "Save Article" or "Bookmark Video" feature.
Add multilingual support for regional languages.
