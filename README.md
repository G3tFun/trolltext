# trolltext
Troll text это библеотека на PyPI с помощью которой вы можете написать красивый шрифтом на ваш вкус!

Библиотека для преобразования текста в разные стили шрифтов Unicode.

## Как использовать

### 1. Установите библиотеку

```bash
pip install trolltext
```

---

### 2. Импортируйте функции

``` Python
from trolltext import style_text, allfont
```

---

### 3. Преобразование текста в выбранный стиль

``` Python
text = "Hello!"

# Преобразуем текст в жирный стиль
bold_text = style_text(text, "bold")
print(bold_text)
# Вывод: 𝗛𝗲𝗹𝗹𝗼!
```
##### ПРИМИЧАНИЕ! Шрифт применяется только к латиниским буквам!

---

### 4. Вывод текста во всех доступных стилях

```
print(allfont(text))
```

Результат будет примерно такой:

``` 
double_struck: 𝕥𝕖𝕩𝕥
bold: 𝘁𝗲𝘅𝘁
italic: 𝘵𝘦𝘹𝘵
bold_italic: 𝙩𝙚𝙭𝙩
script: 𝓉ℯ𝓍𝓉
fraktur: 𝔱𝔢𝔵𝔱
bold_script: 𝓽𝓮𝔁𝓽
bold_fraktur: 𝖙𝖊𝖝𝖙
monospace: 𝚝𝚎𝚡𝚝
circled: ⓣⓔⓧⓣ
```

---

### 5. Список доступных стилей (названия для параметра font)

double_struck
bold
italic
bold_italic
script
fraktur
bold_script
bold_fraktur
monospace
circled

6. Обработка ошибок

Если указать несуществующий стиль:

``` Python
text = "Hello!"

bold_text = style_text(text, "unknown_style")
print(bold_text)
```

Библиотека выдаст ошибку:

ValueError: Шрифт 'unknown_style' не найден.

----------

#### Created by G3tFun!

#### Copywriting without mentioning the author is prohibited!

#### This is my first library:)
