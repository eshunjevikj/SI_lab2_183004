# **Втора лабораториска вежба по Софтверско инженерство**

## **Ева Шуњевиќ, бр. на индекс 183004**

### Група на код: 

Јас ја добив групата на код 4

### Control Flow Graph
![UntitledDiagram](https://user-images.githubusercontent.com/63502120/84577128-efaf0080-adb9-11ea-8911-a7c4075cd1bb.png)

### Функција:
![Screenshot_1](https://user-images.githubusercontent.com/63502120/84577165-2e44bb00-adba-11ea-921c-b55e8917d49d.png)

### Цикломатска комплексност: 
Цикломатската комплексност на овој код е 9, истата ја добив преку формулата E-N+2, каде што E е бројот на ребра, а N бројот на јазли.
Во случајoв 26-19+2=9, па цикломатската комплексност изнесува 9.

### Every path критериум тестови: 

EVERY PATH: 

1.ABRS

//Пример тест: Да не се иницијализира корисник


2.ABCRS

//Пример тест: Да се иницијализира корисник, но да нема корисничко име или лозинка


3.ABCDERS

//Пример тест: Да се иницијализира корисник со корисничко и лозинка, но лозинката е иста со корисничкото име
или должината на внесената лозинка е поголема од 8


4.ABCDEFGHJLNIHPRS

//Пример тест: Да се иницијализира корисник со корисничко и лозинка, но лозинката е иста со корисничкото име
или должината на внесената лозинка е поголема од 8, но лозинката да не содржи голема буква, специјален
карактер или цифра


5.ABCDEFGHJKLNIHPRS

//Пример тест: Да се иницијализира корисник со корисничко и лозинка, но лозинката е иста со корисничкото име
или должината на внесената лозинка е поголема од 8, и во самата лозинка да има барем една цифра


6.ABCDEFGHJKLMNIHPRS

//Пример тест: Да се иницијализира корисник со корисничко и лозинка, но лозинката е иста со корисничкото име
или должината на внесената лозинка е поголема од 8, и во самата лозинка има барем една цифра и барем една 
голема буква


7.ABCDEFGHJKLMNOIHPQRS

//Пример тест: Да се иницијализира корисник со корисничко и лозинка, но лозинката е иста со корисничкото име
или должината на внесената лозинка е поголема од 8, и во самата лозинка има барем една цифра, голема буква 
и специјален карактер


8.ABCDEFGHJLMNOIHPRS

 //Пример тест: Да се иницијализира корисник со корисничко и лозинка, но лозинката е иста со корисничкото име
или должината на внесената лозинка е поголема од 8, и во самата лозинка има барем еден специјален
карактер и барем една голема буква


9.ABCDEFGHJLMNIHPRS 

 //Пример тест: Да се иницијализира корисник со корисничко и лозинка, но лозинката е иста со корисничкото име
или должината на внесената лозинка е поголема од 8, и во самата лозинка има барем една голема буква


10.ABCDEFGHJLNOIHPRS

 //Пример тест: Да се иницијализира корисник со корисничко и лозинка, но лозинката е иста со корисничкото име
или должината на внесената лозинка е поголема од 8, и во самата лозинка има барем еден специјален
карактер


11.ABCDEFGHJKLNOIHPRS

//Пример тест: Да се иницијализира корисник со корисничко и лозинка, но лозинката е иста со корисничкото име
или должината на внесената лозинка е поголема од 8, и во самата лозинка има барем еден специјален
карактер и барем една цифра

### Every branch 

EVERY BRANCH

1.AB -> Преминот од поставување на специјалните карактери, до условот дека корисникот е инстанциран


2.BC -> Корисникот е инстанциран, се продолжува до условот дали се внесени корисничко име и лозинка


3.BR -> Корисникот не е инстанциран, се враќа false и се завршува целата функција. 


4.CD -> Корисникот е инстанциран, внесени се корисничко име и лозинка, се превзема лозинката
и се конвертираат сите букци во мали


5.CR -> Корисникот е инстанциран, но корисничкото име и лозинката не се валидни, се враќа 
false и се завршува целата функција.


6.DE -> По превземањето на лозинката во string променлива, повторно се оди до проверка дали
лозинката го содржи корсничкото име и која е нејзината големина


7.EF ->  Лозинката е валидна, се поставуваат променливите за бројка, голема буква или
специјален карактер на 0.


8.ER -> Лозинката или го содржи корисничкото име или не е доволно голема, се враќа false
и се завршува целата функција.


9.FG -> Се воведува нова променлива i=0 која е бројач во for циклус


10.GH -> Се проверува дали вредноста на новокреираната променлива е помала од должината
на лозинката


11.HP -> Вредноста на променливата i не е помала од должината на лозинката 
(изминати се сите букви од лозинката) и се продолжува до следниот услов.


12.HJ -> Вредноста на променливата i е помала од должината на лозинката, се проверува
дали i-тата буква во лозинката е број.


13.JK -> i-тата буква во лозинката е број, променливата за број се поставува на 1 (true)


14.JL -> i-тата буква во лозинката не е број, се оди до следниот услов кој е дали
i-тата буква во лозинката е голема буква


15.KL -> Поставена е вредноста на променливата за број на 1, се продолжува до следниот услов
дали i-тата буква во лозинката е голема буква


16.LM -> i-тата буква во лозинката е голема буква, променливата за голема
буква се поставува на 1 (true)


17.LN -> i-тиот карактер во лозинката не е голема буква, се оди до следниот услов кој е дали
i-тиот карактер во лозинката е специјален карактер


18.MN -> Поставена е вредноста на променливата за голема буква на 1, се продолжува до 
следниот услов дали i-тиот карактер во лозинката е специјален карактер


19.NO -> i-тиот карактер во лозинката е специјален карактер, се поставува вредноста на 
променливата за специјален карактер во 1 (true)


20.NI -> i-тиот карактер во лозинката не е специјален карактер, се врши инкрементирање на 
вредноста на променливата i (i+1)


21.OI -> Поставувена е вредноста на променливата за специјален карактер во 1 (true) , 
се врши инкрементирање на вредноста на променливата i (i+1)


23.IH -> По инкрементирањето на вредноста на i, повторно се проверува дали вредноста на оваа
променлива е помала од должината на лозинката. 


24.PR -> Вредностите на променливите за број, голема буква и специјален карактер не е 1 (true),
се враќа false и се завршува целата функција.


25.PQ -> Вредностите на променливите за број, голема буква и специјален карактер е 1 (true),
се враќа true.

26.RS -> Откако ќе се врати false или true, се завршува целата функција.  


