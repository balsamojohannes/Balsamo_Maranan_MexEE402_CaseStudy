# MexEE 402: Data Preprocessing Case Study

**MexEE Elective 2: Data Science and Machine Learning**  
**Batangas State University – Alangilan Campus**  
**1st Semester, AY 2026–2027**

---

## 👥 Members

| Name | Student Number | Section |
|---|---|---|
| Balsamo, Johannes C. | 23-07356 | MEXE 4101 |
| Maranan, Alliana Maurice B. | 23-00661 | MEXE 4101 |

---

## 📚 Notebook Links

| Chapter | Balsamo | Maranan |
|---|---|---|
| Chapter 1,2, & 3 | [link](https://colab.research.google.com/drive/1PmJ-JCiv6ojrx_A9Zd5xscvwoj1vOR9H?usp=sharing) | [link](https://colab.research.google.com/drive/1OFkULaWrTIqt7hmuHu0gdjLdbvLa2CJS?usp=sharing) |
| Chapter 4 | [link](https://colab.research.google.com/drive/1Hp-TqbZ0nw1is19u99GSCZjd3KogMGlE?usp=sharing) | [link](https://colab.research.google.com/drive/1Q3-ucsP4Uq2dvcIkrfbYAZqRkGgfDHDK?usp=sharing) |
| Chapter 5| [link](https://colab.research.google.com/drive/1oSdwTByyreMfD_rag2NuprYxBw0vKimp?usp=sharing) | [link](https://colab.research.google.com/drive/1_WdAyvIXbMepLvDo1F5uJjKVIvD8RDDp?usp=sharing) |
| Chapter 6| [link](https://colab.research.google.com/drive/11icyLzzlE1GduB_gqVmkYS5KHjQuH4IN?usp=sharing) | [link](https://colab.research.google.com/drive/1ojgVgTHwPaheQ9LQ2zYQDdUWKhQzcJhf?usp=sharing) |
| Chapter 7| [link](https://colab.research.google.com/drive/11jCaJ1jmLHqeVtXLc068hl2sm6W-NgT7?usp=sharing) | [link](https://colab.research.google.com/drive/1csZv3XoNhTtiWxRlNUWfeAFg-F3FQ_ui?usp=sharing) |
| Chapter 8| [link](https://colab.research.google.com/drive/1Boe3sg6ExVkKWEj2mmrWumw4PonAseLz?usp=sharing) | [link](https://colab.research.google.com/drive/1a_Wz9uh-N4KqjGZppIOY4NLTX8hLqe-f?usp=sharing) |
| Chapter 9| [link](https://colab.research.google.com/drive/1Ub4n03AduqAaHBOKyRLsUUqtHuouktBX?usp=sharing) | [link](https://colab.research.google.com/drive/13TodkjVWuLT4JlKReXnnqHjmmpmfMa7R?usp=sharing) |

---

## 🧠 What We Learned

### Chapter 1,2, & 3
In chapters 1-3, we have learned about the foundation of data pre-processing from the introduction, exploration, and cleaning of our data. It made us realize how important it is for data to undergo pre-processing to produce clean and organized data for machine learning models. We observed that there are issues that may arise such as missing, inconsistent and irrelevant data, so that brought us in understanding the preprocessing techniques used in respective issues that cleans our data. Furthermore, it surprised us that there are methods to easily explore a dataset, which increases efficiency. 

### Chapter 4
Chapter 4 gave us a deeper understanding of data transformation and feature engineering. We have learned that feature engineering could allow us to transform a variable or feature into a useful feature, and there are methods that we can use to reveal more useful patterns. It taught us about creating new features, binning data, interaction features, and the difference between one-hot and ordinal encoding. What surprised us was that simply combining existing features can produce a new pattern. Thus, this made us realize that there are different ways to make the machine learning model understand our data effectively by revealing useful patterns if we use appropriate methods with the right features. 

### Chapter 5
In chapter 5, we understood the importance of data scaling and normalization in machine learning models because they make all features fall in a comparable range or distribution and prevent large scales from dominating the model. It also taught us the difference between StandardScaler and MinMaxScaler. What surprised us is that simple large numbers can negatively impact how the model understands the data and may treat large numbers as more important features. Moreover, we have learned that it is important to know what your algorithm is and how it processes the input features to know whether to use scaling or not. Therefore, knowing your data will help improve the performance of an ML model. 

### Chapter 6
In this chapter, we gained a deeper understanding on what outliers are. We learned that it can affect the results and sometimes create a misleading data. This chapter also taught us how to find outliers by using two methods which are z-score and IQR method, as well as on how to handle them.

### Chapter 7
In chapter 7, it taught us that feature selection is all about choosing the features or categories that are the most useful for making predictions. We were able to identify the different methods for feature selection such as filter, wrapper, and embedded methods, and their distinction from one another. What surprised us was that those three methods for feature selection choose different features from the same dataset, which gave us insights that when choosing a method for feature selection, it must be appropriate on what the machine learning model was trying to predict. This chapter also taught us the correlation of each variable from one another.

### Chapter 8
Chapter 8 is all about preprocessing pipeline which organizes the data. We learned the different processes of handling missing data. The first method is imputation wherein it handles the missing values by replacing it with the mean/median. Then after that it was scaled to standardize the data, so that one feature does not have a huge influence to others.

### Chapter 9
In this chapter, we were able to apply the techniques that we learned from the previous chapters to clean and transform a messy dataset. What surprised us the most was how much preprocessing can change and improve the data. We also able to visualize the data using various plots after the data preprocessing. 

---

## ⚠️ Errors We Found

| Chapter | Original Error | Correct Version |
|---|---|---|
| Chapter 6 | outliers = data[np.abs(z_scores) > 3] | outliers = data[np.abs(z_scores) > 2] |
| Chapter 7 | selector = RFECV(estimator, step=1, cv=5) | selector = RFECV(estimator, step=1, cv=3) |
| Chapter 9 | plt.hist(data['Age'].dropna(), alpha=0.5, label='Before discretization') | plt.hist(data['Age'].dropna(), alpha=0.5, label='After discretization') |
| | plt.hist(titanic_preprocessed[:,2], alpha=0.5, label='After discretization') | plt.hist(titanic_preprocessed[:,0], alpha=0.5, label='Before discretization') |

---

## 🤖 Note on AI Tools
We used AI tools to help us understand the different libraries, functions, and codes used in every chapter. We used AI mainly to explain what each library or function does and to help us understand the concepts better.

---

