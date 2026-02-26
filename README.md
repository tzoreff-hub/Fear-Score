# 🚨 מדד הפחד הישראלי

דשבורד בזמן אמת המציג מדד פחד מורכב לישראל, המבוסס על נתונים חיים ממקורות מרובים.

## 🔗 [צפה בדשבורד החי](https://YOUR-USERNAME.github.io/fear-index/)

> החלף `YOUR-USERNAME` בשם המשתמש שלך ב-GitHub

-----

## 📊 מרכיבי המדד

|מרכיב           |משקל|מקור                                  |
|----------------|----|--------------------------------------|
|שוק הון ביטחוני |20% |stooq.com (ESLT, LMT, RTX, LDOS, KTOS)|
|מטבעות ומתכות   |20% |frankfurter.app + stooq (זהב, כסף)    |
|חיפושי מיגון    |18% |Google Trends RSS ישראל + ידני        |
|כותרות ביטחוניות|18% |ynet, walla, mako RSS                 |
|טיסות לישראל    |12% |OpenSky Network (LLBG)                |
|סקרי מפלגות     |12% |ממוצע ידני – מידגם, פאנלס, N12        |

-----

## 🛠️ עדכון נתונים ידניים

### סקרי מפלגות

ערוך את הקובץ `index.html` וחפש את `const POLLS` – עדכן את מספר המנדטים לפי הסקרים האחרונים.

מקורות מומלצים:

- [מעריב סקרים](https://www.maariv.co.il/elections)
- [הארץ בחירות](https://www.haaretz.co.il/news/elections)
- [Wikipedia סקרי כנסת 26](https://he.wikipedia.org/wiki/סקרי_הבחירות_לכנסת_ה-26)

### Google Trends

ערוך את `const TRENDS_DATA` – עדכן את הערכים (0–100) לפי:
[Google Trends ישראל](https://trends.google.com/trends/?geo=IL)

חפש: `ממד`, `מרחב מוגן`, `אזעקה`, `פיקוד העורף`

-----

## 🚀 פריסה ב-GitHub Pages

1. העלה את כל הקבצים ל-repository
1. עבור ל-**Settings → Pages**
1. בחר Branch: `main`, Folder: `/ (root)`
1. שמור – האתר יהיה זמין תוך ~60 שניות

-----

## ⚙️ APIs בשימוש (כולם חינמיים, ללא API key)

|API                                           |שימוש          |הגבלה        |
|----------------------------------------------|---------------|-------------|
|[stooq.com](https://stooq.com)                |מניות, זהב, כסף|ללא          |
|[frankfurter.app](https://frankfurter.app)    |שער דולר/שקל   |ללא          |
|[open.er-api.com](https://open.er-api.com)    |שער חלופי      |1500/חודש    |
|[OpenSky Network](https://opensky-network.org)|נתוני טיסות    |ללא (אנונימי)|
|[rss2json.com](https://rss2json.com)          |RSS → JSON     |10,000/יום   |
|[allorigins.win](https://allorigins.win)      |CORS proxy     |ללא          |

-----

## 📁 מבנה הקבצים

```
fear-index/
├── index.html      ← הדשבורד הראשי
└── README.md       ← קובץ זה
```

-----

*מדד הפחד הישראלי – פרויקט קוד פתוח*
