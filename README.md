# python-technicial-indicators
A Python library for calculating popular technical indicators for financial data, enabling traders and analysts to quickly implement technical analysis strategies. Modified by QuantRelay. This software includes code from pandas-ta (Copyright (c) 2020 pandas-ta) licensed under the MIT License.
Original repo: https://github.com/Data-Analisis/Technical-Analysis-Indicators---Pandas?tab=coc-ov-file


## To use QuantRelay_ta
Install it via python pip
```bash
pip install quantrelay_ta
```


## Key Features

- **Wide Range of Indicators**: Calculate moving averages, oscillators, trend indicators, and more.
- **pandas Integration**: Works seamlessly with `pandas` DataFrames and Series.
- **Ease of Use**: Intuitive and flexible API for quick implementation.

## example

```python
import pandas as pd
import numpy as np
import quantrelay_ta as ta

# Create sample data with a 'close' column containing 10 random values
np.random.seed(42)
data = {
    'close': np.random.randint(100, 150, 10)  # Random closing prices
}
df = pd.DataFrame(data)

# Calculate a 3-period Simple Moving Average (SMA)
sma = ta.sma(close=df['close'], length=3)

# Display the original data and the SMA results
print("Original Data:")
print(df)
print("\nSimple Moving Average (3-period):")
print(sma)
```

## Documentation

Visit the [documentation](#) for more details about the available indicators and their usage.

## License

This project is licensed under the [MIT License](LICENSE).

