
# 🌪️ AI-Powered Disaster Response & Prediction System

This project combines **multi-modal transformers** and **reinforcement learning** to build a hybrid disaster response system. It processes both **textual and visual inputs** to predict potential disasters and suggests intelligent response strategies using an RL agent.

---

## 📌 Key Features

- 🧠 **BERT-based** text processing
- 🖼️ **Vision Transformer (ViT)** for image inputs
- 🔀 Fused multi-modal prediction model for disaster detection
- 🧭 **Gym environment** for simulating disaster response actions
- 🎯 **Reinforcement Learning Agent** for decision-making and response planning

---

## 🛠️ Technologies Used

- Python 3.x
- PyTorch
- Hugging Face Transformers
- OpenAI Gym
- NumPy

---

## ⚙️ Project Structure

### 1. Multi-modal Preprocessing
- `preprocess_text(text)` → Tokenizes disaster-related text using BERT tokenizer.
- `preprocess_image_dummy()` → Generates a dummy image tensor for testing ViT input.

### 2. Disaster Prediction Model
- Combines `BERT` and `ViT` models.
- Final output is a 2-class prediction (e.g., `Safe`, `Disaster`).

### 3. RL-based Decision Module
- Custom `DisasterEnv` gym environment.
- `RLAgent` neural network suggests response actions:
  - `0`: Alert
  - `1`: Deploy
  - `2`: Evacuate
  - `3`: Wait

---

## ▶️ Example Execution

```bash
python ai_disaster_system.py
```

Example Output:
```
Disaster prediction (probabilities): [[0.25, 0.75]]
Recommended Action: 2 - Evacuate
```

---

## ✅ Installation Requirements

Install dependencies:

```bash
pip install torch transformers numpy gym
```

---

## 🔁 Future Scope

- Integrate real-time satellite and sensor data.
- Use real image datasets instead of dummy tensors.
- Train RL agent using policy gradients or PPO.
- Multi-agent coordination in disaster zones.

---

## 👨‍💻 Author

**Pavan Kumar**  
AI & ML Developer | Disaster Intelligence Systems  

