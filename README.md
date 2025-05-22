# Adversarial Attacks

## Definition

Adversarial attacks manipulate inputs (images, text, audio) with imperceptible perturbations to fool machine learning models into making incorrect predictions.

---

## Types

1. **White-Box Attacks**
  - Attacker has full model access (architecture, gradients).
2. **Black-Box Attacks**
  - Attacker queries model outputs only.
3. **Targeted Attacks**
  - Force specific incorrect predictions.
4. **Non-Targeted Attacks**
  - Cause any misclassification.
5. **Physical Attacks**
  - Real-world perturbations (e.g., stickers on stop signs).
6. **Universal Attacks**
  - Single perturbation fools multiple inputs.

---

## Construction Methods

1. **FGSM (Fast Gradient Sign Method)**
  - Perturbation direction: Gradient sign.
2. **PGD (Projected Gradient Descent)**
  - Iterative FGSM with bounded perturbations.
3. **Carlini & Wagner (C&W)**
  - Optimization-based attack with minimal noise.
4. **GAN-Based Attacks**
  - Generate adversarial examples via generative networks.
5. **Jacobian-Based Saliency Maps**
  - Modify critical features identified by Jacobian matrices.

---

## Real-World Examples

1. **Autonomous Vehicles**
  - Adversarial stickers on road signs mislead object detection.
2. **Facial Recognition**
  - Specially designed glasses bypass face ID systems.
3. **NLP**
  - Text perturbations fool sentiment analysis/translation models.
4. **Healthcare**
  - Perturbed medical images misdiagnose conditions.
5. **Social Media**
  - Adversarial posts evade content moderation filters.

---

## Key Challenges

1. **Transferability**
  - Attacks on one model may fail on another.
2. **Real-World Robustness**
  - Environmental factors (lighting, angles) reduce attack efficacy.
3. **Detection Difficulty**
  - Adversarial examples often resemble clean data.
4. **Trade-Offs**
  - Robustness improvements may reduce model accuracy.
5. **Scalability**
  - High compute costs for large-scale attacks/defenses.

---

## Defenses

1. **Adversarial Training**
  - Train models on adversarial examples.
2. **Input Preprocessing**
  - Denoising, quantization, or JPEG compression.
3. **Detection Networks**
  - Separate models flag adversarial inputs.
4. **Certified Defenses**
  - Provable robustness guarantees via formal methods.
5. **Ensemble Methods**
  - Combine multiple models to dilute attack impact.

---

## Research Gaps

1. **Real-World Robustness**
  - Attacks/defenses under dynamic physical conditions.
2. **Transferability**
  - Cross-model/cross-domain attack generalization.
3. **Explainability**
  - Understanding why specific perturbations work.
4. **Energy-Efficient Attacks**
  - Low-resource methods for edge devices.
5. **Multimodal Attacks**
  - Coordinated perturbations across text/image/audio.
6. **Ethical Frameworks**
  - Balancing robustness with fairness/privacy.
7. **Lifelong Learning**
  - Defenses against adaptive adversaries over time.
8. **Standardized Evaluation**
  - Unified benchmarks for attack/defense efficacy.
