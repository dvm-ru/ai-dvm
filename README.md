# AI-dvm
Расширение AI-dvm позволяет использовать нейросеть GigaChat прямо в Visual Studio Code.

https://developers.sber.ru/portal/products/gigachat-api
**Доступ к GigaChat API**

Примечание: для ввода команд используйте сочетание клавиш: Ctl+Shift+P
1. Чтобы начать использование, сначала получите доступ к GigaChat API, затем используя команду **AI-dvm Settings** введите строку авторизации в поле **GigaChat API authorization data**.
2. Когда вы хотите, чтобы нейросеть продолжила ваш код, используйте команду **AI-dvm Set Prompt** и введите запрос.
3. Затем нажмите **Alt + G**, чтобы сгенерировать код. Если все данные были введены правильно, в нижней части экрана появится сообщение **Done!**
4. Затем нажмите **Alt + Enter**, чтобы вводить результаты генерации по строкам.

### Настройки
- поле **Scope**: **GIGACHAT_API_PERS** - персональная версия, или **GIGACHAT_API_CORP** - для корпоративных версий.
- поле **Enter initial prompt**: первичная инструкция для нейросети. Ее можно изменить, например, так:
```
Ты - помощник в создании программного кода. После получения пояснений к коду, тебе будет отправлен сам код. Продолжай его, не добавляя ничего, кроме продолжения кода!
```

- поле **Max token limit**: максимальное количество токенов текста, которые будут использованы при генерации.
- поле **Lines depth limit**: по умолчанию 100 строк кода выше текущего положения курсора.