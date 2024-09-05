# FNX-Interview-

Client side:
angular-searchRepo-app
השתמשתי ב- ANGULAR CLI 10
קובץ קונפיגורציה שמגדיר את כתובות של שירות ה- REST נמצא ב- assets\appConfig.js.


Server side:
SearchRepo.API

שירות NET CORE 3.1, השירות חושף 3 ENDPOINTS,
1. לצורך ביצוע חיפוש והחזרת גלרית לצד קליינט.
   לצורך ביצוע החיפוש ושימוש ב- API של ה- GITHUB היה צורך לייצר TOKEN, ייצרתי TOKEN והוא נמצא בקובץ appsettings לצורך שימוש בו בפניות לAPI שך GITHUB.
2. עדכון או סימון פריט BOOKMARK.
   על מנת ליישם את המנגנון, השתמשתי ב- IDistributedCache אשר מנהל את ה- SESSIONS ומאפשר החזרתם לקיינט על פי הצורך.
3. החזרת רשימת הפריטים שסומנו כ BOOKMARK.
כל ה- ENDPOINT מבצעים אימות JWT המגיע מהקליינט בהידר של הבקשות על ידי שימוש ב- FILTER (נמצא מעל ה- ENDPOINTS).
