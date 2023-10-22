# Как пользоваться библиотекой?

Сайт: wdonate.ru
Автор питон библы: vk.com/id486001202

Для установки:
```
pip install wdonate
```

Сначало инициализируем класс:

```
from wdonate import wdonate
wd = wdonate('токен wdonate', group_id)
```

Методы к котором вы можете далее обратиться:

```
wd.getBalance() -> float - получение баланса
```

Получение ссылки для оплаты:
```
wd.getLink(user_id: int, amount: float = 0, payload: int = 0, pay_method: str = 'card') -> dict
```

получение списка последних донатов:
```
wd.getPayments(count: int = 0) -> dict
```

получение текущей url callback:
```
wd.getCallback() -> dict
```

установка url callback:
```
wd.setCallback(url: str) -> dict
```

удаление текущей url callbac
```
wd.delCallback() -> dict
```
