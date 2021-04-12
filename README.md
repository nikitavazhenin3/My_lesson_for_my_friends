## Как устроено
В папке `steps/` лежит линейный список «шагов».

Каждый шаг это урок с вложенными в него видосами и/или текстом, или ДЗ, 
или какой угодно mardkdown+html материал.

### Структура папок

`steps/<step_slug>/` — уникальное имя (идентификатор) шага. 

Шаги-ДЗ принято привязывать к соотв. уроку и нумеровать. 

Например после урока `steps/classes-inheritance` есть 2 ДЗ: `steps/classes-inheritance-01` и `steps/classes-inheritance-02`.


| Файл | Его смысл |
|----------------------|-----------------------------|
| `/<step_slug>/content.md` | основное тело шага |
| `/<step_slug>/links.json` | ссылки и материалы к шагу |
| `/<step_slug>/files/*` | файлы для материалов к уроку |
| `/<step_slug>/solution/*` | код с ответом на ДЗ |


### links.json

Отрывок из `steps/argv-test/links.json` — шаг-урок [про аргументы командной строки](https://github.com/aristofun/rubyrush/tree/master/steps/argv-test)

```json
{
  "help": [
    {
      "title": "Тест на логическое мышление",
      "url": "http://syntone.ru/psytesty/test-logicheskogo-myshleniya/"
    },
    {
      "title": "Тонкости работы с командной строкой Windows",
      "url": "http://habrahabr.ru/post/218759/"
    }
  ],
  "materials": [
    {
      "title": "Работа с аргументами запуска",
      "url": "arguments.rb"
    },
    {
      "title": "Тест на ревнивость",
      "url": "jealous_test.rb"
    }
  ]
}
```

### content.md

Содержит хорошо структурированный текст шага (урок или ДЗ). Может содержать вложенные по определенному формату видео и спец. блоки с ДЗ/подсказкой.
