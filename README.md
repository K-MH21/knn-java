# k-Nearest Neighbors (k-NN) in Java with Jupyter

This project demonstrates how to implement the k-Nearest Neighbors (k-NN) algorithm from scratch in **Java**, using the classic **Iris dataset**.

It includes:
- Standard k-NN (majority vote)
- Weighted k-NN (inverse distance)
- Data loading, cleaning, normalization (Z-score), and label encoding
- Evaluation with accuracy and printed misclassifications

The entire project runs inside a **Jupyter notebook** using the [JJava kernel](https://github.com/dflib/jjava).

---

## 📂 Dataset

Uses the standard **Iris** dataset (150 samples, 3 classes: setosa, versicolor, virginica).  
Preprocessing steps include:
- Dropping the ID column
- Normalizing features with z-score
- Encoding species as integers (0, 1, 2)

---

## 📦 Requirements

- **Java 11+**  
- **Jupyter Notebook**
- **[IJava kernel](https://github.com/SpencerPark/IJava)** for running Java in Jupyter
- The following JAR files:
  - [`opencsv-5.11.2.jar`](https://repo1.maven.org/maven2/com/opencsv/opencsv/5.11.2/)
  - [`commons-lang3-3.18.0.jar`](https://repo1.maven.org/maven2/org/apache/commons/commons-lang3/3.18.0/)

In the notebook, they are loaded with:

```java
%jars opencsv-5.11.2.jar
%jars commons-lang3-3.18.0.jar
```


---

## 🚀 Getting Started

1. Clone the repo.
2. Make sure you have Java 11+ installed.
3. Install Jupyter and the IJava kernel:
   - Instructions: [JJava GitHub](https://github.com/dflib/jjava)
4. Download the required JAR files and place them in the same folder as the notebook.
5. Launch the notebook:
   ```bash
   jupyter notebook iris-knn-java.ipynb
   ```
   
## 🧠 Notes
- No machine learning libraries are used — everything is implemented manually.
- Weighted k-NN helps improve performance by reducing the effect of far neighbors.
- The Iris dataset is ideal for learning and testing basic classification techniques.
- Notebook includes basic exploratory analysis and feature normalization.
