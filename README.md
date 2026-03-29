# Cat-vs-Dog-CNN-From-Scratch
A Deep Learning project to classify Cats and Dogs using a custom CNN architecture built from scratch with TensorFlow/Keras, featuring Grad-CAM visualization for model interpretability.

​🐾 Cat vs Dog Classification | Deep Learning from Scratch
​📝 مشروع تصنيف القطط والكلاب باستخدام الشبكات العصبية التلافيفية (من الصفر)
​📖 Overview | نظرة عامة
​English:
This project aims to build a robust Convolutional Neural Network (CNN) from scratch to classify images of cats and dogs. Unlike using pre-trained models, this project focuses on understanding the underlying architecture, data engineering, and model interpretability using Grad-CAM.
​بالعربية:
يهدف هذا المشروع إلى بناء شبكة عصبية تلافيفية (CNN) قوية من الصفر لتصنيف صور القطط والكلاب. على عكس استخدام النماذج الجاهزة، يركز هذا المشروع على فهم الهيكل الأساسي، هندسة البيانات، وتفسير قرارات النموذج باستخدام تقنية Grad-CAM.
​🛠️ Key Features | أهم مميزات المشروع
​Custom CNN Architecture: Built a multi-layer CNN optimized for binary classification.
​Data Augmentation: Implemented ImageDataGenerator with rotation, zoom, and flips to prevent overfitting and improve generalization.
​Fine-Tuning: Applied learning rate scheduling (1e-5) to stabilize training and reach peak accuracy.
​Model Explainability (Grad-CAM): Visualized heatmaps to understand which image features (ears, nose, fur) the model focuses on for its predictions.
​Professional Evaluation: Used Confusion Matrix and Classification Reports to analyze performance beyond simple accuracy.
​📊 Performance | أداء النموذج
​English:
​Final Accuracy: Reached 83.59% on the unseen test set.
​Final Loss: Optimized down to 0.3851.
​Robustness: High F1-score for both classes, indicating a balanced model.
​بالعربية:
​الدقة النهائية: حقق النموذج دقة تصل إلى 83.59% على بيانات الاختبار.
​نسبة الفقد: تم تقليل الفقد إلى 0.3851.
​القوة: درجة F1-score عالية ومتوازنة للفئتين، مما يدل على استقرار النموذج وعدم انحيازه.
​🖼️ Visualizations | الرسوم البيانية والنتائج
​1. Learning Curves (Accuracy & Loss)
​Shows the steady convergence and stability during the training and validation phases.
يوضح استقرار الموديل وتقارب منحنيات التدريب والاختبار مما يضمن عدم حدوث Overfitting.
​2. Confusion Matrix
​Detailed breakdown of correct vs. incorrect predictions for both Cats and Dogs.
تحليل دقيق لعدد الحالات الصحيحة والخاطئة لكل فئة لتحديد نقاط القوة والضعف.
​3. Grad-CAM Analysis
​"Seeing through the model's eyes" - Identifying exactly where the model looks in the image.
"الرؤية بعيون الموديل" - تحديد المناطق التي يركز عليها النموذج لاتخاذ قراره

### 📈 1. نتائج التدريب | Training History
> يوضح الرسم البياني استقرار منحنيات الدقة والفقد (Loss & Accuracy) مما يؤكد نجاح عملية الـ Fine-tuning.
![Loss and Accuracy](<  <img width="1355" height="512" alt="graph_accuracy_and_loss" src="https://github.com/user-attachments/assets/ed45acd1-5a82-479c-824f-0bcd3f703c94" />
  >)

### 📊 2. مصفوفة الارتباك | Confusion Matrix
> تحليل تفصيلي لعدد الصور التي تم تصنيفها بشكل صحيح والخاطئ لكل فئة.
![Confusion Matrix](<    >)

### 📝 3. تقرير التصنيف | Classification Report
> أرقام تفصيلية توضح دقة النموذج (Precision, Recall, F1-Score).
![Classification Report](<    >)

### 🏁 4. التقييم النهائي | Final Evaluation
> النتيجة النهائية التي حققها النموذج على بيانات الاختبار المستقلة.
![Model Evaluation](<    >)

---

### 🧠 5. تفسير قرارات النموذج | Grad-CAM Interpretability
> نستخدم هنا تقنية Grad-CAM لـ "رؤية ما يراه الموديل" وفهم المناطق التي يركز عليها لاتخاذ قراره:

**الحالة الأولى: تصنيف صحيح لقطة (Correct Prediction: CAT)**
> الموديل يركز على ملامح الوجه والأذنين.
![Grad-CAM Cat](<    >)

**الحالة الثانية: تصنيف صحيح لكلب (Correct Prediction: DOG)**
> الموديل يركز على جسم وهيكل الكلب لتمييزه.
![Grad-CAM Dog Correct](<    >)

**الحالة الثالثة: خطأ في التصنيف (Miss-classification Case)**
> هنا نرى أين تشتت انتباه الموديل (صنف كلب على أنه قطة) بسبب زاوية التصوير أو الخلفية.
![Grad-CAM Error Case](<    >)


​💻 Technologies Used | التقنيات المستخدمة
​Language: Python.
​Deep Learning: TensorFlow / Keras.
​Visualization: Matplotlib, Seaborn.
​Environment: Google Colab (T4 GPU).
​🚀 How to Use | كيفية الاستخدام
​English:
​Clone the repository.
​Load the .h5 model file.
​Use the predict function to classify your own pet photos!
​بالعربية:
​قم بتحميل المشروع.
​قم باستدعاء ملف الموديل .h5.
​استخدم دالة التوقع (Predict) لتجربة الموديل على صور حيواناتك الأليفة!

