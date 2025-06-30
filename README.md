# 1. Install packages
pip install yfinance alpha_vantage

# 2. Load historical OHLCV (1𝑦 data)
import yfinance as yf
price_df = yf.download(["AAPL","MSFT","GOOGL"], start="2020-01-01")

# 3. Load intraday data via Alpha Vantage
from alpha_vantage.timeseries import TimeSeries
ts = TimeSeries(key="YOUR_KEY", output_format="pandas")
intraday_df, _ = ts.get_intraday(symbol="AAPL", interval="15min", outputsize="compact")
📈 Daily OHLCV for feature engineering and backtesting

⏱️ Intraday sampling for high-frequency signal detection
 
 
 
 Hybrid Classical-Quantum Architecture

Classical ML for feature engineering and return prediction
Quantum algorithms (QAOA) for combinatorial optimization
Seamless integration between both approaches

2. Advanced QUBO Formulations

Transaction costs integration
Cardinality constraints (limit number of assets)
Sector diversification rules
Multiple risk metrics support

3. Quantum Feature Encoding

Uses QuantumKernel with ZZ and Pauli feature maps
Transforms classical market data into quantum states
Enhanced representation learning for better pattern discovery

4. Quantum-Enhanced Clustering

Groups similar assets for improved diversification
Uses quantum kernels for non-linear similarity detection
Reduces correlation risk in portfolio construction

5. Comprehensive Performance Metrics

Sharpe Ratio, Sortino Ratio, Maximum Drawdown
Information Ratio and downside risk measures
Comparative analysis between quantum and classical approaches
