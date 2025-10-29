# Enter the Matrix: An Introduction to Linear Algebra

## 📖 Overview

*Enter the Matrix* is a complete learning module designed to teach **Linear Algebra through coding**.  
It combines concise theoretical lessons with practical exercises that guide you in implementing key mathematical concepts — from vector operations to matrix transformations — in code.

While the examples use **Rust** syntax, the concepts are **language-agnostic** and can be implemented in any programming language that supports:
- Generic types
- First-class functions (lambdas)
- (Optional) Operator overloading

---

## 🧩 Structure

The document includes:
- **Conceptual explanations**: vectors, matrices, linear maps, norms, dot & cross products, etc.
- **Step-by-step exercises**: progressive coding tasks to solidify understanding.
- **Implementation rules**: design guidelines for building a consistent math library.

---

## 🗂️ Contents (Main Chapters)

1. **Foreword** – Importance of Linear Algebra in physics, CS, graphics, and ML.  
2. **Introduction** – GPU computation, vector spaces, and linear transformations.  
3. **Code Constraints** – Data structures (`Vector<K>`, `Matrix<K>`) and implementation rules.  
4. **Exercises 00–15** –  
   - Add, Subtract, and Scale  
   - Linear Combination  
   - Linear Interpolation  
   - Dot Product and Norms  
   - Cosine and Cross Product  
   - Matrix Multiplication, Trace, Transpose, Determinant, Inverse  
   - Rank, Projections, and Complex Spaces  

---

## ⚙️ Requirements

- No external math libraries allowed (unless stated).
- Implement all algorithms manually (O(n) complexity where possible).
- Respect provided time/space complexity constraints.
- Peer evaluation is expected for verification.

---

## 💡 Example Exercise (Add, Subtract, and Scale)

```rust
impl<K> Vector<K> {
    fn add(&mut self, v: &Vector<K>);
    fn sub(&mut self, v: &Vector<K>);
    fn scl(&mut self, a: K);
}

impl<K> Matrix<K> {
    fn add(&mut self, v: &Matrix<K>);
    fn sub(&mut self, v: &Matrix<K>);
    fn scl(&mut self, a: K);
}
