.. EN-Revision: none
.. _zend.progressbar.adapter.jspull:

Zend\ProgressBar_Adapter\JsPull
===============================

*Zend\ProgressBar_Adapter\JsPull* הוא ההפך מ jsPush, מאחר והוא מחפש ומושך אחר
עדכונים, במקום לדחוף עדכונים בחזרה לדפדפן. בדרך כלל תדרשו
להשתמש במתאם עם אפשרות קבוע של *Zend_ProgressBar*. בעת התראה, המתאם שולח
סטרינג מקודד ב JSON לדפדפן, שנראה בידיוק כמו הסטרינג שנשלח בעזרת
מתאם ה jsPush. ההבדל היחיד ביניהם הוא, שהוא מכיל פרמטר נוסף, *finished*
שיכול להיות או *false* כשנשלח *update()* או *true* כשנשלח *finish()*.

ניתן להגדיר את הגדרות המתאם בעזרת מתודות ה *set** או הזנת מערך או
מערך של *Zend_Config* עם הגדרות כפרמטר ראשון למתודה ההתחלתית של
המחלקה. ההגדרות האפשריות הן:

- *exitAfterSend*: יציאה מהבקשה הנוכחית אחרי שהמידע נשלח לדפדפן. ברירת
  המחדל היא *true*.


