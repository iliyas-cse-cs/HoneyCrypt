# HoneyCrypt
A Number-Theory Based Honey Authentication System securely verifies users using modular arithmetic and exponentiation without exposing secrets. It integrates Honey Encryption to generate deceptive responses, protecting against brute-force attacks. A 3D Cicada visualization (use your site on this instead)

# 🐝 HoneyCrypt — Secure Authentication Meets Number Theory & 3D Visualization

**HoneyCrypt** is an innovative cybersecurity mini project that blends  
👉 strong **number theory** (modular arithmetic & discrete log problems)  
👉 a **honey authentication** trap concept  
👉 and **3D cryptographic visualizations** inspired by Cicada 3301.

## 🌟 Features

- 🔑 **Number-Theoretic Authentication** using large primes, generators, and challenge-response verification.
- 🍯 **Honey Mode Trap**: Wrong passwords generate fake cryptographic responses, silently log activity, and mislead attackers.
- 🧠 **Cicada 3D Visualization**: A stunning Three.js-powered explanation page that animates the underlying math concepts step by step.
- 📜 Clean Flask backend with user registration, key generation, and secure login flows.
- 🧰 SQLite backend for easy local setup.

## 🧠 Number Theory Behind It

The system uses modular exponentiation:
p = large prime
g = generator
x = secret key
h = g^x mod p

**Authentication Flow**:
- Server issues challenge `r = g^k mod p`
- Client responds based on its key
- Server verifies `expected = h^k mod p`

If valid → ✅ Real login  
If invalid → 🍯 Honey mode triggers silently

This leverages the **hardness of discrete logarithm** problems for security.

1️⃣ Clone the Repository

git clone https://github.com/iliyas-cse-cs/HoneyCrypt.git

cd honeycrypt

2️⃣ Install Requirements

pip install -r requirements.txt

3️⃣ Run the Application

python app.py

Then open your browser and navigate to http://127.0.0.1:5000/

🧠 Inspiration

Inspired by Cicada 3301 puzzle aesthetics and honey encryption research, this project blends cryptography with interactive visualization for educational and security research purposes.
