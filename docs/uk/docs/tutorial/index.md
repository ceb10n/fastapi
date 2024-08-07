# Туторіал - Посібник користувача

У цьому посібнику показано, як користуватися **FastAPI** з більшістю його функцій, крок за кроком.

Кожен розділ поступово надбудовується на попередні, але він структурований на окремі теми, щоб ви могли перейти безпосередньо до будь-якої конкретної, щоб вирішити ваші конкретні потреби API.

Він також створений як довідник для роботи у майбутньому.

Тож ви можете повернутися і побачити саме те, що вам потрібно.

## Запустіть код

Усі блоки коду можна скопіювати та використовувати безпосередньо (це фактично перевірені файли Python).

Щоб запустити будь-який із прикладів, скопіюйте код у файл `main.py` і запустіть `uvicorn` за допомогою:

<div class="termy">

```console
$ uvicorn main:app --reload

<span style="color: green;">INFO</span>:     Uvicorn running on http://127.0.0.1:8000 (Press CTRL+C to quit)
<span style="color: green;">INFO</span>:     Started reloader process [28720]
<span style="color: green;">INFO</span>:     Started server process [28722]
<span style="color: green;">INFO</span>:     Waiting for application startup.
<span style="color: green;">INFO</span>:     Application startup complete.
```

</div>

**ДУЖЕ радимо** написати або скопіювати код, відредагувати його та запустити локально.

Використання його у своєму редакторі – це те, що дійсно показує вам переваги FastAPI, бачите, як мало коду вам потрібно написати, всі перевірки типів, автозаповнення тощо.

---

## Встановлення FastAPI

Першим кроком є встановлення FastAPI.

Для туторіалу ви можете встановити його з усіма необов’язковими залежностями та функціями:

<div class="termy">

```console
$ pip install "fastapi[all]"

---> 100%
```

</div>

...який також включає `uvicorn`, який ви можете використовувати як сервер, який запускає ваш код.

/// note

Ви також можете встановити його частина за частиною.

Це те, що ви, ймовірно, зробили б, коли захочете розгорнути свою програму у виробничому середовищі:

```
pip install fastapi
```

Також встановіть `uvicorn`, щоб він працював як сервер:

```
pip install "uvicorn[standard]"
```

І те саме для кожної з опціональних залежностей, які ви хочете використовувати.

///

## Розширений посібник користувача

Існує також **Розширений посібник користувача**, який ви зможете прочитати пізніше після цього **Туторіал - Посібник користувача**.

**Розширений посібник користувача** засновано на цьому, використовує ті самі концепції та навчає вас деяким додатковим функціям.

Але вам слід спочатку прочитати **Туторіал - Посібник користувача** (те, що ви зараз читаєте).

Він розроблений таким чином, що ви можете створити повну програму лише за допомогою **Туторіал - Посібник користувача**, а потім розширити її різними способами, залежно від ваших потреб, використовуючи деякі з додаткових ідей з **Розширеного посібника користувача** .
