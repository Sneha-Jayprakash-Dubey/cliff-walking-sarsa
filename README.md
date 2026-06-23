# 🧗 CliffWalking with SARSA (Gymnasium + Python)

## 📌 Overview
This project demonstrates **SARSA (State–Action–Reward–State–Action)**, an on‑policy reinforcement learning algorithm, applied to the **CliffWalking environment** from Gymnasium.  
It’s designed for:
- 🎓 Students learning RL basics  
- 💼 Recruiters evaluating applied ML/AI projects  

The agent learns to navigate a gridworld without falling off the cliff, balancing exploration and exploitation.

---

## ⚙️ Tech Stack
- Python 3.10+
- Gymnasium (CliffWalking‑v1 environment)
- NumPy (Q‑table operations)
- Matplotlib (visualizations)
- Jupyter Notebook (optional)

---

## 🚀 How It Works
- **State space**: 48 discrete positions in the grid  
- **Action space**: 4 moves (up, down, left, right)  
- **Algorithm**: SARSA with epsilon‑greedy policy  
- **Update rule**:  
  

\[
  Q(s,a) \leftarrow Q(s,a) + \alpha \big[ r + \gamma Q(s',a') - Q(s,a) \big]
  \]



---

## 📊 Training Results
- The agent improves over **500 episodes**.  
- Rewards start negative (falling off cliffs) but improve as the agent learns safer paths.  
- SARSA tends to learn **safer trajectories** compared to Q‑learning, which may choose riskier but shorter paths.

---

## 🖥️ Usage
Clone the repo and install dependencies:

```bash
git clone https://github.com/your-username/cliff_walking_sarsa.git
cd cliff_walking_sarsa
pip install -r requirements.txt
```

Run the notebook:

bash
```
jupyter notebook SARSA_impl.ipynb
```

📂 Repository Structure
code
```
cliff_walking_sarsa/
│── SARSA_impl.ipynb        # Jupyter Notebook with SARSA code
│── requirements.txt        # Dependencies
│── .gitignore              # Ignore checkpoints and temp files
│── README.md               # Project documentation
```

I have also implemented this problem using Q‑learning, which is generally considered a better approach for CliffWalking since it learns the optimal policy (off‑policy).

👉 Check out the Q‑learning implementation here:

https://github.com/Sneha-Jayprakash-Dubey/cliff_qlearning_rl_project

📈 Learning Outcomes :

Understand SARSA fundamentals
Compare SARSA vs Q‑learning behavior
Implement epsilon‑greedy exploration
Apply RL to a classic control problem
Showcase a clean, recruiter‑friendly ML project
