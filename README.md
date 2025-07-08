# Tagsifier
Tagsifier is a Python tool designed to classify web pages into categories based on their HTML tags and structure. By analyzing the DOM elements, Tagsifier groups pages with similar layouts, making it easier to identify templates, detect page types, or cluster websites with alike structures. This can be useful for web scraping, site audits, SEO analysis, or automated website categorization.

## Install
### 1) Clone the repository
`git clone https://github.com/your-username/tagsifier.git
cd tagsifier`

### 2) Install the required Python packages
`pip install openpyxl numpy scikit-learn sklearn bs4`

### 3) Prepare Input URL list
Tagsifier reads input URLs from an Excel file Prepare an Excel file named Input.xlsx in the same directory as the script. URLs must be listed in the first column (column A). The script will process the URLs from a specified row range set by user. A sample Input file is located in the repository.

### 4) Start Classifying
Run the command below to start webpage classifying. '--clusters' is the	Number of structural clusters, --row-start	is starting Excel row, and --row-end	is ending excel row.

`python tagsifier.py --clusters 5 --row-start 2 --row-end 100`

