# Image Labelling and Ranking Project

## **Overview**

This project focuses on developing a prototype model for classifying and ranking images, primarily for use in the travel industry, to enhance customer perception and improve booking rates. The core motivation is to address the need for an automated system that can effectively categorize and assess the quality of a vast number of images associated with various properties, ensuring that visually appealing and relevant images are presented to users.

---

## **Problem Statement**

Hotel booking platforms often display millions of images without proper ordering or classification, and some images may even be visually unappealing. This lack of organization and quality control can negatively impact conversion rates, as customers have diverse image preferences. The challenge is to sort these large sets of images by category and a human-perception-based "attractiveness" quality score.

---

## **Project Goals**

The primary goal of this research project is to build a prototype model that performs two main functions:

* **Image Tagging**: Assigning a relevant category name to images.
* **Quality Scoring**: Assigning a quality score to images, reflecting their attractiveness.

---

## **Methodology**

This project extensively explores Deep Learning applications for image classification and ranking. Both supervised and unsupervised learning methods were implemented.

### **Key Steps:**

1.  **Data Exploration**: Analyzing data structures, image categories, and performing semantic similarity checks between image categories and associated free text.
2.  **Feature Extraction**: Utilizing Convolutional Neural Networks (CNNs), specifically *Xception-Net*, to extract meaningful feature vectors from images.
3.  **Image Labelling (Clustering Solution)**:
    * Unsupervised learning, particularly clustering algorithms, was chosen due to inconsistencies and ambiguities found in existing image labels.
    * Comparison of various clustering algorithms (K-Means, Hierarchical Agglomerative Clustering) applied to features extracted from CNNs to determine the best performance metrics (Silhouette coefficient and Normalized Mutual Index Score).
    * K-Means algorithm was implemented for its efficiency with large datasets, using the 'Elbow' method to determine the optimal number of clusters.
4.  **Image Ranking (Supervised Transfer Learning)**: After images were tagged with cluster-identified labels, a ranking model was built using supervised transfer learning.

---

## **Technologies and Libraries**

The project leverages various technologies and libraries in the domain of Computer Vision and Deep Learning:

* **Computer Vision**
* **Transfer Learning**
* **Convolutional Neural Networks (CNNs)**
* **Clustering Algorithms**
* **Tensorflow**
* **Keras**
* **Microsoft Azure**
* `Pandas`, `NumPy`, `Scikit-learn`, `spaCy` for data processing and exploration.

---

## **Data**

The project utilizes millions of images, with approximately eleven million images originating from a Global Distribution System (GDS) database. These images were accessed via URLs stored in 3-element tuples, which include an image category and free text describing the image.

### Data Structures:

* Linear data structures (arrays, stacks for data frames)
* Hash maps (for dictionaries)
* Graphs (for visualizations) were used for data access and manipulation.

### Image Categories:

* Initial data included 23 provider image categories, with "guest room" being the most frequent.
* However, inconsistencies and ambiguities in these labels necessitated an unsupervised learning approach.

---

## **Conclusion**

This project successfully developed a prototype for image labelling and ranking using advanced Deep Learning techniques. By applying clustering algorithms on features extracted from CNNs and building a ranking model with supervised transfer learning, the project aims to improve the visual content displayed in the travel industry, ultimately enhancing user experience and conversion rates.

---

## **About the Author**

**Abhinav SHARMA/AbhiDS91**


* **Internship Dates**: May 1, 2020 - October 30, 2020
