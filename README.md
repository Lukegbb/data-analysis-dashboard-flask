# Data Analysis Dashboard

A small **Flask** web application that reads data from a CSV file, processes it with **Pandas** and renders a chart with **Matplotlib** on a simple web dashboard.

## Features

- Loads and processes data from `data/dados.csv`
- Generates a bar chart of values by category every time the page loads
- Serves the chart through a clean HTML/CSS interface

## Tech stack

- Python 3, Flask
- Pandas, Matplotlib
- HTML5, CSS3

## Getting started

```bash
git clone https://github.com/Lukegbb/data-analysis-dashboard-flask.git
cd data-analysis-dashboard-flask

python3 -m venv venv
source venv/bin/activate      # Windows: venv\Scripts\activate

pip install -r requirements.txt
python app.py
```

Then open http://127.0.0.1:5000 in your browser.

## Project structure

```
├── app.py               # Flask application (data loading + chart generation)
├── templates/
│   └── index.html       # Main page
├── static/
│   ├── style.css        # Styles
│   └── images/          # Generated charts
├── data/
│   └── dados.csv        # Sample dataset (columns: categoria, valor)
└── requirements.txt
```

## Using your own data

Replace `data/dados.csv` with any CSV that has a `categoria` (category) column and a `valor` (value) column and reload the page.

## Next steps

- Upload CSV files through the web interface
- Interactive charts (Chart.js / Plotly)
- Filters and summary statistics
