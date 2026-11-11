# إزاي تستخدم Beity Store Marketing Workspace

## مهم جدًا: مفيش اشتراك Claude؟

**مش محتاج Claude Code CLI.**

الشغل عندك على مسارين:

| الأداة | تستخدمها في إيه |
|---|---|
| **Cursor** (اللي أنت فيه دلوقتي) | تشغيل workflows محليًا، كتابة كابشن، تقييم جروبات، تحديث ملفات البراند |
| **ChatGPT / ChatGPT Work** | التقارير اليومية/المسائية، القرارات، الداشبورد، المحادثات المستمرة |

ملفات الربط جاهزة في مجلد: `chatgpt-bridge/`

---

## 1) الاستخدام اليومي في Cursor

1. افتح المجلد: `X:\Beity-Store-Marketing-Agent`
2. افتح شات Agent في Cursor
3. اطلب شغل واضح، مثال:
   - `شغّل workflow 03 وقيّم جروبات الدلتا من evidence/groups-snapshot`
   - `اكتب كابشن فيسبوك بالعامية المصرية حسب workflow 06 — السعر UNKNOWN`
   - `اعمل خطة محتوى حسب workflow 05`

Cursor هيقرأ `CLAUDE.md` + `brand/` + `workflows/`.

---

## 2) ربط ChatGPT (الـ "Plugin" العملي)

ChatGPT مش بيتوصل بمجلد ويندوز لوحده. الطريقة الصحيحة:

### أ) ChatGPT Project / Custom GPT / ChatGPT Work
1. افتح ChatGPT → Project جديد باسم **Beity Store Marketing**
2. ارفع الملفات دي من `chatgpt-bridge/upload-pack/`:
   - `01_SYSTEM_INSTRUCTIONS.md` (حطه في Instructions)
   - باقي الملفات في Knowledge / Files
3. ابدأ الشات داخل الـ Project ده فقط لماركتنج بيتي ستور

### ب) كل يوم
- **Cursor**: ينفّذ بحث/مسودات/تقييم جروبات → يحفظ ناتج في ملف
- **ChatGPT**: ياخد الناتج ويعمل تقرير مسائي / قرارات / توصيات

---

## 3) إيه اللي متتعملش هنا

- تسجيل دخول Claude Code لو مفيش اشتراك
- نشر فيسبوك أوتوماتيك من المساحة دي
- اختراع أسعار أو أرقام مبيعات

النشر يفضل عبر مشروع Lakta الحالي: `X:\bytiey-face-agent`

---

## 4) خريطة سريعة للطلبات

| عايز تعمل | فين | قول إيه |
|---|---|---|
| تقييم جروبات | Cursor | workflow 03 |
| كابشن عربي | Cursor | workflow 06 |
| استراتيجية فيسبوك | Cursor | workflow 01 |
| تقرير يومي/مسائي | ChatGPT | استخدم Project + handoff |
| قرارات بيزنس | ChatGPT | بعد ما تاخد ناتج Cursor |

---

## 5) أول تجربة مقترحة (10 دقايق)

1. في Cursor: `لخّص brand/ وقول إيه UNKNOWN`
2. في Cursor: `شغّل workflow 03 على أول 20 جروب في الـ CSV`
3. انسخ الناتج لـ ChatGPT Project واطلب: `حوّل ده لتقرير فرص جروبات للدلتا`
