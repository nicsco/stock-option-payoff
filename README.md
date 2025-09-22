# **Options Payoff Visualiser**

A single-page, interactive web tool for visualising the profit and loss (P/L) payoff diagrams of complex stock option strategies. This tool allows you to combine multiple option legs (long/short calls and puts) to see the net payoff profile at expiration.

The entire application is contained in a single `interactive_chart.html` file, uses no build tools, and is powered by D3.js and Tailwind CSS.

## **Features**

* **Combined Strategy Plotting:** See the net profit/loss diagram for multiple options combined, not just single legs.  
* **Full Option Support:** Add Long Calls, Long Puts, Short Calls, and Short Puts.  
* **Dynamic UI:** Add or remove unlimited option legs to build any strategy (spreads, straddles, condors, etc.).  
* **Rich Visuals:**  
  * Profit/Loss line is coloured **green for profit** and **red for loss**.  
  * The entire profit area is shaded with a light green background.  
  * **Strike Price Markers:** Clearly see where each leg's strike price is on the chart.  
  * **Stacked Labels:** Markers (`+c`, `-p`, etc.) stack vertically to prevent overlap on shared strikes.  
* **Interactive Chart Range:** Set the minimum and maximum stock price to view on the x-axis.  
* **Shareable Strategies:** The entire state of your strategy (range and all legs) is encoded in the URL. Just copy and paste the URL to share your exact model with others\!

## **How to Use**

1. **Open:** Simply open the `interactive_chart.html` file in any modern web browser.  
2. **Set Range:** Adjust the "Stock Price Min" and "Stock Price Max" to define the x-axis of the chart.  
3. **Build Strategy:**  
   * Use the "Operations (Legs)" section to build your strategy.  
   * Select the option `Type`, set its `Strike` price, and enter the `Premium` (cost).  
   * Click **"Add Option"** to add more legs.  
   * Click the **"X"** icon on any leg to remove it.  
4. **View Chart:** The chart updates instantly with every change you make.  
5. **Share:** Once your strategy is built, copy the full URL from your browser's address bar to save or share it.

## **Technologies Used**

* **HTML5**  
* **Tailwind CSS** (loaded via CDN for styling)  
* **D3.js (v7)** (loaded via CDN for all charting)  
* **Vanilla JavaScript (ES6+)** (for all application logic)

## **License**

This project is licensed under the MIT License. See the `LICENSE` file for details (or feel free to add one).
