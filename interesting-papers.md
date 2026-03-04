[SymTorch: A Framework for Symbolic Distillation of Deep Neural Networks](https://arxiv.org/pdf/2602.21307)

- SymTorch addresses a complementary question: what function does a component compute? In doing so, we provide a more holistic approach to model interpretability.
- Inspired by this physics-centric view of interpretability,
SymTorch brings a symbolic perspective to Neural Network
(NN) analysis1. We use Symbolic Regression (SR) to distill
NN components into human-readable mathematical formulas. Symbolic distillation provides architecture-agnostic
interpretability by approximating component behavior with
closed-form expressions. This enables direct inspection of
input-output mappings and analysis of how input variations
affect outputs, including in out-of-distribution settings.

- SymTorch handles the engineering challenges of GPU-CPU data transfer, activation
caching, forward hook management, and hybrid neuralsymbolic model serialization

Definitions
<strong>Symbolic surrogates</strong> are explicit, interpretable algebraic approximations—often generated via symbolic regression or sparse identification—used to emulate complex, expensive computational models or physical systems. They provide closed-form equations, allowing for high efficiency, analytical manipulation, and, unlike neural networks, full transparency in high-dimensional AI,, scientific, and engineering applications.

<img width="664" height="323" alt="Screenshot 2026-03-04 at 12 16 03 PM" src="https://github.com/user-attachments/assets/f63c33da-ce67-4685-80f1-a3ccca65de67" />


