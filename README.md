# Домашние задания по Kotlin

Этот репозиторий содержит домашние задания курса Kotlin для студентов ВШЭ и ИТМО.

## Процесс сдачи

1. Вы работаете над заданием в собственном форке этого репозитория.
2. По окончанию работы вы посылаете Pull Request с изменениями в этот репозиторий.
  - Формат названия пулл-реквеста: `Kotlin. ДЗ <номер задания>, <фамилия и имя сдающего>`
3. Преподаватель проверяет ваше решение и, возможно, оставляет замечения, которые вам необходимо исправить, а также оповещает вас об окончании проверки комментарием в пулл-реквесте.
4. После исправления всех замечаний вы оставляете комментарий в пулл-реквесте; далее либо повторяется пункт 3, либо, при отсутствии замечаний, решение засчитывается и выставляется оценка.
  - Решение не засчитывается если есть хотя бы одно неисправленное замечание

## Сроки сдачи

- Решение со всеми исправленными замечаниями: 1 неделя после дедлайна

## Что оценивается

- Соблюдение [общепринятых соглашений о форматировании кода](https://kotlinlang.org/docs/reference/coding-conventions.html)
- Отсутствие самоповторения
- Покрытие тестами (для заданий в которых необходимо самому придумать тесты)
- Читаемость кода

## Как сдавать домашние задания (в первый раз)

1. Сделайте форк этого репозитория. В дальнейшем вы будете работать с ним.
2. Склонируйте форк к себе на компьютер

  ```
  $ git clone <your-fork-url>
  ```
 
3. Выберите задание над которым вы собираетесь работать:

  ```
  $ git checkout <your-assignment-branch>
  ```

4. Сделайте задание. Обыкновенно от вас будет требоваться реализовать определенный интерфейс и, возможно, написать несколько тестов для него. Подробнее смотрите в README.mkdn в ветке задания.
5. Сохраните изменения и отправьте их на сервер:

  ```
  $ git commit -m <your-message>
  $ git push
  ```
Если вы посылаете ветку в первый раз, необходимо явно указать, что отправление идёт в ваш репозиторий:

  ```
  $ git push -u origin <your-assignment-branch>
  ```

6. Сделайте Pull Request в этот репозиторий. Проверьте, чтобы ветка в репозитории в которую вы делаете реквест совпадала с веткой задания над которым вы работали. О том, как сделать реквест написано [здесь](https://help.github.com/articles/creating-a-pull-request/).
7. При наличии падающих тестов или замечаний с нашей стороны повторите шаги 4 и 5, новый реквест делать не надо.

## Как сдавать домашние задания (в последующие разы)

1. У вас уже должен быть форк и клон форка на комьютере. Если нет, то воспользуйтесь инструкцией выше.
2. Проверьте, что git настроен на синхронизацию с этим репозиторием:

  ```
  $ git remote -v
  ```
  
  Если вывод этой команды содержит `upstream https://github.com/zarechenskiy/kotlin-course-se19`, то перейдите на шаг 4.
3. Настройте git на синхронизацию с этим репозиторием:

  ```
  $ git remote add upstream https://github.com/zarechenskiy/kotlin-course-se19
  ```
4. Обновите свой форк:

  ```
  $ git fetch upstream
  ```
5. Выполните шаги 3-7 из инструкции выше.
