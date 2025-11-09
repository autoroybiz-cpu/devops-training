
# AutoRoy — DevOps Demo

אתר סטטי קטן שמדגים *CI/CD אמיתי*: שינוי בקוד ב-GitHub → פריסה אוטומטית ל-Render (Static Site).  
כולל גם אפשרות פריסה עם Docker (Web Service).

[![Deploy to Render](https://render.com/images/deploy-to-render-button.svg)](https://render.com)

*Live demo:* https://devops-training-3g38.onrender.com

---

* מה יש כאן
- 🔹 אתר סטטי (HTML/CSS) מעוצב
- 🔹 פריסה כ-*Static Site* על CDN (מהיר, לא “נרדם”)
- 🔹 קונפיג Docker פשוט ל-Nginx (לאתר סטטי/דמו Backend)
- 🔹 תהליך CI/CD: כל Commit ל-main → Deploy אוטומטי

---

* טכנולוגיות
- HTML5, CSS3
- Nginx (תצורת Docker בסיסית)
- GitHub + Render (Static Site / Web Service)

---

* מבנה הפרויקט
├── index.html
├── styles.css
├── favicon.ico
├── Dockerfile
└── .github/workflows/
* הפעלה מקומית
```bash
# Docker אופציונלי
docker build -t autoroy-devops-demo .
docker run -p 8080:80 autoroy-devops-demo
# http://localhost:8080
