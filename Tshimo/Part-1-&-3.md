# 🔹 Tshimo – AI Tools & Applications: Theoretical Understanding & Ethics

## Part 1: Theoretical Understanding

### Q1: Explain the primary differences between TensorFlow and PyTorch. When would you choose one over the other?

**TensorFlow** and **PyTorch** are both powerful, open-source deep learning frameworks, but they differ in architecture, syntax, and usage preferences:

| Feature | TensorFlow | PyTorch |
|--------|------------|---------|
| **Execution Model** | Static computation graph (TensorFlow 1.x) and eager execution (TensorFlow 2.x) | Dynamic computation graph (eager by default) |
| **Ease of Use** | Slightly more verbose and abstract | More Pythonic and intuitive |
| **Community & Industry Use** | Widely used in production (e.g., Google, production-grade pipelines) | Preferred in research and experimentation (e.g., academia, rapid prototyping) |
| **Visualization** | TensorBoard for visual debugging | TensorBoard support via integration; native debugging is simpler |
| **Deployment** | Strong deployment tools like TensorFlow Lite and TensorFlow Serving | TorchScript and ONNX for deployment, slightly less mature ecosystem |

**When to Choose Which:**
- Choose **TensorFlow** if your goal is **robust deployment**, **cross-platform inference**, or using **Google Cloud tools**.
- Choose **PyTorch** for **research**, **rapid development**, or **educational settings** where code readability and flexibility matter most.

---

### Q3: How does spaCy enhance NLP tasks compared to basic Python string operations?

spaCy enhances NLP workflows with pre-trained pipelines and deep linguistic features that go far beyond what basic Python string functions can provide:

| Feature | Basic Python | spaCy |
|---------|--------------|--------|
| **Tokenization** | Manual string splitting | Language-specific, rule-based + statistical |
| **Part-of-Speech Tagging** | Not supported | Built-in tagging with linguistic context |
| **Named Entity Recognition (NER)** | Not available | Pre-trained models detect names, dates, organizations, etc. |
| **Dependency Parsing** | Manual or external tools required | Built-in syntactic dependency analysis |
| **Speed & Accuracy** | Limited and manual | Optimized for production and high accuracy |
| **Pipeline Support** | None | Modular NLP pipelines for preprocessing and inference |

spaCy streamlines complex NLP workflows, making it more efficient and scalable for real-world applications.

---

## Part 3: Ethics & Optimization

### Ethical Considerations: Model Biases and Mitigation using TensorFlow Fairness Indicators or spaCy

**Model Bias in AI:**
Machine learning models often inherit biases present in training data, leading to unfair or discriminatory outcomes. This can be especially harmful in sensitive applications like hiring, healthcare, or law enforcement.

**Mitigation with TensorFlow Fairness Indicators:**
TensorFlow provides **Fairness Indicators**—a suite of tools that enable evaluation of model performance across different slices of data (e.g., age, gender, race). It helps:
- Identify disparities in precision, recall, or accuracy
- Visualize and compare metrics across subgroups
- Promote transparent model evaluation before deployment

**Mitigation with spaCy:**
While spaCy is not fairness-specific, developers can:
- Inspect and preprocess biased text data before training
- Use curated datasets to reduce linguistic or cultural bias
- Manually audit NER or classification outputs for skewed results

**Best Practices:**
- Use diverse and representative training data
- Continuously monitor performance across user groups
- Document assumptions, limitations, and potential harms

---

_This file was prepared for AI Tools & Applications coursework by Tshimo._
