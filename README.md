# 🌎 GMapExtractor: Advanced Local SEO Analysis Tool

[![Python](https://img.shields.io/badge/Python-3.7+-blue.svg)](https://www.python.org/downloads/)
[![aiohttp](https://img.shields.io/badge/aiohttp-Latest-green.svg)](https://docs.aiohttp.org/)
[![pandas](https://img.shields.io/badge/pandas-Latest-yellow.svg)](https://pandas.pydata.org/)
[![SerpAPI](https://img.shields.io/badge/SerpAPI-Latest-red.svg)](https://serpapi.com/)

## 🚀 About GMapExtractor

GMapExtractor is a powerful, asynchronous tool for SEO professionals and local business analysts to extract, analyze, and compare Google Maps and organic search rankings. With support for multiple queries across various locations, this tool provides comprehensive data for local SEO campaigns and competitive analysis.

## ✨ Key Features

- **Asynchronous Processing**: Extract data from multiple queries simultaneously
- **Dual Analysis Mode**: Get both Google Maps listings and organic search results
- **Custom Filtering**: Identify truly local businesses with exception list support
- **Advanced Metrics**: Track reviews, ratings, and local relevance
- **CSV Export**: Clean, formatted data ready for analysis or import to other tools

## 🛠️ Tech Stack

- **Python** 🐍
- `asyncio`, `aiohttp`
- `pandas`
- `SerpApi`
- `re` (Regex), `urllib`

## 🛠️ How It Works

1. Enter your desired number of search results
2. Specify target cities, states, and search queries
3. Let GMapExtractor asynchronously gather data from both Google Maps and organic search results
4. Receive neatly formatted CSV files with all the data you need for analysis

## 📊 Data Points Collected

### Google Maps Results:
- Business name, address, and phone
- Website and domain
- Rating and review count
- Business location (city/state)
- Local business identification

### Organic Search Results:
- Ranking position
- Business domain and name
- Page title
- URL
- Search query details

## 🚦 Getting Started

1. Clone this repository to your local machine:
    ```sh
    git clone https://github.com/yourusername/google-maps-data-extractor.git
    ```

2. Install the required dependencies using pip:

    ```sh
    pip install -r requirements.txt
    ```
3. **Set Up Your SerpApi Key**

   - Get an API key from [SerpApi](https://serpapi.com/)
   - Replace `YOUR SerpApi GOOGLE search API KEY` in `GMapExtractor.py` with your actual key.

4. **Create an Exception List (Optional)**

   - Add domain names to exclude in `ExceptionList.txt` (one per line).

## 📝 Example Usage

```python
# Example queries
cities = "Seattle,Portland,Denver"
states = "WA,OR,CO"
queries = "coffee shop,bakery,coffee roaster"
limit = 20

# Run the extraction
asyncio.run(main(cities, states, queries, limit))
```

## 💡 Use Cases

- **Local SEO Campaigns**: Identify top-ranking local businesses in your niche
- **Competitor Analysis**: Track your competitors' rankings across multiple locations
- **Market Research**: Discover business trends across different cities and states
- **Client Reporting**: Generate comprehensive ranking reports for clients

## 🔍 Advanced Tips

- Use the exception list to filter out national chains and focus on truly local businesses
- Run weekly or monthly to track ranking changes over time
- Compare results across different geographic locations to spot regional trends

