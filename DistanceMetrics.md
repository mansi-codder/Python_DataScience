## Distance metrics commonly used in machine learning and  data science are :

These four distance metrics are commonly used in machine learning, data science, and various fields of mathematics to measure the similarity or difference between data points. Let’s break them down:

### **1. Euclidean Distance (📏 Straight-Line Distance)**
- Measures the **shortest** straight-line distance between two points in space.
- Calculated using the formula:
  \[
  d = \sqrt{(x_2 - x_1)^2 + (y_2 - y_1)^2}
  \]
- Example: Distance between two locations on a flat surface.

🔹 **Use case:** Clustering (e.g., K-Means), nearest neighbor searches.

---

### **2. Manhattan Distance (🛣️ Block-Based Distance)**
- Measures distance between two points **by only moving in horizontal and vertical directions** (like city blocks).
- Calculated using:
  \[
  d = |x_2 - x_1| + |y_2 - y_1|
  \]
- Example: Finding the shortest route in a grid-based city.

🔹 **Use case:** Robotics, pathfinding (e.g., taxi cab movement in a city).

---

### **3. Hamming Distance (🔢 Bitwise Difference)**
- Measures the **number of positions** where two strings/binary codes differ.
- Example:
  ```
  A = "1011101"
  B = "1001001"
  ```
  Hamming distance = **2** (since two positions differ).

🔹 **Use case:** Error detection/correction (like checksum, genetic sequencing).

---

### **4. Cosine Distance (📐 Angle-Based Similarity)**
- Measures how similar two vectors are **based on the cosine of their angle**.
- Formula:
  \[
  d = 1 - \frac{A \cdot B}{||A|| \times ||B||}
  \]
- Example: Comparing text documents by analyzing word frequency vectors.

🔹 **Use case:** Text analysis, recommendation systems.

---

### **Comparison Table**
| Distance Type    | Measurement Basis | Best for |
|-----------------|------------------|----------|
| **Euclidean**   | Straight-line distance | Physical distances, clustering |
| **Manhattan**   | Grid-like movement | Pathfinding, city navigation |
| **Hamming**     | Bit/character differences | DNA analysis, error detection |
| **Cosine**      | Angle similarity | Text comparison, vector analysis |


