# Bitcoin Trader Sentiment Analysis 📊

This project studies how Bitcoin trader performance changes with **market sentiment (Fear vs Greed)**.  
We combine the **Fear & Greed Index** with historical trader data to measure profit, win rate, trading activity, and the best times/days to trade.

---

## 📂 Project Structure

├── data/
│ ├── fear_greed_index.csv # daily sentiment data
│ └── historical_trader_data.csv # raw trader records
├── notebooks/
│ └── Data_Science_Task.ipynb # main Colab notebook
├── outputs/
│ ├── merged_trading_data.csv # trades + sentiment
│ ├── sentiment_summary.csv # avg profit, win rate
│ ├── top_traders.csv # top 10 traders
│ ├── sentiment_analysis_overview.png # charts: profit, win rate, activity, hours
│ └── detailed_analysis.png # charts: top traders, weekdays
├── requirements.txt
└── README.md


---

## 📊 Datasets
1. **fear_greed_index.csv**  
   - Columns: `timestamp, value, classification (Fear/Greed/etc), date (yyyy-mm-dd)`
2. **historical_trader_data.csv**  
   - Columns:  
     `Account, Coin, Execution Price, Size Tokens, Size USD, Side, Timestamp IST, Start Position, Direction, Closed PnL, Transaction Hash, Order ID, Crossed, Fee, Trade ID, Timestamp`

---

## ⚙️ Setup & Run

### Run in Google Colab
1. Open `notebooks/Data_Science_Task.ipynb` in **Google Colab**.  
2. Upload the two CSVs into the Colab environment or mount Google Drive.  
3. Run all cells → outputs will be saved in `outputs/`.  

### Run locally
```bash
git clone https://github.com/<your-username>/<repo>.git
cd <repo>
pip install -r requirements.txt
jupyter notebook

Open `Data_Science_Task.ipynb` and run the cells.

---

## 📦 Requirements

```
pandas
numpy
matplotlib
seaborn
gradio
nbformat
```

Install with:

```bash
pip install -r requirements.txt
```

---

## 📈 Key Outputs

* **sentiment_analysis_overview.png** → 4 main charts:

  * Profit in Fear vs Greed
  * Win rates
  * Trading activity
  * Best trading hours
* **detailed_analysis.png** →

  * Top 10 traders
  * Best weekdays
* **sentiment_summary.csv** → stats for Fear vs Greed
* **top_traders.csv** → top performing accounts
* **merged_trading_data.csv** → cleaned dataset with sentiment merged

---

## 🔑 Key Questions Answered

* Do traders make more money during **Fear or Greed**?
* What’s the **win rate** in each condition?
* Who are the **best traders**?
* When is the **best time to trade** (hour & day)?

---

## 🚀 Insights

* Traders earned **more on Greed days** (higher avg profit & win rate).
* **More trades** happened on Fear days, but they were less profitable.
* Certain **hours and weekdays** had better profit chances.
* A few traders consistently performed better — showing stronger skill.

---

## 📌 Recommendations

* Focus trading on **Greed days** for higher profit potential.
* Avoid overtrading in Fear conditions.
* Watch for **best hours & weekdays** to optimize timing.
* Study strategies of **top-performing traders**.

---

## 📜 License

This project is released under the [MIT License](LICENSE).

---

✍️ Author: *[Akanksha Sawant]*

```
