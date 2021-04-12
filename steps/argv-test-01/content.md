# Поют ли соловьи? 

В городском парке живут соловьи. Однако, их редко слышно, потому что они поют только когда температура на улице от 22 до 30 градусов в любое время года. Летом они поют при температуре от 15 до 35 градусов.

Напишите программу, которая определяет, поют в данный момент соловьи или нет.

Текущую температуру и время года программа должна брать из аргументов командной строки. А если их не передали — спрашивать у пользователя. 

**Например:**

```sh
$ ruby nightingales.rb 10 0
Сейчас соловьи молчат, греются или прохлаждаются :)
```

```sh
$ ruby nightingales.rb
Какая сейчас температура?
> 15
Какое время года? (0 - весна, 1 - лето, 2 - осень, 3 - зима)
> 1
Скорее идите в парк, соловьи поют!
```

<div class="rubyrush-task-hint">

Проверьте, указаны ли параметры `ARGV[0]` и `ARGV[1]`. Если указаны, берите их, если нет, спрашивайте у пользователя числа `STDIN.gets`-ом. И именно им, а не обычным `gets`-ом. 

Вспомните, как вы использовали вложенные `if` в прошлых примерах и заданиях. Для одновременной проверки нескольких условий в операторе `if` используйте логический оператор `&&`.

</div>


<div class="rubyrush-task-answer">


<ul>
<li><a href="https://github.com/aristofun/rubyrush-path/blob/master/steps/argv-test-01/solution/nightingales.rb" class="rubyrush-task-solution-link">Наш вариант решения</a></li></ul>

</div>