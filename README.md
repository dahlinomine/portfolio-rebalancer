# Portfolio Rebalancer

![finance](https://img.shields.io/badge/finance-blue?style=flat-square) ![trading](https://img.shields.io/badge/trading-blue?style=flat-square) ![automation](https://img.shields.io/badge/automation-blue?style=flat-square)

Autonomous agent that executes trades to maintain a target asset allocation.

## Overview
Portfolio Rebalancer is a Python-based automated trading agent designed to eliminate the manual overhead of wealth management. It monitors your current holdings in real-time and automatically executes buy/sell orders whenever your portfolio drifts from its predefined target percentages. By automating the rebalancing process, it ensures consistent risk management and disciplined adherence to your long-term investment strategy.

## Features
*   **Automated Drift Detection:** Continuously monitors asset fluctuations and identifies deviations from target weights.
*   **Precision Execution:** Calculates exact share quantities required to return to the target allocation.
*   **Custom Thresholds:** Set "drift buffers" to prevent over-trading and minimize transaction costs.
*   **Multi-Asset Support:** Manage a diverse mix of equities, ETFs, and other assets supported by your connected brokerage.

## Installation
Ensure you have Python 3.8+ installed. Clone the repository and install the necessary dependencies:

```bash
git clone https://github.com/yourusername/portfolio-rebalancer.git
cd portfolio-rebalancer
pip install -r requirements.txt
```

## Usage
Configure your target allocation in the `config.yaml` file (or via environment variables), then run the agent:

```bash
python main.py
```

**Example:**
If your target is 60% VTI and 40% BND, but VTI rises to 65%, the agent will automatically calculate and execute the sell order for VTI and the buy order for BND to restore the 60/40 balance.

## Contributing
Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change. Ensure that your code adheres to PEP 8 standards and includes appropriate tests.

## License
This project is licensed under the [MIT License](LICENSE).