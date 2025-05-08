## ✅ Test Plan

### 📋 Objective
To ensure the web application accurately calculates and displays:
- Solo mining odds vs Powerball odds
- Block reward profitability
- Power cost and ROI
- Monthly and yearly profits
- Breakeven chart based on input

### 🧪 Test Categories

#### 1. Functionality Tests
| Test Case | Description | Expected Outcome |
|-----------|-------------|------------------|
| TC1 | Load the app in Chrome, Firefox, and mobile browser | Page loads without errors |
| TC2 | Click `Bitaxe Gamma` preset | Form inputs populate with 1.7 TH/s, 5W, $100 |
| TC3 | Click `Antminer S17+` preset | Inputs set to 73 TH/s, 2920W, $1000 |
| TC4 | Enter custom values and click `Run the Numbers` | All result fields are populated |
| TC5 | Clear a required input and run | No crash, calculations skip or prompt gracefully |

#### 2. Calculation Accuracy
| Test Case | Description | Expected Result |
|-----------|-------------|------------------|
| TC6 | Use 1 miner, 1 TH/s, 24h/day | Solo odds match expected ratio: 600M TH/s network |
| TC7 | Use Bitaxe preset | Odds ≈ 1 in 3.6 million, power cost ~$0.75/year |
| TC8 | Use S17+ preset | Odds ≈ 1 in 84,000, power cost ~$319/year |
| TC9 | Adjust power rate to $0.50/kWh | Power cost reflects increased rate |
| TC10 | Input 0 hours/day | $0 cost and $0 income shown |
| TC11 | Yearly Profit = Yearly Income - Power Cost |
| TC12 | Breakeven shown when profit exceeds hardware cost |

#### 3. Graph Validation
| Test Case | Description | Expected Result |
|-----------|-------------|------------------|
| TC13 | Submit values and check graph | Chart renders 12-month profit line |
| TC14 | Profit crosses 0 around breakeven month | X-axis intersection reflects breakeven point |

#### 4. Visual & UX
| Test Case | Description | Expected Result |
|-----------|-------------|------------------|
| TC15 | App loads on mobile | Layout adapts, readable inputs |
| TC16 | Hover over presets | Tooltips show miner specs |
| TC17 | Logo renders and looks circular |
| TC18 | Fonts and colors match design spec |
| TC19 | Dark background with light font accessible |

### 🧠 Edge Cases & Errors
- Large inputs (e.g. 10,000 miners)
- Power rate = 0
- Extremely high or low hashrates
- Empty fields

### 🛠 Tools
- Chrome DevTools
- BrowserStack
- Calculator for validation
- JS console for error tracking

## 📜 License
MIT — free to use, modify, and share with credit.
