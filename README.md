# 📊 SEC 8-K Product Announcement Extractor

This project analyzes U.S. SEC Form 8-K filings using local large language models (LLMs) via the Ollama API to extract new product and service announcements.

## 🔍 What It Does

- Retrieves 8-K filings from the SEC EDGAR system (using CIK + ticker)
- Extracts filing text and feeds it to an LLM (e.g., `mistral`, `deepseek-coder`)
- Extracts:
  - `company_name`
  - `stock_name`
  - `filing_time`
  - `new_product`
  - `product_description`
- Saves output to `8k_product_releases.csv`

## 📁 Files Included

- `LLM_Doc_V2.ipynb`: Full implementation in Jupyter Notebook
- `8k_product_releases.csv`: Structured CSV with extracted products
- `report`: Brief summary of methodology

## 🧠 Technologies Used

- Python, Pandas, BeautifulSoup
- SEC EDGAR Atom Feed
- Ollama (LLM runner)
- Local LLM models (`mistral`, etc.)

## 📎 Author

Chandler Davis  
GitHub: [@ChandlerD1025](https://github.com/ChandlerD1025)
