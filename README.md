# Humanoid Software Technical Exercise

This repository contains a technical exercise for training and evaluating a robotic dog's locomotion using the Genesis framework.

---

## Getting Started

### Clone the Repository

```bash
git clone https://github.com/jpetrasek1217/genesis_exercise
cd genesis_exercise
```

### Install Dependencies

Install the necessary Python libraries:

```bash
pip install tensorboard rsl-rl-lib==2.2.4
```

---

## Training the Model

Run the training script:

```bash
python go2_train.py
```

To monitor the training process, open TensorBoard in another terminal:

```bash
tensorboard --logdir logs
```

> Take note of the final values under the `train/mean_reward` chart.

---

## Evaluating the Model

Run the evaluation script:

```bash
python go2_eval.py
```

---

## Improving the Model

1. **Fix the issue in `go2_train.py`** to improve the reward.
2. Retrain the model and compare the TensorBoard results to your initial training session.

```bash
python go2_train.py
tensorboard --logdir logs
```

> Make sure to save your first session’s results, as retraining will overwrite the output model files.

---

## Questions to Answer

1. **Fix Analysis:**
   What did you fix in `go2_train.py` to improve the rewards? If you did not figure it out, what are your suspicions?

2. **Training Curve Analysis:**
   Examine the `train/mean_reward` chart in TensorBoard. How did the training progress according to the curve? What do the X and Y axes represent?

3. **Screenshot:**
   Attach a screenshot of the final `train/mean_reward` chart from TensorBoard.

---

## Hint

Consider the robotic dog’s joint starting positions when analyzing or modifying the training script.
