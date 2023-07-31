# Коспект: Роберт Мартин. Идеальный программист
The Clean Coder: A Code of Conduct for Professional Programmers" (2011)

## Профессионализм
Профессионализм = ответственность за свою работу.
#### Не вреди функциональности
- писать код с минимальным количеством ошибок
- Контроль качества не должен обнаружить проблем
- Проверить код так, чтобы быть уверенным, что он работает
- Покрывать код тестами
#### Не вреди структуре
- Код должен быть гибким
- Внесение изменений не должно приводить к непомерным затратам.
#### Обучение
Тратить 20 часов в неделю для учебы.
Разбираться в:
- паттернах проектирования
- принципах проектирования (SOLID)
- методологии (Scrum, Xp, Lean, kanban, каскадная разработка, структурный анализ, структурное проектирование)
- артефакты (UML, DFD, структурные диаграммы, сети Петри, диаграммы переходов, блок-схемы, таблицы решений)
##### Способы обучения
- решение простых задач
- совместная работа
- наставничество

## Трудовая этика
- Разбираться в предметной области
- Понимать интересы бизнеса, работодателя, заказчика
- Уметь говорить "нет" если цель не является достижимой (нереалистичные сроки)
- Стремится к оптимальному результату. Найти общую цель с заказчиком
- Не "пытаться" и не "пробовать" а ставить реальные задачи и сроки которые могут быть выполнены

Хороший код всегда можно писать если не отходить от своих принципов разработки и не соглашаться на "жертвы".

#### Язык обещаний
1. вы говорите что это сделаете
2. вы серьезно относитесь к своим словам
3. вы выполняете обещанное

Обещать можно только то что находится под полным контролем.

Как я могу проконтролировать выполнение обещания если оно не зависит только от меня?

Если обещание выполнить невозможно, можно пообещать выполнить конкретные действия для достижения цели.

Если есть признаки того что обещание может быть не выполнено - об этом стоит сообщить как можно раньше.

## Написание кода

- код должен работать
- соответствовать потребностям заказчика. Решать его задачу
- код должен хорошо вписываться в систему.
- нормально читаться другими программистами.

#### Готовность писать код
- не писать код ночью, в расстроенных чувствах, решить проблему связанную с тревожными мыслями
- избегать зоны потока (снижаются мыслительные способности, теряется общая картина)
- устранить помехи
- выспаться. Здоровый сон

Проблема: Творческий кризис (беспокойство, страх депрессия). Выход: парное программирование

Вдохновляться другим творчеством (чтение книг в других областях, поход в кино и т.д)

TDD помогает свести отладку к нулю.

Писать код в морафонском темпе. Вовремя останавливаться.

Худший вид нeпрофессионализма - попытка выдать недоделку за готовый продукт.

Помогать другим и принимать помощь.

## Разработка через тестирование

1. Новый код пишется после написания модульного теста который он не проходит.
2. Пишем такой объем модульного теста, какой необходим чтобы он не проходил.
3. Объем рабочего кода пишем столько, сколько необходимо чтобы тест проходил.

Разработка через тестирование приводит к более качественной архитектуре (приходится изолировать код для написания тестов).

#### Приемочные тесты
Тесты удовлетворяющие заказчика, которые как бы выполняются вручную. 
Автоматизация с помощью: Selenium, robot framework, cucumber

#### Модульные тесты (unit-тесты) 
В отличие от приемочных пишутся для программистов.

## Стратегии тестирования
Контроль качества не должен находить ошибки. Если контроль качества находит ошибку - разработчики 
должны спросить себя - что нужно сделать чтобы этого не случилось снова?

Требования со стороны бизнеса преобразуются в тесты

| тип               | название            | процент покрытия |
|-------------------|---------------------|------------------|
| исследовательские | исследовательские   | ~5%              |
| GUI               | Системные           | ~10%             |   
| API               | Интеграционные тесты | ~20%             |
| API               | Компонентные        | ~50%             |
| xUnit             | Модульные           | ~100%            |

**Модульные тесты** - тестирование ф-й, методов и т.д. Самый нижний уровень.

**Компонентные тесты** - тестирование компонентов, методов API

**Интеграционные тесты** - тестирование взаимодействия между компонентами.

**Системные тесты** - проверяют работу всей интегрированной системы, проверяют
что компоненты правильно связанны друг с другом (тесты производительности, пропускной способности).
Пишутся системным архитектором.

**Исследовательские тесты** - проходятся в ручную (день охоты за ошибками, попытки взлома, поиск странностей).

## Планирование

#### Встречи
* от бесполезных встреч можно отказаться
* если встреча идет не так как планировалось - с нее можно уйти

Эффективная встреча
* что я сделал вчера?
* что я буду делать сегодня?
* какие сложности мне предстоит решить?

#### Споры

Любые споры, которые не удается завершить за 5 минут, не может быть
решен обсуждением. Сила воли не может разрешить спор на продолжительное время.
Данные - могут.

#### Мана концентрации
Программирование - деятельность для которой необходима концентрация.

Сон - восстанавливает большую часть маны концентрации.

Кофеин - умеренные дозы повышают концентрацию. Слишком сильная доза
приводит к концентрации на малозначительных вещах.

Перезарядка. Отвлекающие занятия: прогулка, беседа с друзьями, взгляд из окна,
медитация, подкасты.

Физические упражнения.

#### Инверсия приоритетов
Если сердце не лежит к "решению задачи" - мы убеждаем себя что у нас есть более серьезна задача.
Такое поведение непрофессионально. Профессионал оценивает приоритет каждой
задачи и решает задачи в порядке приоритетов.

#### Тупики
Профессионал не увлекается идеей настолько, чтобы у него не хватило сил
отказаться от нее и вернуться к исходной точке.

#### Грязь, болота и трясины
Профессионалы следят за возможным возникновением грязи и вычищают ее при первых признака.
Движение вперед по грязи является худшим из инверсии приоритетов.

## Оценки
Оценка является предположением и не подразумевает обязательств.

Обязательство - нечто такое, что вы обязаны сделать. Обязательствам присуща определенность.
Нарушение обязательств обернется огромным ущербом для вашей репутации.

#### REPT
O - оптимистическая оценка (если все пройдет исключительно гладко).

N - номинальная оценка (наиболее вероятная).

P - пессимистическая оценка. С учетом всех возможных неприятностей.

u = O + 4N + P / 6 ожидаемая продолжительность задачи

Вероятностное распределение

G = P - O / 6 среднеквадратическое отклонение распределения времени выполнения задачи

### Широкополосный дельфийский метод (метод Delphi)
Группа экспертов собирается, обсуждает задачу и оценивает ее сложность.
Обсуждение и оценка повторяется до тех пор, пока не будет достигнуто согласие.

### Метод быстрого голосования
Задачи рассматриваются последовательно. Для каждой задачи проводится краткое обсуждение. 
Участники одновременно показывают оценку (от 0 до 5 пальцев).
Если оценки согласуются, участники переходят к следующей задаче. В противном случае они продолжают обсуждение,
чтобы определить причины расхождений.

### Аффинная оценка
Все задачи записываются на картах. Участники сортируют карты. Карты, которые занимают
больше времени - направо, а карты меньших задач - налево. 
Перемешанные более n раз карты откладываются для обсуждений.

На следующем этапе между картами рисуются линии, представляющие трудоемкость задачи в днях, неделях и т.д.

## Под давлением
Важно избежать принятие обязательств на сроки, в соблюдении которых вы не уверены.

Двигаться быстро - соблюдать чистоту в коде.

Во время кризисов не отклоняться от своих рабочих методов.

Спешка затягивает еще больше на дно. Притормозите и продумайте задачу.

Уведомить группу и начальство о неприятностях. Изложите план по выходу из кризиса. Обратитесь за информацией и советом.

Помощь, парное программирование.

## Сотрудничество
Одним из условий эффективной работы группы является профессиональное взаимодействие участников.

Первая обязанность профессионального программиста - заботиться об интересах своих работодателей.
Общаться с участниками группы, чтобы глубоко понимать коммерческие цели проекта.

Ваша работа - удерживать бизнес на плаву.

## Группы и проекты
Лучше формировать группы с постоянным составом которые переходят от одного проекта к другому.








