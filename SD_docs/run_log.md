## תיעוד הרצת הפרויקט

**מה עבד?**

- הפקודה `node --version` עבדה והחזירה `v22.12.0`.

**מה לא עבד?**

- הפקודה `npm install` נכשלה.
- התקבלה שגיאה שלפיה PowerShell אינו מאפשר הרצת סקריפטים.

**מה היה צריך לשנות כדי שיעבוד?**

- זיהיתי שהבעיה נובעת ממדיניות האבטחה של PowerShell ולא מהפרויקט.
- הפתרון שנבחר הוא להשתמש בפקודה `npm.cmd install` במקום `npm install`.

**מה למדתי?**

למדתי שלפעמים שגיאה בהרצת פרויקט נובעת מהגדרות סביבת העבודה ולא משגיאה בקוד עצמו.

`npm run test`
רץ בהצלחה
`npm run typecheck`
לא התגלו שגיאות
> event-photo-capstone@0.1.0 typecheck
> tsc --noEmit

`npm.cmd run dev`

> event-photo-capstone@0.1.0 dev
> tsx watch src/server.ts

Event Photo API listening on http://localhost:3000

