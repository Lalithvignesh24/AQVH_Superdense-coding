# ✈️ Superdense Quantum Communication for Secure Aircraft Alerting

A quantum communication project demonstrating **Superdense Coding (SDC)** and **Quantum Key Distribution (QKD)** applied to a real-world defense-inspired use case:

> 🚨 Alerting a fighter aircraft when it is entering a restricted airspace using quantum-secured communication.

This project proves that **2 classical bits can be transmitted using only 1 qubit** via entanglement and integrates aircraft path prediction with quantum communication.

---

## 🧠 Project Objective

- Demonstrate Superdense Coding (2 classical bits via 1 qubit)
- Implement entanglement-based QKD concepts by E91 protocol
- Apply quantum communication to aircraft restricted-zone alerting
- Execute circuits on:
  - Local Qiskit simulator
  - IBM Quantum hardware (IBM Cloud)

---

## 🏗️ Project Structure

```
SUPERDENSE_QUANTUM/
│
├── superdense-backend/
│   ├── aircraft.py
│   ├── sender.py
│   ├── receiver.py
│   ├── errorcorrection.py
│   ├── compare.py
│   ├── ibm_cloud.py
│   ├── app.py
│   ├── application.py
│   ├── simulated_flights.csv
│   ├── requirements.txt
│   └── .env
│
├── superdense-frontend/
│   ├── src/
│   │   ├── SuperdenseCoding.jsx
│   │   ├── QKDSimulation.jsx
│   │   ├── AircraftNavigation.jsx
│   │   ├── FullSimulation.jsx
│   │   └── Other UI Components
│   ├── package.json
│   └── vite.config.js
│
└── README.md
```


# 🚀 Installation & Setup

## 1️⃣ Clone Repository

```bash
git clone https://github.com/Lalithvignesh24/AQVH_Superdense-coding.git"
cd AQVH_Superdense-coding
```

---

# 🐍 Backend Setup (Python)

## Step 1: Navigate to backend

```bash
cd superdense-backend
```

## Step 2: Create virtual environment

```bash
python3 -m venv venv
```

## Step 3: Activate environment

### Mac / Linux
```bash
source venv/bin/activate
```

### Windows
```bash
venv\Scripts\activate
```

## Step 4: Install dependencies

```bash
pip install -r requirements.txt
```

---

# ▶️ Running Backend Files

You can run backend modules individually:

```bash
python3 aircraft.py
python3 sender.py
python3 receiver.py
python3 errorcorrection.py
python3 compare.py
python3 ibm_cloud.py
python3 app.py
python3 application.py
```

For complete integrated workflow:

```bash
python3 application.py
```

---

# ☁️ Running on IBM Quantum Hardware

1. Create an account at:
   https://quantum.ibm.com/

2. Copy your IBM Quantum API token.

3. Add it to `.env` file:

```
IBM_TOKEN= your_api_token_here
IBM_INSTANCE= crn_token_here
MONGO_USER= username_here
MONGO_PASSWORD= password_here
MONGO_CLUSTER_URL= api_key_here
OPENSKY_URL= _api_key_here


```

4. Run:

```bash
python3 ibm_cloud.py
```

This executes the quantum circuit on real IBM Quantum hardware.

---

# 💻 Frontend Setup (React + Vite)

```bash
cd superdense-frontend
npm install
npm run dev
```

Open in browser:

```
http://localhost:5173
```

---

# 🧪 Local Simulator vs IBM Quantum

| Feature | Local Simulator | IBM Quantum |
|----------|----------------|-------------|
| Speed | Fast | Slower (Queue-based) |
| Noise | Ideal | Real Quantum Noise |
| Real Hardware | No | Yes |
| Educational | Yes | Yes |

---

# 📊 Technologies Used

- Python
- Qiskit
- IBM Quantum Cloud
- Flask
- React.js
- Vite

---

# 🔐 Security Aspects

- Entanglement-based secure communication
- QKD-inspired key validation
- Measurement comparison
- Basic quantum error handling

---

# 🎯 Key Learning Outcomes

- Implementation of Superdense Coding
- Entanglement-based communication
- Running circuits on real quantum hardware
- Integrating classical aircraft prediction with quantum transmission
- Secure alert communication model

---

# 🛠 Troubleshooting

### Qiskit Installation Issue

```bash
pip install --upgrade qiskit qiskit-aer qiskit-ibm-runtime
```

### IBM Backend Connection Issue

- Verify API token
- Check internet connection
- Ensure backend is available on IBM dashboard

---

# 👨‍💻 Author

Quantum Communication Defense Simulation Project  
Superdense Coding + QKD + Aircraft Path Prediction  

---

# 📜 License

This project is for educational and research purposes only.