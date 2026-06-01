# Contributing to AIDPSI

Thank you for your interest in contributing! 
This project welcomes contributions of all kinds — bug fixes, new features, documentation improvements, and more.

---

## Getting Started

1. **Fork** the repository on GitHub
2. **Clone** your fork locally:
   ```bash
   git clone https://github.com/YOUR_USERNAME/Productivity-stress-prediction-model.git
   cd Productivity-stress-prediction-model
   ```
3. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```
4. **Create a branch** for your changes:
   ```bash
   git checkout -b feature/your-feature-name
   ```

---

## Types of Contributions

### Bug Reports
- Open an [issue](../../issues) with the label `bug`
- Include steps to reproduce, expected vs actual behavior, and your Python version

### Feature Requests
- Open an [issue](../../issues) with the label `enhancement`
- Describe the feature and why it would be useful

### Pull Requests
1. Make your changes in your feature branch
2. Keep commits focused and descriptive:
   ```
   Add: new model evaluation metric (F1 score)
   Fix: scaler mismatch in productivity pipeline
   Docs: update dataset feature descriptions
   ```
3. Push to your fork and open a Pull Request against the `main` branch
4. Fill in the PR description explaining what you changed and why

---

## Code Guidelines

- Use **Python 3.8+** compatible code
- Follow **PEP 8** style conventions
- Add **comments** to any non-obvious logic, especially in ML pipelines
- If you add a new model or feature, update `requirements.txt` if needed
- Test your changes by running the Streamlit app: `streamlit run GUI.py`

---

## 📁 Areas Open for Contribution

| Area | Ideas |
|------|-------|
|  Models | Try XGBoost, Random Forest, or neural networks |
|  EDA | Add new visualizations to `Analysis.ipynb` |
|  GUI | Improve the Streamlit UI layout or add charts |
|  Data | Contribute anonymized developer data |
|  Docs | Improve README, add examples, write a wiki |
|  Tests | Add unit tests for data preprocessing and model loading |

---

## Before Submitting

- [ ] Code runs without errors
- [ ] `streamlit run GUI.py` still works if you changed `GUI.py`
- [ ] No sensitive or personal data is included
- [ ] Commit messages are clear and descriptive

---

## Questions?

Open a [discussion](../../discussions) or an issue — happy to help!