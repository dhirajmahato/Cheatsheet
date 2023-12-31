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
| ctrl+0 | hide column/row |
| **logical test**  |  |
|=FILTER(A2:A5, B2:B5 > 90)   |  filter A column based on condition on B column|
|=UNIQUE(A2:B100)  | Ctrl + Shift + Enter is essential when working with array formulas like UNIQUE that produce dynamic arrays   |
|=IF(A2>B2, Truecall, falsecall)   |  |
|=IF(A2>B2,  C2+D2, today() )  |  even have function within output | 
|=IF(A2>200, "best", IF(A2>100,"avg", "fail"))   | Nested IF - for making categorical field |
|=AND(D2>=0, D2<=100)   | returns TRUE and FALSE   |
|=NOT(B2)  | returns opposite   |
|=IFERROR(B2,"skipp this")  | if error "skipp this" text displays |
|=SUMIF(A2:A9, ">3", B2:B9)   | on condition put on column A summing over Column B  |
|=COUNTIF(A2:A9, ">3") | instead of summming , it find out count here  |
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
| =DATEDIF(start_date, end_date,"Y"/ "YM"/"MD") |  3 paramter gives the format of output |
| **Lookup Functions** |  |
| =VLOOKUP(lookup_value, table, col_index) similarily HLOOKUP)( -do-) |  It then returns a value in the same row from a column you specify.  |
| =XLOOKUP ( lookup_value (cell F2), lookup_array (range B2:B11), and return_array (range D2:D11)  )  | XLOOKUP uses a lookup array and a return array |
| **Count Functions**  |  |
| =COUNTIF(B2:B10, "Apple")  | count no of cell containing "Apple"  |
| =COUNTIFS(B2:B5, ">=90", C2:C5, ">=90") | condition on multiple columns |


