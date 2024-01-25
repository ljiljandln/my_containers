# containers

Реализация библиотеки containers.h.


### Part 1. Реализация библиотеки containers.h

Реализованы классы библиотеки `containers.h`  
Список классов: `list`, `map`, `queue`, `set`, `stack`, `vector`.
- Оформлено в виде заголовочного файла `containers.h`, который включает в себя другие заголовочные файлы с реализациями необходимых контейнеров (`list.h`, `map.h` и т.д.)
- Выполнено полное покрытие тестами
- `map` и `set` написаны на основе собственной реализации красно-черного дерева
- Сделан Makefile для тестов написанной библиотеки (с целями clean, test)


### Part 2. Дополнительно. Реализация библиотеки containersplus.h

- Реализованы функции библиотеки `containersplus.h`: `array`, `multiset`
- Выполнено полное покрытие тестами
- Написан Makefile для тестов написанной библиотеки (с целями clean, test)

### Part 3. Дополнительно. Реализация методов `insert_many`

Классы  дополнены соответствующими методами, согласно таблице:

| Modifiers      | Definition                                      | Containers |
|----------------|-------------------------------------------------| -------------------------------------------|
| `iterator insert_many(const_iterator pos, Args&&... args)`          | inserts new elements into the container directly before `pos`  | List, Vector |
| `void insert_many_back(Args&&... args)`          | appends new elements to the end of the container  | List, Vector, Queue |
| `void insert_many_front(Args&&... args)`          | appends new elements to the top of the container  | List, Stack |
| `vector<std::pair<iterator,bool>> insert_many(Args&&... args)`          | inserts new elements into the container  | Map, Set, Multiset |

