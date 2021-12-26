This project is to exercise some skills in web scrapping using python.

![cafezinho](https://user-images.githubusercontent.com/66270476/147421996-e823f1a9-1bd8-473a-b3f9-8b59dd1ac5d6.jpg)


## 📚 1. Business Context

The Coffee&Cookies Books Club is a startup in the UK that wants to build a subscription-based book club for lovers of coffee and books.

Coffee&Cookies picks only hard-to-find and greatly-rated books. The company packs them with a unique reading guide and a wellness set including exotic varieties of coffee and specialty candies.

Their market research showed that the customers keeps their subscription for longer when they receive a mix of casual and business books, from the following categories:

- Classics
- Science Fiction
- Humor
- Business

Coffee&Cookies needs to decide what books to deliver next to their subscribers, and required me search for a dataset including the following info:

- Book name
- Price in GBP
- Customer Rating
- Stock availability

## 💭 2. Development Strategy

### Desired Output

The customer asked for the raw information as it will be used later for further analysis.

- ***.csv file with the information**

A table will be created containing the following information:

| Columns | Description |
| --- | --- |
| scrap_date | the date the scrapping was held |
| upc | a unique identifier for each title |
| book_name | the title of the book |
| book_category | the book's category page |
| book_price | price excl. tax |
| book_rating | from 1 to 5 |
| book_stock_availability | quantity available |

### 🛠Process

Tools used:

- Jupyter Notebook
- Python 3.9
- BeautifulSoup4
- Pandas
- Requests

**STEP 01:**  use a browser to understand the tags structure for the website, and find where the data we need is embedded within the code.

**STEP 02:** scrap the catalogue pages to get a dataset of titles available with their respective categories.

**STEP 03:** use the list of titles created in step 02 to access the books pages to scrap for the remaining information needed.

**STEP 04: join** the tables on step 02 and step 03, using the title of the books as a key.

**STEP 05:** export the data to *.csv and deliver it to Coffee&Cookies.

### ⏩ Inputs

I will use [https://books.toscrape.com](https://books.toscrape.com) as a source for the data. It is a website made for scrapping and can be used free of charge.
