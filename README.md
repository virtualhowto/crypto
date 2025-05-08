🎰 Bitcoin Mining vs Powerball 🎯

An interactive, web-based calculator that compares your Bitcoin solo mining odds to winning the Powerball — and tells you when you'll break even on your mining rig 💸



⚡ Features

🔢 Compare solo mining chances vs. Powerball odds

📈 Live profit and breakeven calculations

💰 Estimate power usage and miner hardware costs

📊 Dynamic Chart.js graph of monthly ROI

🚀 Presets for common miners (Bitaxe Gamma & Antminer S17+)

🌞 Perfect for solar mining and hobbyists!

🧮 How It Works

Just plug in:

Your miner’s hashrate (TH/s)

Power consumption (Watts)

Electricity cost (AUD per kWh)

Average hours per day mining

Number of miners

Upfront cost per miner

It calculates your:

🎯 Chance of solo mining a block per day

💸 Daily, monthly & yearly income and costs

📉 Powerball odds comparison

🧾 Total hardware cost

📈 Monthly cumulative profit and breakeven chart

📦 How to Use

🔗 Live Demo (GitHub Pages)

Or run locally:

git clone https://github.com/yourusername/bitcoin-vs-powerball.git
cd bitcoin-vs-powerball
open index.html

🧠 Tech Stack

HTML5 + CSS3

JavaScript (vanilla)

Chart.js for profit graph

Google Fonts: Orbitron & Roboto

Fully responsive + mobile-ready

🔧 Customization

To add new miner presets:

Edit the setPreset() function in index.html:

else if (model === 'yourNewMiner') {
  document.getElementById('hashrate').value = XX;
  document.getElementById('miners').value = X;
  document.getElementById('power').value = XXXX;
  document.getElementById('unitCost').value = XXXX;
}

🤝 Credits

Miner specs: asicminervalue.com

Logo: GitHub Avatar

💡 This tool was built out of curiosity... because honestly, mining might just beat the lottery 🎯# crypto
