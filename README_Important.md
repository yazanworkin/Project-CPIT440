# 📂 LogicMinds Project — CPIT-440 Spam Detection

## 📋 الملفات المرفقة

| الملف | الوصف | متى تستخدمه |
|---|---|---|
| **LogicMinds_Proposal.docx** | المقترح (٢ صفحات) | تسلمه أولاً |
| **LogicMinds_Final_Report.docx** | التقرير النهائي (٩ صفحات) | تسلمه ثانياً |
| **LogicMinds_Presentation.pptx** | العرض التقديمي (١٢ سلايد) | للمناقشة |
| **Spam_Detection_Project.ipynb** | الكود الفعلي | تشغيله للحصول على النتائج |
| **spambase.csv** | البيانات | لازم بنفس مجلد الـ notebook |

---

## 🚀 خطوات قبل التسليم

### 1. تشغيل الكود (مهم جداً!)
- افتح `Spam_Detection_Project.ipynb` في VS Code
- تأكد إن `spambase.csv` بنفس المجلد
- اضغط **Run All**
- تأكد إن كل الخلايا اشتغلت صح (النتائج المتوقعة: Accuracy 90-96%)

### 2. مراجعة الملفات
- **Proposal:** راجعه مع المجموعة، تأكد من المعلومات
- **Final Report:** اقرأه كامل، تأكد إن الجدول والصور صحيحة
- **Presentation:** افتحه في PowerPoint، تدرب على العرض

### 3. التسليم على Blackboard
الدكتور قال "ارفعوا الكل قبل السبت" → ارفع **كل الملفات**:
1. LogicMinds_Proposal.docx
2. LogicMinds_Final_Report.docx
3. LogicMinds_Presentation.pptx
4. Spam_Detection_Project.ipynb (الكود)

---

## ⚠️ ملاحظات مهمة

### عن البيانات (spambase.csv)
الملف اللي عندك **بيانات تجريبية مشابهة** للـ UCI Spambase. للتسليم النهائي، **يُفضّل** إنك تحمل البيانات الحقيقية من:
- **الرابط الرسمي:** https://archive.ics.uci.edu/dataset/94/spambase
- تحمل ملف `spambase.data` وتعيد تسميته `spambase.csv`
- تستبدل ملفنا بالملف الحقيقي

البيانات الحقيقية راح تعطي نتائج مشابهة جداً (90-95% accuracy تقريباً).

### عن النتائج في التقرير
النتائج المذكورة في التقرير والـ Presentation:
- Decision Tree: 90.6%
- Naïve Bayes: 95.7%
- Random Forest: 95.5%

هذي نتائج حقيقية من البيانات التجريبية. لما تشغل على البيانات الحقيقية، الأرقام راح تكون مشابهة لكن ممكن تختلف بشوي. **بعد ما تشغل الكود، حدّث الأرقام في التقرير لو فيها فرق ملحوظ.**

---

## 👥 توزيع الشغل (موجود في Final Report)

| العضو | الدور | المهام |
|---|---|---|
| Azzam Saeed Alghamdi | Leader + ML Engineer | تنسيق المشروع، تحميل البيانات، Random Forest، أقسام 1-3 |
| Yazan Ezz Basnawi | Data Analyst | EDA، Decision Tree، الرسومات، أقسام 4-5 |
| Abdullah Mansour Alhalawani | ML Engineer + Reviewer | Naïve Bayes، Evaluation، Presentation، Conclusion |

---

## 🎓 نصائح للمناقشة

عند المناقشة مع الدكتور توقع أسئلة مثل:
1. **ليش اخترتم 3 algorithms معيّنة؟** → جواب: غطاهم الدكتور في الكورس، وكل واحد يمثّل عائلة مختلفة (tree-based, probabilistic, ensemble)
2. **ليش 75/25 split؟** → جواب: مناسب لحجم البيانات (4601)، يعطي test set كبير كفاية (1151) عشان نقيس بدقة
3. **ليش standardization فقط للـ Naïve Bayes؟** → جواب: لأنه يفترض distribution طبيعي (Gaussian)، أما Trees غير حساسة للـ scale
4. **ليش Naïve Bayes أعلى من Random Forest؟** → جواب: مفاجأة، لكنها معروفة في text classification. الـ Naïve Bayes شاطر لما الـ features مستقلة نسبياً
5. **ليش توصون بـ Random Forest وليس Naïve Bayes رغم إنه الأعلى؟** → جواب: Random Forest أكثر مرونة وأقل حساسية للـ outliers، وأفضل في الـ production الحقيقي

---

بالتوفيق يا فريق LogicMinds! 🚀
