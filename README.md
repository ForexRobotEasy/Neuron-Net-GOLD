# Neuron Net GOLD

## Description

This code is a sample implementation of the Neuron Net GOLD trading robot, developed by Forex Robot Easy Team. The Neuron Net GOLD is an AI-powered forex software designed to make predictions for XAU/USD (Gold) trading.

For detailed reviews and trading results of this product, please visit [Forex Robot Easy - Neuron Net GOLD Review](https://forexroboteasy.com/forex-robot-review/neuron-net-gold-review-ai-powered-forex-software-for-xauusd-predictions/).

Please note that ForexRobotEasy is not the official developer of this product. We are only providing a sample code that can work as described in this product. To find the official developer of this product, please use the MQL5 platform.

## How it Works

The Neuron Net GOLD trading robot uses a trained model to predict the price movement of XAU/USD. It then opens buy or sell orders based on the predicted movement.

### Input Parameters

- `ModelPath`: The path to the trained model.
- `LotSize`: The trading lot size.
- `StopLoss`: The stop loss in points.
- `TakeProfit`: The take profit in points.
- `MaxSpread`: The maximum allowed spread in points.
- `MaxSlippage`: The maximum allowed slippage in points.

### Global Variables

- `ticket`: The order ticket.
- `prediction`: The predicted price movement.

### Initialization

The Python interpreter is initialized using the `Py_Initialize()` function.

### Deinitialization

The Python interpreter is deinitialized using the `Py_Finalize()` function.

### Predicting Price Movement

The `PredictPriceMovement()` function calculates the predicted price movement using the trained model. It imports the model, gets the predict function, and calls it with the necessary inputs. The predicted value is then converted to a double.

### Opening an Order

The `OpenOrder()` function opens a buy order if the predicted price movement is positive, and a sell order if it is negative. The order is sent using the `OrderSend()` function.

### Checking if the Order is Closed

The `IsOrderClosed()` function checks if the order is closed. It selects the order by ticket, and if the order is closed successfully, it returns `true`.

### Entry Point

The `OnTick()` function is the entry point of the trading robot. It checks the current spread and slippage, and if they are within the allowed ranges, it calculates the predicted price movement, opens an order based on the prediction, and checks if the order is closed.

## Disclaimer

Please note that this code is a sample implementation provided by Forex Robot Easy Team. It is not the official code of the Neuron Net GOLD trading robot. To find the official developer of this product and obtain the official code, please use the MQL5 platform.
