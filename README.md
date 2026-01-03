# Humanoid Software Technical Exercise

This repository contains a technical exercise for training and evaluating a robotic dog's locomotion using the Genesis framework.

---

### 1. Clone this repository

```bash
git clone https://github.com/jpetrasek1217/genesis_exercise
cd genesis_exercise
```

---

### 2. Install the necessary Python libraries

```bash
pip install torch torchvision torchaudio
pip install genesis-world
pip install tensorboard gymnasium pyopengl stable-baselines3 rsl-rl-lib==2.2.4
```

---

### 3. Run the training script:

```bash
python go2_train.py
```

---

### 4. To monitor the training process, open TensorBoard in another terminal:

```bash
tensorboard --logdir logs
```

---

### 5. Take note of the final values under the `train/mean_reward` chart.

---

### 6. Evaluate the model

```bash
python go2_eval.py
```

---

### 7. Fix the issue in `go2_train.py` to improve the reward.

---

### 8. Retrain and compare TensorBoard results to what you had the first time.

> Make sure to save your first session’s results, as retraining will overwrite the output model files.

```bash
python go2_train.py
tensorboard --logdir logs
```

---

## Questions to Answer in Google Form

1. What did you fix from go2_train.py to improve the rewards? If you did not figure it out, what are your suspicions?

2. Look at the train/mean_reward chart. How did the training go according to the curve? What do the X and Y axes values mean?

3. Attach a screenshot of the final train/mean_reward training charts from the TensorBoard.

---

Hint: Consider the robotic dog’s joint starting positions when analyzing or modifying the training script.
