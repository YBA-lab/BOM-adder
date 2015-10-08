# BOM-adder
add UTF8 BOM (byte order mark) to all csv files in a folder

TODO: English Readme
<DIV 
style="WHITE-SPACE: normal; WORD-SPACING: 0px; TEXT-TRANSFORM: none; COLOR: rgb(34,34,34); FONT: small arial; WIDOWS: 1; LETTER-SPACING: normal; BACKGROUND-COLOR: rgb(255,255,255); TEXT-INDENT: 0px; -webkit-text-stroke-width: 0px; font-stretch: normal" 
dir=rtl>
יש בעיה עם עברית בקבצי CSV. זה לא משהו ייחודי לOS, אלא דפקט של הסטדנרטים שמתכנתים משתמשים בהם.
אם מנסים לפתוח את קובץ הנתונים באקסל אז התשובות המספריות יהיו בסדר, גם התשובות באנגלית, אבל התשובות בעברית יראו ככה:
</div>
<center>![screenshot](https://yba-lab.github.io/BOM-adder/img/image1.png)</center>
<DIV 
style="WHITE-SPACE: normal; WORD-SPACING: 0px; TEXT-TRANSFORM: none; COLOR: rgb(34,34,34); FONT: small arial; WIDOWS: 1; LETTER-SPACING: normal; BACKGROUND-COLOR: rgb(255,255,255); TEXT-INDENT: 0px; -webkit-text-stroke-width: 0px; font-stretch: normal" 
dir=rtl>
(זה אמור להיות 'זכר')
</div>

<DIV 
style="WHITE-SPACE: normal; WORD-SPACING: 0px; TEXT-TRANSFORM: none; COLOR: rgb(34,34,34); FONT: small arial; WIDOWS: 1; LETTER-SPACING: normal; BACKGROUND-COLOR: rgb(255,255,255); TEXT-INDENT: 0px; -webkit-text-stroke-width: 0px; font-stretch: normal" 
dir=rtl> כתבתי תוכנה קטנה שמתקנת את קבצי הנתונים. זו תוכנה מאוד פשוטה, ועל כן מאוד מסוכנת. היא עושה overwrite לקבצים, והיא לא תוודא אם אתם בטוחים שאתם רוצים לעשות את מה שאתם מבקשים ממנה.
כדי לעשות בה שימוש מושכל כדאי ליצור העתק של קובץ הנתונים בתיקייה נפרדת, ולכוון את התוכנה להעתק. אם בתיקייה הזו יש כמה קבצים היא תסדר את כולם, ותדווח את אילו קבצים היא תיקנה. אם לא קיבלתם דיווח שכולל את שמות הקבצים אז משהו לא עבד טוב.
אגב, התוכנה עובדת רק עם קבצי CSV.
</div>

<DIV 
style="WHITE-SPACE: normal; WORD-SPACING: 0px; TEXT-TRANSFORM: none; COLOR: rgb(34,34,34); FONT: small arial; WIDOWS: 1; LETTER-SPACING: normal; BACKGROUND-COLOR: rgb(255,255,255); TEXT-INDENT: 0px; -webkit-text-stroke-width: 0px; font-stretch: normal" 
dir=rtl>
*מדריך שימוש קצר:*
הרצה של הסקריפט (או גרסה מקומפלת שלו), תעלה את המסך הבא:
</div>
<center>![screenshot](https://yba-lab.github.io/BOM-adder/img/image2.png)</center>
<DIV 
style="WHITE-SPACE: normal; WORD-SPACING: 0px; TEXT-TRANSFORM: none; COLOR: rgb(34,34,34); FONT: small arial; WIDOWS: 1; LETTER-SPACING: normal; BACKGROUND-COLOR: rgb(255,255,255); TEXT-INDENT: 0px; -webkit-text-stroke-width: 0px; font-stretch: normal" 
dir=rtl>
כאן צריך לרשום את התיקייה שבה מופיע קובץ(ים) הנתונים שרוצים לתקן.
במקרה שלי הם מופיעים בתיקייה הזו:
</div>
<center>![screenshot](https://yba-lab.github.io/BOM-adder/img/image3.png)</center>

<DIV 
style="WHITE-SPACE: normal; WORD-SPACING: 0px; TEXT-TRANSFORM: none; COLOR: rgb(34,34,34); FONT: small arial; WIDOWS: 1; LETTER-SPACING: normal; BACKGROUND-COLOR: rgb(255,255,255); TEXT-INDENT: 0px; -webkit-text-stroke-width: 0px; font-stretch: normal" 
dir=rtl>הדרך הכי קלה לראות את שם התיקייה המלא היא ללחוץ על שורת הכתובת למעלה (מסומנת בתמונה),  (לא בטוח שזה יעבוד בכל הגרסאות של וינדוס)
</div>
<center>![screenshot](https://yba-lab.github.io/BOM-adder/img/image4.png)</center>

<DIV 
style="WHITE-SPACE: normal; WORD-SPACING: 0px; TEXT-TRANSFORM: none; COLOR: rgb(34,34,34); FONT: small arial; WIDOWS: 1; LETTER-SPACING: normal; BACKGROUND-COLOR: rgb(255,255,255); TEXT-INDENT: 0px; -webkit-text-stroke-width: 0px; font-stretch: normal" 
dir=rtl> בתוכנה שכתבתי אין אפשרות לעשות הדבק, אז צריך להקליד ידנית.
אין צורך להוסיף סלאש בסוף שם התיקייה.<br>
שימו לב להקליד נכון... <br>
</div>
<center>![screenshot](https://yba-lab.github.io/BOM-adder/img/image5.png)</center>

<DIV 
style="WHITE-SPACE: normal; WORD-SPACING: 0px; TEXT-TRANSFORM: none; COLOR: rgb(34,34,34); FONT: small arial; WIDOWS: 1; LETTER-SPACING: normal; BACKGROUND-COLOR: rgb(255,255,255); TEXT-INDENT: 0px; -webkit-text-stroke-width: 0px; font-stretch: normal" 
dir=rtl> מקישים אנטר, והתוכנה does it's magic.
תקבלו פלט עם כל שמות הקבצים שטופלו:
</div>
<center> ![screenshot](http://yba-lab.github.io/BOM-adder/img/image6.png) </center>


<DIV 
style="WHITE-SPACE: normal; WORD-SPACING: 0px; TEXT-TRANSFORM: none; COLOR: rgb(34,34,34); FONT: small arial; WIDOWS: 1; LETTER-SPACING: normal; BACKGROUND-COLOR: rgb(255,255,255); TEXT-INDENT: 0px; -webkit-text-stroke-width: 0px; font-stretch: normal" 
dir=rtl>
אם לא הופיעו שמות של קבצים והגעתם ישר להודעת הסיום, כנראה שיש טעות בשם התיקייה, או שאין בתיקייה הזו קבצים בסיומת CSV.
</div>
<br>

<DIV 
style="WHITE-SPACE: normal; WORD-SPACING: 0px; TEXT-TRANSFORM: none; COLOR: rgb(34,34,34); FONT: small arial; WIDOWS: 1; LETTER-SPACING: normal; BACKGROUND-COLOR: rgb(255,255,255); TEXT-INDENT: 0px; -webkit-text-stroke-width: 0px; font-stretch: normal" 
dir=rtl>
זו תוכנה פשוטה, ואין בה שום מנגנוני בטיחות/אזהרה; היא מאוד לא stupid-proof.
שימו לב להשתמש בה לפי הוראות השימוש...<br>
בהצלחה...
</div>
