# crypto-wallet
A Python-based cryptocurrency wallet tracker with multi-chain support.
# Crypto Wallet Tracker 🪙  

A simple Python application to track balances from multiple cryptocurrency wallets and exchanges.  

## Features  
- Multi-chain support: Bitcoin, Ethereum, Binance Smart Chain.  
- Fetch live data from Binance API.  
- Track historical portfolio value.  

## Installation  
1. Clone the repository:  
   ```bash
   git clone https://github.com/your-username/crypto-wallet.git
   pip install -r requirements.txt
   python main.py

   ---

### **3. Добавление кода в репозиторий**  

#### Шаг 3.1: Инициализация локального проекта  
1. На вашем компьютере:  
   - Установите **Git** и **Python**.  
   - В терминале выполните:  
     ```bash
     git clone https://github.com/your-username/crypto-wallet.git  
     cd crypto-wallet  
     ```  

#### Шаг 3.2: Добавьте код для криптопроекта  
Пример: Мини-кошелек на Python.  
1. Создайте файл `main.py`:  
   ```python
   import requests  

   def get_bitcoin_price():  
       response = requests.get("https://api.coindesk.com/v1/bpi/currentprice/BTC.json")  
       data = response.json()  
       return data['bpi']['USD']['rate']  

   print(f"Current Bitcoin Price: ${get_bitcoin_price()}")  
