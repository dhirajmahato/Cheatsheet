## Excel basic commands

|Shortcut  | operations  |
|----------|-------------|
|Ctrl+E    | Flash fill |
|Ctrl+D    | down fill |
|Ctrl+R    | right fill |
|Ctrl+1    | formatting cell |
|Ctrl+space| select column of the active cell |
|Ctrl+shift+space| select whole data |
|Ctrl+shift++| create a new row/column|
| Ctrl + ` | shows the forlmula underneath|
| ctrl + [ | trace formula precedence |
| alt  | shows schortcuts |
| **logical test**  |  |
|=IF(A2>B2, Truecall, falsecall)   |  |
|=IF(A2>B2,  C2+D2, today() )  |  even have function within output | 
|=IF(A2>200, "best", IF(A2>100,"avg", "fail"))   | Nested IF - for making categorical field |
|=AND(D2>=0, D2<=100)   | returns TRUE and FALSE   |
|=NOT(B2)  | returns opposite   |
|=IFERROR(B2,"skipp this")  | if error "skipp this" text displays |
| **Text Functions**   |   |
| =TRIM(A2)   | eleminate the unnessary space   |
| =PROPER(A2)  | capitalise the 1st letter  of every word   |
| =UPPER(A2)or LOWER(A2)    | Capitalise the letters   |
| =LEN(A2)   | it count even the space in between  |
| =LEFT(A2, 3) or  =RIGHT(A2, 3) | returns the first 3 letter from left/ Right|
| =MID(A2, 3, 6) | returns the mid letters  |
| =CONCATENATE( A2, " ", B2)   | add two columns word  with a space in between|
| =FIND("m", A2) having value - Mumbai |   returns 3 - position no of the letter |
| **Date Functions**   |  |
|=TODAY(),=NOW(), =DAY()/ =MONTH() / =YEAR() |  |
| =EDATE(ref_date, num)   | addition and substraction with minus sign in num_value  |
| =NETWORKDAYS(start_date, end_date, holidays) | get the no of working days  |
| =DATEDIFF(start_date, end_date,"Y"/ "YM"/"MD") |  3 paramter gives the format of output |

