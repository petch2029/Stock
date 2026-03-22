<!DOCTYPE html>

<html>
<head>
  <title>Petch Stock Website</title>
</head>
<body style="background:black; color:white; font-family:sans-serif;">

  <h1>📊 My Stock Dashboard</h1>

  <!-- TradingView Chart -->

  <div id="chart"></div>
  <script src="https://s3.tradingview.com/tv.js"></script>
  <script>
    new TradingView.widget({
      "container_id": "chart",
      "width": "100%",
      "height": 500,
      "symbol": "NASDAQ:AAPL",
      "interval": "1",
      "theme": "dark",
      "style": "1",
      "watchlist": [
        "NASDAQ:AAPL",
        "NASDAQ:NVDA",
        "NASDAQ:TSLA",
        "NASDAQ:ASML",
        "NYSE:TSM",
        "NASDAQ:RKLB",
        "NYSE:OKLO",
        "AMEX:SPY",
        "OANDA:XAUUSD",
        "BINANCE:BTCUSDT"
      ]
    });
  </script>

  <h2>📰 Market News</h2>

  <!-- News Widget -->

  <div class="tradingview-widget-container">
    <script src="https://s3.tradingview.com/external-embedding/embed-widget-timeline.js" async>
    {
      "feedMode": "market",
      "colorTheme": "dark",
      "width": "100%",
      "height": 600
    }
    </script>
  </div>

</body>
</html>
