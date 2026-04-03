# Cat-vs-Dog-CNN-From-Scratch
A Deep Learning project to classify Cats and Dogs using a custom CNN architecture built from scratch with TensorFlow/Keras, featuring Grad-CAM visualization for model interpretability.

​🐾 Cat vs Dog Classification | Deep Learning from Scratch
​📝 مشروع تصنيف القطط والكلاب باستخدام الشبكات العصبية التلافيفية (من الصفر)
​📖 Overview | 
نظرة عامة
​
English:
This project aims to build a robust Convolutional Neural Network (CNN) from scratch to classify images of cats and dogs. Unlike using pre-trained models, this project focuses on understanding the underlying architecture, data engineering, and model interpretability using Grad-CAM.

​بالعربية

يهدف هذا المشروع إلى بناء شبكة عصبية تلافيفية (CNN) قوية من الصفر لتصنيف صور القطط والكلاب. على عكس استخدام النماذج الجاهزة، يركز هذا المشروع على فهم الهيكل الأساسي، هندسة البيانات، وتفسير قرارات النموذج باستخدام تقنية Grad-CAM.

​🛠️ Key Features | 
أهم مميزات المشروع

​Custom CNN Architecture: Built a multi-layer CNN optimized for binary classification.
​Data Augmentation: Implemented ImageDataGenerator with rotation, zoom, and flips to prevent overfitting and improve generalization.
​Fine-Tuning: Applied learning rate scheduling (1e-5) to stabilize training and reach peak accuracy.
​Model Explainability (Grad-CAM): Visualized heatmaps to understand which image features (ears, nose, fur) the model focuses on for its predictions.
​Professional Evaluation: Used Confusion Matrix and Classification Reports to analyze performance beyond simple accuracy.

​📊 Performance | 
أداء النموذج
​
English:
​Final Accuracy: Reached 83.59% on the unseen test set.
​Final Loss: Optimized down to 0.3851.
​Robustness: High F1-score for both classes, indicating a balanced model.

​بالعربية

​الدقة النهائية: حقق النموذج دقة تصل إلى 83.59% على بيانات الاختبار.
​نسبة الفقد: تم تقليل الفقد إلى 0.3851.
​القوة: درجة F1-score عالية ومتوازنة للفئتين، مما يدل على استقرار النموذج وعدم انحيازه.

​🖼️ Visualizations | الرسوم البيانية والنتائج
​
1. Learning Curves (Accuracy & Loss)
​
Shows the steady convergence and stability during the training and validation phases.

يوضح استقرار الموديل وتقارب منحنيات التدريب والاختبار مما يضمن عدم حدوث Overfitting.

​2. Confusion Matrix

​Detailed breakdown of correct vs. incorrect predictions for both Cats and Dogs.

تحليل دقيق لعدد الحالات الصحيحة والخاطئة لكل فئة لتحديد نقاط القوة والضعف.
​
3. Grad-CAM Analysis

​"Seeing through the model's eyes" - Identifying exactly where the model looks in the image.

"الرؤية بعيون الموديل" - تحديد المناطق التي يركز عليها النموذج لاتخاذ قراره

### 📈 1. نتائج التدريب | Training History
> يوضح الرسم البياني استقرار منحنيات الدقة والفقد (Loss & Accuracy) مما يؤكد نجاح عملية الـ Fine-tuning.
![Loss and Accuracy](<  <img width="1355" height="512" alt="graph_accuracy_and_loss" src="https://github.com/user-attachments/assets/ed45acd1-5a82-479c-824f-0bcd3f703c94" />
  >)

Model Convergence & Training Stability | 
استقرار النموذج وتقارب منحنيات التعلم

​English Description:

​Training Dynamics (Fine-tuning): The learning curves illustrate a healthy convergence between training and validation metrics. The stability of the validation accuracy around 83.6% and the downward trend of the loss function (reaching ~0.38) confirm that the model is well-regularized and generalizes effectively to unseen data.

​الوصف بالعربي

​ديناميكيات التدريب (الضبط الدقيق):
توضح منحنيات التعلم حالة من التقارب الصحي بين مقاييس التدريب والتحقق. استقرار دقة التحقق حول 83.6% مع الاتجاه الهبوطي المستمر لدالة الفقد (لتصل إلى حوالي 0.38) يؤكد كفاءة "التعميم" لدى النموذج واستقراره البرمجي ضد حدوث الـ Overfitting.


### 📊 2. مصفوفة الارتباك | Confusion Matrix
> تحليل تفصيلي لعدد الصور التي تم تصنيفها بشكل صحيح والخاطئ لكل فئة.
![Confusion Matrix](<  <img width="751" height="633" alt="Confusion_Matrix" src="https://github.com/user-attachments/assets/a857903a-2be7-42e1-b270-163200bbd119" />>)

Model Performance & Error Analysis | 
تحليل أداء النموذج ومصفوفة الارتباك

​English Description:

​Evaluation Metrics (Confusion Matrix): The matrix demonstrates robust predictive power on the unseen test set. The model achieved a high True Positive rate, correctly identifying 927 dogs and 764 cats. The low False Negative rate (only 85 missed dogs) reflects high sensitivity, confirming the model's reliability in distinguishing complex features between the two classes.

​الوصف بالعربي

​مقاييس التقييم (مصفوفة الارتباك):
تُظهر المصفوفة قدرة تنبؤية قوية للنموذج على بيانات الاختبار. نجح النموذج في التصنيف الصحيح لـ 927 كلب و 764 قطة. كما يعكس الانخفاض الملحوظ في معدل السلبيات الكاذبة (تجاهل 85 كلب فقط) حساسية عالية للموديل، مما يؤكد دقة استخلاص الميزات والتمييز بين الفئتين بفاعلية.


### 📝 3. تقرير التصنيف | Classification Report
> أرقام تفصيلية توضح دقة النموذج (Precision, Recall, F1-Score).
![Classification Report](<  <img width="551" height="206" alt="Classification_Report" src="https://github.com/user-attachments/assets/9bf8c2e4-67b5-4fe9-abf8-1f7d032a8064" />>)

Detailed Classification Metrics | 
مقاييس التصنيف التفصيلية

​English Description:

​Statistical Evaluation (Classification Report): The model demonstrates high precision and recall across both classes, achieving an overall Accuracy of 84%. With a Macro F1-Score of 0.83, the results confirm a balanced performance, specifically showing the model's high confidence in identifying cats (90% Precision) and its superior sensitivity in detecting dogs (92% Recall).

​الوصف بالعربي

​التقييم الإحصائي (تقرير التصنيف):
يُظهر الموديل توازناً كبيراً بين الدقة (Precision) والاستدعاء (Recall) للفئتين، محققاً دقة إجمالية بنسبة 84%. تشير قيمة F1-Score (0.83) إلى كفاءة الأداء واستقراره، مع تميز واضح في دقة تحديد القطط (90%) وحساسية عالية جداً في اكتشاف فئة الكلاب (92%).


### 🏁 4. التقييم النهائي | Final Evaluation
> النتيجة النهائية التي حققها النموذج على بيانات الاختبار المستقلة.
![Model Evaluation](<  <img width="665" height="149" alt="Model_Evaluation" src="https://github.com/user-attachments/assets/fe023b60-b4c8-40a2-af0e-6a703a44e943" />>)

Overall Test Performance | الأداء النهائي لنموذج الاختبار
​English Description:
​Final Generalization Results: The model achieves a solid 83.59% accuracy on the independent test set, with a optimized loss of 0.3851. These metrics verify that the custom CNN architecture effectively learned the core distinguishing features of cats and dogs, maintaining consistent performance between training and real-world inference.
​الوصف بالعربي:
​نتائج التعميم النهائية:
حقق النموذج دقة نهائية بلغت 83.59% على مجموعة بيانات الاختبار المستقلة، مع نسبة فقد مثالية وصلت إلى 0.3851. تؤكد هذه الأرقام نجاح بنية الـ CNN المصممة يدوياً في استخلاص الميزات الجوهرية للقطط والكلاب بفاعلية، مع الحفاظ على استقرار الأداء عند اختبار الموديل على بيانات جديدة تماماً.


---

### 🧠 5. تفسير قرارات النموذج | Grad-CAM Interpretability
> نستخدم هنا تقنية Grad-CAM لـ "رؤية ما يراه الموديل" وفهم المناطق التي يركز عليها لاتخاذ قراره:

**الحالة الأولى: تصنيف صحيح لقطة (Correct Prediction: CAT)**
> الموديل يركز على ملامح الوجه والأذنين.
![Grad-CAM Cat](<  <img width="1081" height="557" alt="Grade_CAM_1" src="https://github.com/user-attachments/assets/42363197-d312-48cd-a05a-896d031b530d" />
  >)

**الحالة الثانية: تصنيف صحيح لكلب (Correct Prediction: DOG)**
> الموديل يركز على جسم وهيكل الكلب لتمييزه.
![Grad-CAM Dog Correct](<  <img width="1088" height="562" alt="Grade_CAM_2" src="https://github.com/user-attachments/assets/f82e4d8a-9ab0-4c2c-b1db-65532d08e981" />
  >)

**الحالة الثالثة: خطأ في التصنيف (Miss-classification Case)**
> هنا نرى أين تشتت انتباه الموديل (صنف كلب على أنه قطة) بسبب زاوية التصوير أو الخلفية.
![Grad-CAM Error Case](<  <img width="1084" height="562" alt="Grade_CAM_3" src="https://github.com/user-attachments/assets/b1700f8f-9006-4018-8608-a30e564b9cb4" />
  >)


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

