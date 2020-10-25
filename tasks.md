## Gettings started
Базовите условия на задачите за в хронологичен ред на материала. От друга страна допълнителните условия не са, допълнителните условия на една задача може да изискват повече знания от базовото условие в следваща задача.

---

## 1. comparison of digits

 Да се състави програма, която по въведено 4-цифренo естествено число в интервала [1000, 9999]формира 2 нови двуцифрени числа. 
*Първото* число се формира от **първата и четвъртата** цифра на въведеното число, а *второто* число се формира от **втората и третата** цифра.
На екрана да се изведе дали първото ново число e по-малко, равно или по-голямо от второто.
 
 | Input | Output |
 | --- | --- |
 | 3332 |  32 is less than 33 |
 | 1144 |  14 is equal to 14 |
 | 9875 |  85 is more than 87 |

 > tags: variables, flow-control, division operators
 ---

## 2. valid triangle
По въведени 3 цели положителни числа, определете дали те са валидни страни на триъгълник. Изведете на екрана информация за това. 

**Допълнително:** Добавете валидация на входа, при невалидни входни данни, изписвайте съобщение за грешка в конзолата.

 | Input | Output |
 | --- | --- |
 | 3 4 5 |  Triangle is valid. |
 | 1 2 128 |  Triangle is invalid. |
 | -12 3 5 |  Please enter positive numbers for the sides of the triangle. |

 > tags: variables, flow-control, comparisons, validation
 ---

 ## 3. is valid leap year
По въведена година, определете дали тя е високосна или не. Една година е високосна, ако се дели точно на 4, изключение правят годините, които се делят точно на 100. Но и тези години, които се делят точно на 400, също са високосни. 

**Допълнително:** Валидация на входа.

| Input | Output |
 | --- | --- |
 | 2020 | 2020 is a leap year. |
 | 2000 | 2000 is a leap year. |
 | 1600 | 1600 is a leap year. |
 | 1700 | 1700 is not a leap year. |
 | 2007 | 2007 is not a leap year. |
 | 1963 | 1963 is not a leap year. |
 | -202 | Jesus wasn't born yet :( |

 > tags: variables, same checks flow-control, comparisons, validation
 ---

  ## 4. find distance between two points
По въведени координати на две точки `A(x1, y1)` и `B(x2, y2)` в равнина, намерете дистанцията между тях.

**Допълнително:** Нека точките да са от тримерното пространство - `A(x1, y1, z1)` и `B(x2, y2, z2)` 

**Допълнително 2:** За начало на входа има 2 възможности: 
  * `a` - ако потребителят въведе буквата приемете, че ще се въведат 4 координати за двумерния случай и и намерет дистанцията
  * `b` - при въвеждане на `b` очаквайте 6 координати за тримерния случай и намерете дистанцията
  * Във всички други случай изпишете съобщение за грешка и прекратете програмата. **Бонус**: четете буква от конзолата докато потребителят не въведе `a` или `b`.

| Input | Output |
 | --- | --- |
 | 0 0 0 2 | The distance between A(0, 0) and B(0, 2) is 2. |
 | 0 0 1 1 | The distance between A(0, 0) and B(1, 1) is 1.41. |
 | 0 0 2 2 | The distance between A(0, 0) and B(2, 2) is 2.82. |

 | Input | Output|
 | --- | --- |
 | 0 0 0 0 0 2 | The distance between A(0, 0, 0) and B(0, 0, 2) is 2.82. |

 | Input | Output|
 | --- | --- |
 | a 0 0 2 2 | The distance between A(0, 0) and B(2, 2) is 2.82. |
 | b 0 0 0 0 0 2 | The distance between A(0, 0, 0) and B(0, 0, 2) is 2.82. |
 | c 0 0 2 2 | Please enter a valid value for dimensions: 'a' for 2D, 'b' for 3D |

 > tags: variables, flow-control, math

 > additional tags: functions, 3D distance, validation, loop-validation
 ---


## 5. member of a range
Въведете две числа `а` и `b`. Въведете трето число в интервала `[a, b]`.
 Ако е извън него, програмата да иска ново въвеждане, **докато числото не попадне в дадения интервал.**


 | Input | Output |
 | --- | --- |
 | 5 10 7 |  Success! |
 | 5 10 16 |  Please add a value in the interval [5, 10]. |

 > tags: variables, validation-loop
 ---

 ## 6. find letter casing
От конзолата се въвежда един символ, буква от английската азбука, изведете съобщения дали буквата е главна или малка.

**Допълнение:** Добавете проверка дали въведения символ наистина е буква. Ако не е, изведете съобщение за грешка и приключете програмата.

**Допълнение:** Превърнете единичната проверка в проверка, която прави ново запитване при въведен невалиден символ.

 | Input | Output |
 | --- | --- |
 | a |  'a' is lower case. |
 | B |  'B' is upper case. |
 | * |  '*' is not a letter. Shutting down... |
 | % |  '%' is not a letter. Please try again. |


 > tags: variables, ASCII, flow-control

 > additional tags: validation, loop-validation
 ---

 ## 7. change letter casing
От конзолата се въвежда един символ, буква от английската азбука, ако е малка буква, създайте голяма такава и изведете двете букви в конзолата. Ако е голямата, направете обратното.

**Допълнение:** Добавете проверка дали въведения символ наистина е буква. Ако не е, изведете съобщение за грешка и приключете програмата.

 | Input | Output |
 | --- | --- |
 | a |  You've entered 'a', the upper-case is 'A'. |
 | B |  You've entered 'B', the lower-case is 'a'. |
 | * |  '*' is not a letter. Shutting down... |


 > tags: variables, ASCII, flow-control, constants
 ---

