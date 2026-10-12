<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>AI Debate Lab</title>

<style>
* {
    box-sizing: border-box;
}

body {
    margin: 0;
    padding: 20px;
    font-family: Arial, sans-serif;
    background: #101827;
    color: white;
}

.container {
    max-width: 650px;
    margin: 30px auto;
}

h1 {
    text-align: center;
    color: #60a5fa;
}

.subtitle {
    text-align: center;
    color: #cbd5e1;
    line-height: 1.9;
}

.card {
    background: #1e293b;
    padding: 20px;
    border-radius: 16px;
    margin-top: 24px;
}

label {
    display: block;
    margin-bottom: 12px;
    font-weight: bold;
}

textarea {
    width: 100%;
    height: 140px;
    padding: 14px;
    border-radius: 10px;
    border: 1px solid #475569;
    background: #0f172a;
    color: white;
    font-size: 16px;
    resize: vertical;
}

button {
    width: 100%;
    padding: 15px;
    margin-top: 16px;
    background: #2563eb;
    color: white;
    border: none;
    border-radius: 10px;
    font-size: 17px;
    font-weight: bold;
    cursor: pointer;
}

button:active {
    background: #1d4ed8;
}

#result {
    margin-top: 20px;
    line-height: 2;
    white-space: pre-wrap;
}

.note {
    color: #94a3b8;
    font-size: 13px;
    line-height: 1.8;
}
</style>
</head>

<body>
<div class="container">

<h1>🧠 AI Debate Lab</h1>

<p class="subtitle">
آزمایشگاه همکاری هوش‌های مصنوعی<br>
دو ذهن مصنوعی، یک مسئله، راه‌حل‌های بهتر
</p>

<div class="card">

<label for="idea">موضوع یا ایده‌ات را بنویس:</label>

<textarea id="idea"
placeholder="مثلاً: چگونه می‌توانم یک کسب‌وکار موفق با سرمایه کم بسازم؟"></textarea>

<button onclick="startDebate()">
شروع همکاری هوش‌های مصنوعی
</button>

<div id="result"></div>

<p class="note">
نسخه آزمایشی رابط برنامه است.
برای گفت‌وگوی واقعی میان دو هوش مصنوعی،
باید در مرحله بعد اتصال امن به مدل‌های هوش مصنوعی را اضافه کنیم.
</p>

</div>
</div>

<script>
function startDebate() {
    const idea = document.getElementById("idea").value.trim();
    const result = document.getElementById("result");

    if (!idea) {
        result.textContent = "لطفاً ابتدا موضوع یا ایده‌ات را بنویس.";
        return;
    }

    result.textContent =
        "موضوع ثبت شد:\n\n" + idea +
        "\n\nمرحله بعد: اتصال هوش مصنوعی اول، " +
        "هوش مصنوعی دوم و سیستم نقد متقابل آن‌ها.";
}
</script>

</body>
</html>
