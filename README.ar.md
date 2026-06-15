# بوت الدردشة الذكي - نظام محادثة ذكي

[![الترخيص: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![Streamlit](https://img.shields.io/badge/Streamlit-1.0+-red.svg)](https://streamlit.io/)
[![OpenAI](https://img.shields.io/badge/OpenAI-API-green.svg)](https://openai.com/)

تطبيق ويب حديث وتفاعلي لنظام دردشة ذكي مدعوم بنماذج GPT من OpenAI. مبني باستخدام Streamlit لتجربة مستخدم سهلة مع دعم كامل للغة العربية والإنجليزية.

## 🌟 المميزات

- 🤖 **محادثات قوية بالذكاء الاصطناعي** - يستخدم نماذج GPT من OpenAI للإجابات الذكية
- 🌍 **دعم متعدد اللغات** - دعم كامل للعربية والإنجليزية
- 💾 **سجل المحادثات** - يحتفظ بسجل المحادثات ويعرضها
- ⚙️ **شخصية قابلة للتخصيص** - قم بتخصيص اسم البوت وسماته الشخصية
- 🎨 **واجهة حديثة** - واجهة نظيفة وسريعة الاستجابة مبنية بـ Streamlit
- 🔐 **معالجة آمنة للمفاتيح** - دعم متغيرات البيئة لمفاتيح API
- 📱 **تصميم سريع الاستجابة** - يعمل بسلاسة على أجهزة سطح المكتب والهواتف الذكية

## 🛠️ المكدس التقني

- **الخادم**: Python 3.8+
- **إطار العمل**: Streamlit
- **نموذج الذكاء الاصطناعي**: OpenAI API (GPT-3.5-turbo / GPT-4)
- **إدارة البيئة**: python-dotenv
- **إدارة المكتبات**: pip

## 📋 المتطلبات الأساسية

قبل تشغيل هذا المشروع، تأكد من أن لديك:

- Python 3.8 أو أحدث
- pip (مدير حزم Python)
- مفتاح OpenAI API (احصل عليه من [openai.com](https://platform.openai.com/api-keys))
- Git (لاستنساخ المستودع)

## 📥 التثبيت

### 1. استنسخ المستودع

```bash
git clone https://github.com/nadaelkholi29-beep/chatbot-.git
cd chatbot-
```

### 2. أنشئ بيئة افتراضية

```bash
# على Windows
python -m venv venv
venv\Scripts\activate

# على macOS/Linux
python3 -m venv venv
source venv/bin/activate
```

### 3. ثبت المكتبات المطلوبة

```bash
pip install -r requirements.txt
```

### 4. قم بتكوين متغيرات البيئة

أنشئ ملف `.env` في المجلد الجذر (استخدم `.env.example` كنموذج):

```bash
cp .env.example .env
```

عدّل `.env` وأضف مفتاح OpenAI API الخاص بك:

```env
OPENAI_API_KEY=sk-your-api-key-here
```

## 🚀 الاستخدام

### تشغيل التطبيق

```bash
streamlit run app.py
```

سيتم فتح التطبيق في متصفحك الافتراضي على `http://localhost:8501`

### استخدام البوت

1. **ابدأ الدردشة**: اكتب رسالتك في حقل الإدخال في الأسفل
2. **أرسل الرسالة**: اضغط Enter أو انقر على زر الإرسال
3. **عرض السجل**: جميع المحادثات معروضة في نافذة الدردشة
4. **مسح الدردشة**: استخدم الشريط الجانبي لبدء محادثة جديدة

### أمثلة التفاعل

**إنجليزي:**
```
المستخدم: Hello, what is artificial intelligence?
البوت: Artificial intelligence (AI) refers to computer systems...
```

**عربي:**
```
المستخدم: مرحبا، ما هو التعليم الآلي؟
البوت: التعليم الآلي (Machine Learning) هو فرع من فروع...
```

## ⚙️ التكوين

### متغيرات البيئة

يستخدم التطبيق متغيرات البيئة التالية:

| المتغير | الوصف | مطلوب |
|---------|-------|-------|
| `OPENAI_API_KEY` | مفتاح OpenAI API الخاص بك | نعم |
| `CHATBOT_NAME` | اسم البوت (الافتراضي: "AI Assistant") | لا |
| `MODEL_NAME` | نموذج OpenAI المستخدم (الافتراضي: "gpt-3.5-turbo") | لا |
| `TEMPERATURE` | إبداعية الاستجابة (0-2، الافتراضي: 0.7) | لا |
| `MAX_TOKENS` | الحد الأقصى لطول الاستجابة | لا |

### التخصيص

عدّل التكوين في `app.py`:

```python
CHATBOT_NAME = "اسم بوتك"
SYSTEM_PROMPT = "تعليماتك المخصصة هنا"
```

## 📁 هيكل المشروع

```
chatbot-/
├── app.py                 # تطبيق Streamlit الرئيسي
├── requirements.txt       # مكتبات Python المطلوبة
├── .env.example          # مثال متغيرات البيئة
├── README.md             # هذا الملف (إنجليزي)
├── README.ar.md          # التوثيق بالعربية
├── CONTRIBUTING.md       # دليل المساهمة
├── LICENSE               # ترخيص MIT
└── docs/                 # التوثيق والمقاطع
    └── screenshots/      # لقطات شاشة التطبيق
```

## 🤝 المساهمة

نرحب بالمساهمات! يرجى اتباع هذه الإرشادات:

1. **انسخ المستودع** (Fork)
2. **أنشئ فرعًا للميزة الجديدة** (`git checkout -b feature/amazing-feature`)
3. **قم بتأكيد التغييرات** (`git commit -m 'Add amazing feature'`)
4. **ادفع إلى الفرع** (`git push origin feature/amazing-feature`)
5. **افتح طلب دمج** (Pull Request)

للمزيد من الإرشادات، انظر [CONTRIBUTING.md](CONTRIBUTING.md)

## 🐛 المشاكل المعروفة

- حدود معدل API: لـ OpenAI API حدود معدل بناءً على خطتك
- وقت الاستجابة: قد يختلف بناءً على حمل API وتعقيد الاستجابة
- عرض النصوص العربية: تأكد من ترميز UTF-8 الصحيح في الطرفية

## 🔐 اعتبارات الأمان

- لا تقم بتأكيد ملف `.env` مع مفاتيح API الفعلية
- استخدم متغيرات البيئة للمعلومات الحساسة
- احتفظ بمفتاح OpenAI API الخاص بك خاصًا وآمنًا
- قم بتدوير مفاتيح API بانتظام
- راجع أفضل الممارسات الأمنية من OpenAI

## 📊 نصائح الأداء

- استخدم `gpt-3.5-turbo` للاستجابات الأسرع والتكاليف المنخفضة
- اضبط معامل `temperature` لاتساق الاستجابات
- راقب استخدام OpenAI API في لوحة التحكم
- ضع في الاعتبار تخزين مؤقت للاستجابات للأسئلة المتكررة

## 🔗 الموارد

- [توثيق Streamlit](https://docs.streamlit.io/)
- [توثيق OpenAI API](https://platform.openai.com/docs/)
- [توثيق Python](https://docs.python.org/3/)
- [توثيق Git](https://git-scm.com/doc)

## 📝 الترخيص

هذا المشروع مرخص تحت ترخيص MIT - انظر ملف [LICENSE](LICENSE) للتفاصيل.

## 👨‍💼 المؤلف

**ندى الخولي**
- GitHub: [@nadaelkholi29-beep](https://github.com/nadaelkholi29-beep)
- البريد الإلكتروني: nadaelkholi29@gmail.com

## 🙏 شكر وتقدير

- [OpenAI](https://openai.com/) على API GPT
- [Streamlit](https://streamlit.io/) على إطار العمل الرائع
- مساهمي المجتمع والداعمون

## 📧 الدعم

إذا واجهت أي مشاكل أو لديك أسئلة:

1. تحقق من [صفحة المشاكل](https://github.com/nadaelkholi29-beep/chatbot-/issues)
2. راجع ملف [CONTRIBUTING.md](CONTRIBUTING.md)
3. افتح مشكلة جديدة على GitHub بمعلومات مفصلة

---

**تم إنشاؤه بـ ❤️ لمجتمع الذكاء الاصطناعي**
