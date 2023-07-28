# AppiumExtended  
An extension library for adding ease of use Appium-Python-Client  
  
Required to be installed appium cli with plugins: appium-device-farm, appium-dashboard.  
  
```
npm i -g appium@next  
appium driver install uiautomator2  
appium plugin install --source=npm appium-device-farm  
appium plugin install --source=npm appium-dashboard
```

## Метод: `connect(capabilities: dict)`

Метод `connect` выполняет подключение к устройству на основе заданных возможностей или свойств, передаваемых в формате словаря.

### Параметры

`capabilities`: Словарь, который содержит набор возможностей устройства, к которому производится подключение. Этот словарь может включать такие параметры, как имя устройства, версию операционной системы, путь к приложению и пр.

### Пример использования

```python
app = AppiumExtended()

capabilities_with_install = {  
"platformName": "android",  
"appium:automationName": "uiautomator2",  
"appium:deviceName": adb.get_device_model(),  
"appium:udid": adb.get_device_uuid(),  
"appium:app": self.path_to_apk,  
"appium:appPackage": self._package,  
"appium:appWaitActivity": self._activity_launchable,  
"appium: autoGrantPermissions": True,  
}

capabilities_without_install = {  
"platformName": "android",  
"appium:automationName": "uiautomator2",  
"appium:deviceName": adb.get_device_model(),  
"appium:udid": adb.get_device_uuid(),  
"appium:noReset": True,  
"appium: autoGrantPermissions": True,  
}

app.connect(capabilities=self.capabilities_without_install)
```

### Детали реализации

Метод включает следующие основные этапы:

1. Сохранение переданных возможностей в свойстве объекта `self.capabilities`.
2. Запуск локального сервера Appium, если не используется прокси и сервер ещё не запущен. Для запуска сервера используется задержка в 10 секунд, чтобы дать ему время для инициализации.
3. Инициализация драйвера `webdriver.Remote` с заданными возможностями и адресом сервера. Сохранение драйвера в свойстве объекта `self.driver`.
4. Инициализация объекта `AppiumImage` с созданным драйвером.
5. Запись в лог информации о подключении и номере сессии драйвера.

### Исключения

Метод не генерирует исключения напрямую, но может пробросить исключения, сгенерированные внутренними вызовами, такими как ошибка запуска сервера Appium или ошибки, связанные с `webdriver.Remote`.
		
	

## Метод: `disconnect()`

Метод `disconnect` отвечает за отключение от устройства. 

### Пример использования

```python
app.disconnect()
```

### Детали реализации

1. Проверка, установлен ли драйвер (`self.driver`). Если драйвер установлен, то выполняется его завершение с помощью метода `quit()` и затем драйвер обнуляется. В процессе выполнения этих операций в лог записывается информация о номере сессии, от которой происходит отключение.
2. Если не установлено значение `self.keep_alive_server`, то останавливается работа сервера с помощью метода `stop()`.

### Исключения

Метод не генерирует исключения напрямую, но может пробросить исключения, сгенерированные внутренними вызовами, например, при ошибке остановки сервера.


## Метод: `is_running()`

Метод `is_running` проверяет, активна ли текущая сессия драйвера.

### Возвращаемое значение

Возвращает `True` если текущая сессия драйвера активна, и `False` в противном случае.

### Пример использования

```python
if device.is_running():
    print("Устройство активно")
else:
    print("Устройство не активно")
```

### Исключения

Метод может генерировать исключения, в случае если `self.driver` не инициализирован. Также исключения могут быть сгенерированы внутренними вызовами метода `is_running` из объекта `self.driver`, например, при проблемах сети или сервера.


## Метод: `get_element(locator, by, value, timeout_elem, timeout_method, elements_range, contains)`

Этот метод обеспечивает поиск элемента в текущей структуре DOM. Метод должен получать либо локатор, либо значения `by` и `value`.

### Параметры

`locator`: Определяет локатор элемента. Это может быть:
- кортеж - локатор в виде ('атрибут', 'значение')
- объект WebElement
- словарь, содержащий пары атрибут: значение
- строка - путь до файла с изображением элемента.

`by`: Тип локатора для поиска элемента (всегда в связке с `value`). Может быть типом MobileBy, AppiumBy, By, или строкой.

`value`: Значение локатора или словарь аргументов, если используется AppiumBy.XPATH. Может быть строкой, словарём или `None`.

`timeout_elem`: Время ожидания элемента в секундах.

`timeout_method`: Время ожидания метода поиска элемента в секундах.

`elements_range`: Ограничивает поиск элемента в указанном диапазоне. Используется при поиске по изображению. Может быть кортежем, списком, словарём или `None`.

`contains`: Используется для поиска по словарю. Если `True`, ищет элемент, содержащий фрагмент значения.

### Возвращаемое значение

Возвращает объект WebElementExtended или `None`, если элемент не был найден.

### Пример использования

```python
element = app.get_element(locator=("id", "foo"))
element = app.get_element(element)
element = app.get_element(locator={'text': 'foo'})
element = app.get_element(locator='/path/to/file/pay_agent.png')
element = app.get_element(locator=part_image, elements_range={'class':'android.widget.FrameLayout', 'package':'ru.app.debug'})
element = app.get_element(by="id", value="ru.sigma.app.debug:id/backButton")
element = app.get_element(by=MobileBy.ID, value="ru.sigma.app.debug:id/backButton")
element = app.get_element(by=AppiumBy.ID, value="ru.sigma.app.debug:id/backButton")
element = app.get_element(by=By.ID, value="ru.sigma.app.debug:id/backButton")
```

### Исключения

Метод может генерировать исключения, в случае если введены некорректные аргументы или возникают ошибки при обработке элементов (например, `NoSuchElementException`, `TimeoutException` или `WebDriverException`).

## Метод: `get_elements(locator, by, value, timeout_elements, timeout_method, elements_range, contains)`

Этот метод обеспечивает поиск элементов в текущей структуре DOM. Метод может получать либо локатор, либо пару значений `by` и `value`.

### Параметры

- `locator`: Определяет локатор элементов. Это может быть:
  - Кортеж - локатор в виде ('атрибут', 'значение')
  - Список объектов WebElement
  - Словарь, содержащий пары атрибут: значение
  - Строка - путь до файла с изображением элемента.
- `by`: Тип локатора для поиска элемента (всегда используется в связке с `value`). Может быть типом MobileBy, AppiumBy, By, или строкой.
- `value`: Значение локатора или словарь аргументов, если используется AppiumBy.XPATH. Может быть строкой, словарём или `None`.
- `timeout_elements`: Время ожидания в секундах для появления каждого элемента.
- `timeout_method`: Общее время ожидания в секундах для выполнения всего метода.
- `elements_range`: Ограничивает поиск элементов в указанном диапазоне. Используется при поиске по изображению. Может быть кортежем, списком, словарём или `None`.
- `contains`: Используется для поиска по словарю. Если `True`, ищет элементы, содержащие фрагмент значения.

### Возвращаемое значение

Возвращает список объектов WebElementExtended, или `None`, если элементы не были найдены.

### Пример использования

```python
elements = app.get_elements(locator=("id", "foo"))
elements = app.get_elements(locator={'text': 'foo'})
elements = app.get_elements(locator='/path/to/file/pay_agent.png')
elements = app.get_elements(locator=part_image, elements_range={'class':'android.widget.FrameLayout', 'package':'ru.app.debug'})
elements = app.get_elements(by="id", value="ru.sigma.app.debug:id/backButton")
elements = app.get_elements(by=MobileBy.ID, value="ru.sigma.app.debug:id/backButton")
elements = app.get_elements(by=AppiumBy.ID, value="ru.sigma.app.debug:id/backButton")
elements = app.get_elements(by=By.ID, value="ru.sigma.app.debug:id/backButton")
```

### Исключения

Метод может генерировать исключения, в случае если введены некорректные аргументы или возникают ошибки при обработке элементов (например, `NoSuchElementException`, `TimeoutException` или `WebDriverException`).

## Метод: `get_image_coordinates(image, full_image, threshold)`

Этот метод находит координаты наиболее вероятного совпадения частичного изображения в полном изображении. Используется для поиска элементов или участков интерфейса на экране по изображению.

### Параметры

- `image`: Путь к файлу частичного изображения, которое нужно найти внутри полного изображения. Может быть байтами, массивом `np.ndarray`, объектом `Image.Image`, или строкой (путь к файлу).
    
- `full_image`: Путь к файлу полного изображения. Может быть байтами, массивом `np.ndarray`, объектом `Image.Image`, или строкой (путь к файлу). Если `None`, то будет использовано текущее скриншотное изображение.
    
- `threshold`: Минимальный порог совпадения, необходимый для считывания совпадения допустимым. По умолчанию равно 0.7.
    

### Возвращаемое значение

Возвращает кортеж с координатами наиболее вероятного совпадения в формате (x1, y1, x2, y2) или `None`, если совпадение не найдено.

### Пример использования

pythonCopy code

`coords = app.get_image_coordinates(image="/path/to/partial/image.png", full_image="/path/to/full/image.png", threshold=0.8)`

### Дополнительная информация

Этот метод использует декоратор `retry`, который выполняет функцию до тех пор, пока она не вернет результат, отличный от `None` или `False`, или пока не будет достигнуто максимальное количество попыток (3 попытки по умолчанию). После каждой неудачной попытки происходит пауза на 1 секунду.

pythonCopy code

`@retry def get_image_coordinates(...):     ...`

### Исключения

Метод может генерировать исключения при обработке изображений или при работе с файлами.



find_and_get_element


get_element_contains





get_elements_contains





get_inner_image_coordinates
	

get_many_coordinates_of_image
	

get_screenshot_as_base64_decoded
	

get_text_coordinates
	

input_by_virtual_keyboard
	

is_element_within_screen
	

is_image_on_the_screen
	

is_text_on_screen
	

swipe
	

swipe_bottom_to_top
	

swipe_left_to_right
	

swipe_right_to_left
	

swipe_top_to_bottom
	

tap
	

wait_for
	

wait_for_not
	

wait_return_true
	

draw_by_coordinates
	



