# WH Fair Value Gap MT5

## Developer: Forex Robot Easy
## Developer's Site: [forexroboteasy.com](https://forexroboteasy.com/forex-robot-review/wh-fair-value-gap-mt5-unbiased-review-and-real-results/)

This is the code for the WH Fair Value Gap MT5 expert advisor. This expert advisor is designed to identify fair value gaps in the Forex market and execute trades based on the identified gaps.

### Functionality

The expert advisor utilizes the MetaTrader 5 platform and requires the inclusion of the Trade and Expert libraries. The Trade library provides functionality for executing trades, while the Expert library is used to define the expert advisor class.

The expert advisor class, named CWhFairValueGapMT5, is defined and includes a private variable, m_trade, which is an instance of the CTrade class. This variable is used to execute trades.

The expert advisor class also includes several event handlers:

- OnInit: This event handler is called when the expert advisor is initialized. It performs any necessary initialization tasks.
- OnDeinit: This event handler is called when the expert advisor is deinitialized. It performs any necessary cleanup tasks.
- OnTick: This event handler is called on each tick of the Forex market. It implements the algorithm to identify fair value gaps and execute trades based on the identified gaps.

Other event handlers, such as OnTrade and OnChartEvent, can be added to the expert advisor class as needed.

### Usage

To use this expert advisor, include the necessary libraries and create an instance of the CWhFairValueGapMT5 class. The expert advisor's OnInit, OnDeinit, and OnTick event handlers should be called in the corresponding functions in the expert initialization file.

```cpp
#include <Trade\Trade.mqh>
#include <Expert\Expert.mqh>

class CWhFairValueGapMT5 : public CExpertAdvisor
{
   // ...
};

CWhFairValueGapMT5 expert;

int OnInit()
{
   expert.OnInit();
   return(INIT_SUCCEEDED);
}

void OnDeinit(const int reason)
{
   expert.OnDeinit(reason);
}

void OnTick()
{
   expert.OnTick();
}
```

Note: Forex Robot Easy is not the official developer of this product. This code is provided as a sample that can work as described in the product. To find the official developer of this product, please refer to MQL5.

For detailed reviews and trading results of this product, please visit [forexroboteasy.com](https://forexroboteasy.com/forex-robot-review/wh-fair-value-gap-mt5-unbiased-review-and-real-results/).
