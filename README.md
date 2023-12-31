# AppiumExtended  

Представляем вам библиотеку расширения, которая значительно улучшает опыт использования Appium-Python-Client. С этой библиотекой вам будут доступны новые удобные функции и возможности, которые позволят более эффективно и легко автоматизировать ваши тесты. Позвольте вашим разработчикам сосредоточиться на более сложных задачах, а наша библиотека облегчит взаимодействие с Appium и сделает процесс автоматизации более приятным и эффективным. Дайте вашим приложениям возможность раскрыть свой полный потенциал с помощью этого интуитивного расширения Appium-Python-Client.

Требуется установить appium cli с плагинами: appium-device-farm, appium-dashboard.  
  
```
npm i -g appium@next  
appium driver install uiautomator2  
appium plugin install --source=npm appium-device-farm  
appium plugin install --source=npm appium-dashboard
```

# Содержание

### Класс `AppiumExtended`

- [connect](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-connect)
- [disconnect](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-disconnect)
- [is_running](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-is_running)
- [get_element](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-get_element)
- [find_and_get_element](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-find_and_get_element)
- [get_elements](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-get_elements)
- [get_image_coordinates](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-get_image_coordinates)
- [get_inner_image_coordinates](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-get_inner_image_coordinates)
- [get_many_coordinates_of_image](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-get_many_coordinates_of_image)
- [get_text_coordinates](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-get_text_coordinates)
- [get_screenshot_as_base64_decoded](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-get_screenshot_as_base64_decoded)
- [get_element_contains](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-get_element_contains)
- [get_elements_contains](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-get_elements_contains)
- [is_element_within_screen](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-is_element_within_screen)
- [is_text_on_screen](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-is_text_on_screen)
- [is_image_on_the_screen](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-is_image_on_the_screen)
- [tap](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-tap)
- [swipe](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-swipe)
- [swipe_top_to_bottom](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-swipe_top_to_bottom)
- [swipe_bottom_to_top](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-swipe_bottom_to_top)
- [swipe_right_to_left](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-swipe_right_to_left)
- [swipe_left_to_right](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-swipe_left_to_right)
- [wait_for](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-wait_for)
- [wait_for_not](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-wait_for_not)
- [wait_return_true](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-wait_return_true)
- [draw_by_coordinates](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-draw_by_coordinates)
- [input_by_virtual_keyboard](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-input_by_virtual_keyboard)

### Класс `WebElementExtended`

- [get_element](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-get_element-1)
- [get_attributes](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-get_attributes)
- [click](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-click)
- [double_click](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-double_click)
- [click_and_move](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-click_and_move)
- [adb_tap](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-adb_tap)
- [adb_multi_tap](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-adb_multi_tap)
- [adb_swipe](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-adb_swipe)
- [tap](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-tap-1)
- [double_tap](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-double_tap)
- [tap_and_move](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-tap_and_move)
- [get_elements](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-get_elements-1)
- [scroll_down](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-scroll_down)
- [scroll_up](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-scroll_up)
- [scroll_to_bottom](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-scroll_to_bottom)
- [scroll_to_top](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-scroll_to_top)
- [scroll_until_find](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-scroll_until_find)
- [get_parent](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-get_parent)
- [get_parents](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-get_parents)
- [get_sibling](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-get_sibling)
- [get_siblings](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-get_siblings)
- [get_cousin](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-get_cousin)
- [get_cousins](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-get_cousins)
- [is_contains](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-is_contains)
- [zoom](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-zoom)
- [unzoom](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-unzoom)
- [get_center](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-get_center)
- [get_coordinates](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-get_coordinates)

### Класс `AppiumServer`

- [start](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-start)
- [is_alive](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-is_alive)
- [stop](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-stop)
- [wait_until_alive](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-wait_until_alive)

### Класс `AppiumNavigator`

- [add_page](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-add_page)
- [navigate](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-navigate)
- [find_path](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-find_path)
- [perform_navigation](https://github.com/molokov-klim/appium_extended#%D0%BC%D0%B5%D1%82%D0%BE%D0%B4-perform_navigation)

Вы можете переходить по этим ссылкам для получения дополнительной информации о каждом методе.
# class AppiumExtended

## Метод: `connect()`

Метод `connect` выполняет подключение к устройству на основе заданных возможностей или свойств, передаваемых в формате словаря.

### Параметры

`capabilities`: Словарь, который содержит набор возможностей устройства, к которому производится подключение. Этот словарь может включать такие параметры, как имя устройства, версию операционной системы, путь к приложению и пр.

### Пример использования

```python
app = AppiumExtended()

capabilities_with_install = {  
"platformName": "android",  
"appium:automationName": "uiautomator2",  
"appium:deviceName": device_model,  
"appium:udid": device_uuid,  
"appium:app": path_to_apk,  
"appium:appPackage": package,  
"appium:appWaitActivity": activity_launchable,  
"appium: autoGrantPermissions": True,  
}

capabilities_without_install = {  
"platformName": "android",  
"appium:automationName": "uiautomator2",  
"appium:deviceName": device_model,  
"appium:udid": device_uuid,  
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


## Метод: `get_element()`

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

## Метод: `find_and_get_element()`

Этот метод используется для поиска элемента. Если элемент не найден, метод будет скроллить все скроллируемые элементы, пока не найдет искомый элемент или пока не будет проскроллено все доступное пространство.

### Параметры

- `locator` (Union[Tuple, WebElement, 'WebElementExtended', Dict[str, str], str]): Это местоположение или определение элемента, который нужно найти. Это может быть кортеж, экземпляр WebElement, словарь или строка.

- `timeout` (int, опционально): Это максимальное время ожидания для поиска элемента. По умолчанию это 10 секунд.

### Возвращаемое значение

Метод возвращает экземпляр `WebElementExtended`, если элемент найден. Если элемент не найден после прокрутки всей доступной страницы, возвращается `None`.

### Пример использования

```python
element = app.find_and_get_element(locator={'id': 'element_id'})
```

### Дополнительная информация

Внутри этого метода сначала проверяется, виден ли элемент на экране с помощью `is_element_within_screen()`. Если это так, то элемент возвращается с помощью `get_element()`.

Если элемент не виден на экране, то метод производит поиск во всех доступных для прокрутки элементах страницы. Если элемент найден в каком-то из этих элементов, он возвращается. Если элемент не найден после прокрутки всей доступной страницы, метод возвращает `None`.



## Метод: `get_elements()`

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


## Метод: `get_image_coordinates()`

Этот метод находит координаты наиболее вероятного совпадения частичного изображения в полном изображении. Используется для поиска элементов или участков интерфейса на экране по изображению.

### Параметры

- `image`: Путь к файлу частичного изображения, которое нужно найти внутри полного изображения. Может быть байтами, массивом `np.ndarray`, объектом `Image.Image`, или строкой (путь к файлу).
    
- `full_image`: Путь к файлу полного изображения. Может быть байтами, массивом `np.ndarray`, объектом `Image.Image`, или строкой (путь к файлу). Если `None`, то будет использовано текущее скриншотное изображение.
    
- `threshold`: Минимальный порог совпадения, необходимый для считывания совпадения допустимым. По умолчанию равно 0.7.
    

### Возвращаемое значение

Возвращает кортеж с координатами наиболее вероятного совпадения в формате (x1, y1, x2, y2) или `None`, если совпадение не найдено.

### Пример использования

```python
coords = app.get_image_coordinates(image="/path/to/partial/image.png", full_image="/path/to/full/image.png", threshold=0.8)
```

### Дополнительная информация

Этот метод использует декоратор `retry`, который выполняет функцию до тех пор, пока она не вернет результат, отличный от `None` или `False`, или пока не будет достигнуто максимальное количество попыток (3 попытки по умолчанию). После каждой неудачной попытки происходит пауза на 1 секунду.

### Исключения

Метод может генерировать исключения при обработке изображений или при работе с файлами.

## Метод: `get_inner_image_coordinates()`

Этот метод сначала находит изображение на экране (внешнее изображение), а затем находит другое изображение (внутреннее изображение) внутри обнаруженного изображения.

### Параметры

- `outer_image_path`: Путь к файлу с изображением, которое нужно найти на экране. Может быть байтами, массивом `np.ndarray`, объектом `Image.Image`, или строкой (путь к файлу).

- `inner_image_path`: Путь к файлу с изображением, которое нужно найти внутри внешнего изображения. Может быть байтами, массивом `np.ndarray`, объектом `Image.Image`, или строкой (путь к файлу).

- `threshold`: Пороговое значение сходства для шаблонного сопоставления. По умолчанию 0.9.

### Возвращаемое значение

Возвращает координаты внутреннего изображения относительно экрана в формате ((x1, y1), (x2, y2)). Если внутреннее изображение не найдено, возвращает `None`.

### Пример использования

```python
coords = app.get_inner_image_coordinates(outer_image_path="/path/to/outer/image.png", inner_image_path="/path/to/inner/image.png", threshold=0.8)
```

### Дополнительная информация

Этот метод использует декоратор `retry`, который выполняет функцию до тех пор, пока она не вернет результат, отличный от `None` или `False`, или пока не будет достигнуто максимальное количество попыток (3 попытки по умолчанию). После каждой неудачной попытки происходит пауза на 1 секунду.

### Исключения

Метод может генерировать исключения при обработке изображений или при работе с файлами.


## Метод: `get_many_coordinates_of_image()`

Этот метод находит все вхождения частичного изображения внутри полного изображения.

### Параметры

- `image`: Путь к файлу частичного изображения, которое нужно найти внутри полного изображения. Может быть байтами, массивом `np.ndarray`, объектом `Image.Image`, или строкой (путь к файлу).

- `full_image`: Путь к файлу полного изображения. Может быть байтами, массивом `np.ndarray`, объектом `Image.Image`, или строкой (путь к файлу). Если `None`, то будет сделан скриншот экрана и использован как полное изображение.

- `cv_threshold`: Минимальный порог совпадения, необходимый для считывания совпадения допустимым. По умолчанию равно 0.7.

- `coord_threshold`: Целое число, представляющее максимальное различие между значениями x и y двух кортежей, чтобы они считались слишком близкими друг к другу. По умолчанию равно 5.

### Возвращаемое значение

Возвращает список кортежей, содержащий расположение каждого найденного совпадения. Если совпадений не найдено, возвращается `None`.

### Пример использования

```python
matches = app.get_many_coordinates_of_image(image="/path/to/image.png", full_image="/path/to/full/image.png", cv_threshold=0.7, coord_threshold=5)
```

### Дополнительная информация

Этот метод использует декоратор `retry`, который выполняет функцию до тех пор, пока она не вернет результат, отличный от `None` или `False`, или пока не будет достигнуто максимальное количество попыток (3 попытки по умолчанию). После каждой неудачной попытки происходит пауза на 1 секунду.


### Исключения

Метод может генерировать исключения при обработке изображений или при работе с файлами.


## Метод: `get_text_coordinates()`

Этот метод возвращает координаты области, содержащей указанный текст на предоставленном изображении или снимке экрана. 

### Параметры

- `text`: Искомый текст.

- `language`: Язык для распознавания текста. По умолчанию 'rus'.

- `image`: Изображение, на котором осуществляется поиск текста. Может быть байтами, строкой (путь к файлу), объектом `Image.Image` или массивом `np.ndarray`. Если не указано, будет использован снимок экрана. По умолчанию `None`.

- `ocr`: Булев флаг, определяющий, следует ли использовать распознавание оптических символов (OCR) для извлечения текста из изображения. По умолчанию `True`.

### Возвращаемое значение

Возвращает кортеж из четырех целых чисел, представляющих координаты области с текстом (верхний левый угол и нижний правый угол). Если текст не найден, возвращается `None`.

### Пример использования

```python
coordinates = app.get_text_coordinates(text="Hello, world!", language="eng", image="/path/to/image.png", ocr=True)
```

### Дополнительная информация

Если флаг `ocr` установлен в `False`, метод будет использовать внутреннюю реализацию поиска элемента для извлечения координат области, содержащей искомый текст.


## Метод: `get_screenshot_as_base64_decoded()`

Этот метод возвращает текущий снимок экрана в браузере, декодированный из формата base64 в байты.

### Параметры

Метод не требует никаких параметров.

### Возвращаемое значение

Возвращает байты, представляющие снимок экрана. Эти байты могут быть использованы для создания изображения.

### Пример использования

```python
screenshot = app.get_screenshot_as_base64_decoded()
```

### Дополнительная информация

Этот метод используется внутри других методов класса для получения текущего снимка экрана при работе с изображениями.
	


## Метод: `get_element_contains()`

Этот метод пока не реализован. Ожидается, что он будет использоваться для поиска и возврата родительского элемента, который содержит определённый дочерний элемент.

### Параметры

На данный момент в методе нет параметров.

### Возвращаемое значение

На данный момент метод возвращает ошибку `NotImplementedError` при вызове, так как он ещё не реализован.

### Пример использования

```python
# Этот метод еще не реализован, поэтому его нельзя вызвать.
```

### Дополнительная информация

В текущей реализации метод возвращает исключение `NotImplementedError` с сообщением "This method is not implemented yet". Это означает, что метод ещё не реализован. Предполагается, что в будущем он будет реализован для поиска и возврата родительского элемента, содержащего определённый дочерний элемент.



## Метод: `get_elements_contains()`

Этот метод пока не реализован. Ожидается, что он будет использоваться для поиска и возврата всех родительских элементов, которые содержат определённые дочерние элементы.

### Параметры

На данный момент в методе нет параметров.

### Возвращаемое значение

На данный момент метод возвращает ошибку `NotImplementedError` при вызове, так как он ещё не реализован.

### Пример использования

```python
# Этот метод еще не реализован, поэтому его нельзя вызвать.
```

### Дополнительная информация

В текущей реализации метод возвращает исключение `NotImplementedError` с сообщением "This method is not implemented yet". Это означает, что метод ещё не реализован. Предполагается, что в будущем он будет реализован для поиска и возврата всех родительских элементов, содержащих определённые дочерние элементы.


## Метод: `is_element_within_screen()`

Этот метод проверяет, находится ли заданный элемент полностью на экране.

### Параметры

- `locator` (`Union[Tuple, WebElement, 'WebElementExtended', Dict[str, str], str]`): Локатор или элемент, который нужно проверить. Может быть кортежем, объектом WebElement, объектом WebElementExtended, словарем или строкой.
- `timeout` (`int`, необязательный): Время ожидания появления элемента в секундах. По умолчанию равно 10.

### Возвращаемое значение

- `bool`: Возвращает `True`, если элемент находится на видимой части экрана, и `False` в противном случае.

### Пример использования

```python
# Допустим, мы хотим проверить, находится ли элемент с id 'some_id' на видимой части экрана.
is_visible = app.is_element_within_screen(locator=('id', 'some_id'))
```

### Дополнительная информация

Метод сначала получает размеры экрана, затем ищет элемент с помощью предоставленного локатора. Если элемент не найден или не отображается, метод возвращает `False`. Если элемент найден и отображается, метод проверяет, находятся ли координаты элемента в пределах размеров экрана. Если элемент находится за пределами экрана, метод возвращает `False`. В противном случае, если элемент находится в пределах видимой области экрана, метод возвращает `True`.


## Метод: `is_text_on_screen()`

Этот метод проверяет, присутствует ли заданный текст на экране.

### Параметры

- `text` (`str`): Текст, который нужно найти на экране.
- `ocr` (`bool`, необязательный): Определяет, производить ли поиск текста на изображении или в DOM. Если `True`, распознавание текста производится с помощью библиотеки `pytesseract`. Если `False`, производится поиск элемента по xpath. Значение по умолчанию: `True`.
- `language` (`str`, необязательный): Язык для распознавания текста. По умолчанию 'rus'.

### Возвращаемое значение

- `bool`: Возвращает `True`, если заданный текст найден на экране. В противном случае возвращает `False`.

### Пример использования

```python
# Допустим, мы хотим проверить, находится ли текст 'Hello' на экране.
is_present = app.is_text_on_screen(text='Hello')
```

### Дополнительная информация

Метод использует разные подходы в зависимости от значения параметра `ocr`. Если `ocr=True`, то он использует библиотеку `pytesseract` для распознавания текста на изображении экрана. Если `ocr=False`, то он производит поиск элемента по xpath, используя текст как значение атрибута 'text' элемента.


## Метод: `is_image_on_the_screen()`

Этот метод сравнивает, присутствует ли заданное изображение на экране.

### Параметры

- `image` (`Union[bytes, np.ndarray, Image.Image, str]`): Изображение для поиска. Это может быть имя файла, байтовый поток, массив numpy или объект PIL Image.
- `threshold` (`float`, необязательный): Пороговое значение схожести части изображения со снимком экрана. По умолчанию 0.9.

### Возвращаемое значение

- `bool`: Возвращает `True`, если изображение найдено на экране. В противном случае возвращает `False`.

### Пример использования

```python
# Допустим, мы хотим проверить, находится ли изображение 'button.png' на экране.
is_present = app.is_image_on_the_screen(image='button.png')
```

### Дополнительная информация

Метод сначала делает снимок текущего экрана, затем преобразует его и искомое изображение в оттенки серого для лучшего сопоставления. Затем используется метод `cv2.matchTemplate` для сопоставления мелкого изображения и снимка экрана. Затем используется `cv2.minMaxLoc` для извлечения максимального коэффициента схожести и его координат. Если максимальное значение превышает заданный порог, метод возвращает `True`, в противном случае `False`.

## Метод: `tap()`

Этот метод выполняет действие "тап" или "клик" по определенным координатам, элементу или изображению на экране.

### Параметры

- `locator` (`Union[Tuple[str, str], WebElementExtended, WebElement, Dict[str, str], str]`, необязательный): Элемент или локатор, на который нужно нажать.
- `x` (`int`, необязательный): X координата точки, по которой следует нажать.
- `y` (`int`, необязательный): Y координата точки, по которой следует нажать.
- `image` (`Union[bytes, np.ndarray, Image.Image, str]`, необязательный): Изображение, на котором следует нажать.
- `duration` (`Optional[int]`, необязательный): Продолжительность нажатия в миллисекундах.
- `timeout` (`int`, необязательный): Время ожидания в секундах перед тем как метод вернет `None`, если изображение не найдено на экране. По умолчанию равно 5.

### Возвращаемое значение

- `Union['AppiumExtended', None]`: Возвращает экземпляр класса `AppiumExtended`, если действие "тап" или "клик" успешно выполнено. В противном случае возвращает `None`.

### Пример использования

```python
# Нажатие на элемент с указанным локатором
app.tap(locator=('id', 'button'))

# Нажатие по координатам
app.tap(x=100, y=200)

# Нажатие на изображение
app.tap(image='button.png')
```

### Дополнительная информация

Этот метод использует внутренний метод `_extract_point_coordinates_by_typing()` для получения координат точки, по которой следует нажать, если был передан `locator` или `image`. Если указано изображение, метод будет ожидать его появления на экране в течение указанного времени ожидания, прежде чем выполнить действие "тап". Затем вызывается внутренний метод `_tap()` для выполнения действия "тап" по заданным координатам.

## Метод: `swipe()`

Этот метод выполняет свайп (перетаскивание) элемента или изображения на экране.

### Параметры

- `start_position`: Позиция начала свайпа. Может быть задана в различных форматах:
  - Если `start_position` является кортежем и оба его элемента являются строками, то он представляет собой локатор элемента. В этом случае будет выполнен поиск элемента и используется его позиция.
  - Если `start_position` является словарем, то считается, что это локатор элемента, основанный на атрибутах. Например, {'text': 'some text'} или {'class': 'SomeClass', 'visible': 'true'}. В этом случае будет выполнен поиск элемента по указанным атрибутам, и используется его позиция.
  - Если `start_position` является экземпляром класса WebElement или WebElementExtended, то используется его позиция.
  - Если `start_position` является строкой, массивом байтов (bytes), массивом NumPy (np.ndarray) или объектом класса Image.Image, то считается, что это изображение. В этом случае будет вычислен центр изображения и используется его позиция.
  - Если `start_position` является кортежем, и оба его элемента являются целыми числами, то считается, что это координаты в формате (x_coordinate, y_coordinate).
- `end_position`: Позиция конца свайпа. Принимает те же форматы, что и `start_position`. По умолчанию None.
- `direction`: Направление свайпа. Принимает значения от 0 до 360 градусов. Если указано направление, то будет вычислена конечная точка свайпа на основе текущего размера окна и указанного расстояния. По умолчанию None.
- `distance`: Расстояние свайпа. Принимается в пикселях. Используется только в сочетании с параметром `direction`. По умолчанию None.
- `duration`: Продолжительность свайпа в миллисекундах. По умолчанию 0.

### Возвращаемое значение

- `AppiumExtended`: Экземпляр класса AppiumExtended.

### Примечания

- В качестве конечной позиции свайпа должен быть указан `end_position` или пара `direction, distance`.
- `str` принимается как путь к изображению на экране и вычисляется его центр, а не как локатор элемента

### Пример использования

```python
# Свайп элемента на экране по указанным координатам
app.swipe(start_position=(100, 200), end_position=(300, 400))

# Свайп по направлению и расстоянию
app.swipe(start_position=('xpath', '//button[@id="submit"]'), direction=90, distance=100)

# Свайп изображения
app.swipe(start_position='image.png', end_position=(300, 400))
```

### Дополнительная информация

Метод обязательно должен принимать либо end_postition, либо direction и distance

## Метод: `swipe_top_to_bottom()`

Этот метод выполняет свайп (перетаскивание) с верхней части экрана к нижней.

### Параметры

Метод не принимает параметров.

### Возвращаемое значение

- `None`

### Примечания

- Метод использует функцию `adb.get_screen_resolution()` для определения размера экрана.
- Позиция начала свайпа (`start_position`) вычисляется как 10% от высоты экрана.
- Позиция конца свайпа (`end_position`) вычисляется как 90% от высоты экрана.

### Пример использования

```python
# Свайп сверху вниз на экране
app.swipe_top_to_bottom()
```

## Метод: `swipe_bottom_to_top()`

Этот метод выполняет свайп (перетаскивание) с нижней части экрана к верхней.

### Параметры

Метод не принимает параметров.

### Возвращаемое значение

- `None`

### Примечания

- Метод использует функцию `adb.get_screen_resolution()` для определения размера экрана.
- Позиция начала свайпа (`start_position`) вычисляется как 90% от высоты экрана.
- Позиция конца свайпа (`end_position`) вычисляется как 10% от высоты экрана.
- Может использоваться для выдвигания шторки.

### Пример использования

```python
# Свайп снизу вверх на экране
app.swipe_bottom_to_top()
```


## Метод: `swipe_right_to_left()`

Этот метод выполняет свайп (перетаскивание) с правой части экрана к левой.

### Параметры

Метод не принимает параметров.

### Возвращаемое значение

- `None`

### Примечания

- Метод использует функцию `adb.get_screen_resolution()` для определения размера экрана.
- Позиция начала свайпа (`start_position`) вычисляется как 90% от ширины экрана.
- Позиция конца свайпа (`end_position`) вычисляется как 10% от ширины экрана.

### Пример использования

```python
# Свайп справа налево на экране
app.swipe_right_to_left()
```

## Метод: `swipe_left_to_right()`

Этот метод выполняет свайп (перетаскивание) с левой части экрана к правой.

### Параметры

Метод не принимает параметров.

### Возвращаемое значение

- `None`

### Примечания

- Метод использует функцию `adb.get_screen_resolution()` для определения размера экрана.
- Позиция начала свайпа (`start_position`) вычисляется как 10% от ширины экрана.
- Позиция конца свайпа (`end_position`) вычисляется как 90% от ширины экрана.

### Пример использования

```python
# Свайп слева направо на экране
app.swipe_left_to_right()
```


## Метод: `wait_for()`

Этот метод ожидает появления на экране указанного локатора или изображения.

### Параметры

- `locator`: Локатор(ы), которые нужно ожидать. Может быть одним локатором или списком локаторов. Принимает форматы, аналогичные `start_position` в методе `swipe()`. По умолчанию None.
- `image`: Изображение(я), которые нужно ожидать. Может быть одним изображением или списком изображений. Принимает строку, массив байтов (bytes), массив NumPy (np.ndarray) или объект класса Image.Image. По умолчанию None.
- `timeout`: Максимальное время ожидания в секундах. По умолчанию 10.
- `contains`: Если True, проверяет, содержит ли элемент указанный локатор. Если False, проверяет, точно ли соответствует элемент указанному локатору. По умолчанию True.
- `full_image`: Основное изображение, на котором будет искаться `image`. Принимает строку, массив байтов (bytes), массив NumPy (np.ndarray) или объект класса Image.Image. По умолчанию None.

### Возвращаемое значение

- `bool`: True, если элемент(ы) или изображение(я) найдены в течение периода ожидания, иначе False.

### Примечания

- Этот метод использует приватный метод `_wait_for()`, который реализует основную логику ожидания.

### Пример использования

```python
# Ожидание появления элемента по локатору
app.wait_for(locator=('xpath', '//button[@id="submit"]'), timeout=30)

# Ожидание появления изображения
app.wait_for(image='image.png', timeout=20)

# Ожидание появления нескольких элементов и изображений
app.wait_for(locator=[('id', 'button1'), ('id', 'button2')], image=['image1.png', 'image2.png'], timeout=40)
```


## Метод: `wait_for_not()`

Этот метод ожидает, пока указанный локатор или изображение не исчезнет с экрана или из DOM.

### Параметры

- `locator`: Локатор(ы), которые нужно ожидать. Может быть одним локатором или списком локаторов. Принимает форматы, аналогичные `start_position` в методе `swipe()`. По умолчанию None.
- `image`: Изображение(я), которые нужно ожидать. Может быть одним изображением или списком изображений. Принимает строку, массив байтов (bytes), массив NumPy (np.ndarray) или объект класса Image.Image. По умолчанию None.
- `timeout`: Максимальное время ожидания в секундах. По умолчанию 10.
- `contains`: Если True, проверяет, содержит ли элемент указанный локатор. Если False, проверяет, точно ли соответствует элемент указанному локатору. По умолчанию True.

### Возвращаемое значение

- `bool`: True, если элемент(ы) или изображение(я) исчезли в течение периода ожидания, иначе False.

### Пример использования

```python
# Ожидание исчезновения элемента по локатору
app.wait_for_not(locator=('xpath', '//button[@id="submit"]'), timeout=30)

# Ожидание исчезновения изображения
app.wait_for_not(image='image.png', timeout=20)

# Ожидание исчезновения нескольких элементов и изображений
app.wait_for_not(locator=[('id', 'button1'), ('id', 'button2')], image=['image1.png', 'image2.png'], timeout=40)
```


## Метод: `wait_return_true()`

Этот метод ожидает, когда другой метод вернет True.

### Параметры

- `method`: ссылка на метод, который мы ожидаем.
- `timeout`: максимальное время ожидания в секундах. По умолчанию равно 10.

### Возвращаемое значение

- `bool`: возвращает True, если метод возвращает True в течение периода времени, указанного в timeout. В противном случае возвращает False.

### Пример использования

```python
# Ожидаем, когда метод `check_login_status` вернет True в течение 20 секунд
result = AppiumExtended.wait_return_true(obj.check_login_status, timeout=20)

# Если `check_login_status` вернет True в течение 20 секунд, тогда `result` будет True, иначе `result` будет False.

app.wait_return_true(obj.is_connected, timeout=30)
```

Обратите внимание, что это статический метод, что означает, что он принадлежит классу, а не экземпляру класса. Это значит, что вам не нужен экземпляр класса, чтобы вызвать этот метод. Вы можете просто вызвать его на самом классе, как показано в примере выше.


## Метод: `draw_by_coordinates()`

Этот метод рисует прямоугольник на указанном изображении или скриншоте экрана. Прямоугольник задается координатами или верхней левой и нижней правой точками. Результирующее изображение сохраняется по указанному пути.

### Параметры

- `image`: Изображение, на котором будет рисоваться прямоугольник. Может быть представлено в форматах bytes, str (путь к файлу) или PIL Image. Если не указано, используется скриншот экрана. По умолчанию равно None.
- `coordinates`: Координаты прямоугольника в виде кортежа (x1, y1, x2, y2). По умолчанию равно None.
- `top_left`: Координаты верхней левой точки прямоугольника в виде кортежа (x, y). По умолчанию равно None.
- `bottom_right`: Координаты нижней правой точки прямоугольника в виде кортежа (x, y). По умолчанию равно None.
- `path`: Путь для сохранения результирующего изображения. По умолчанию равно None.

### Возвращаемое значение

- `AppiumExtended`: Возвращает экземпляр класса `AppiumExtended` для дальнейших вызовов методов.

### Пример использования

```python
appium_extended = AppiumExtended(driver)
image = driver.get_screenshot_as_base64().encode('utf-8')
appium_extended.draw_by_coordinates(image=image, coordinates=(123, 123, 123, 123), path='pictures')
```

В этом примере мы делаем скриншот экрана, рисуем на нем прямоугольник с указанными координатами и сохраняем полученное изображение в директории "pictures".


## Метод: `input_by_virtual_keyboard()`

Этот метод пока не реализован. Ожидается, что он будет использоваться для поиска и возврата родительского элемента, который содержит определённый дочерний элемент.

### Параметры

На данный момент в методе нет параметров.

### Возвращаемое значение

На данный момент метод возвращает ошибку `NotImplementedError` при вызове, так как он ещё не реализован.

### Пример использования

```python
# Этот метод еще не реализован, поэтому его нельзя вызвать.
```

### Дополнительная информация

В текущей реализации метод возвращает исключение `NotImplementedError` с сообщением "This method is not implemented yet". Это означает, что метод ещё не реализован. Предполагается, что в будущем он будет реализован для ввода данных с помощью виртуальной клавиатуры.


# class WebElementExtended

`WebElementExtended` - это класс, расширяющий базовый класс `WebElement` дополнительными возможностями. Он объединяет несколько классов, предоставляя различные методы взаимодействия с веб-элементами.

## Метод: `get_element()`

Этот метод извлекает элемент из другого элемента. Должен принимать как минимум либо локатор, либо значения параметров by и value.

### Параметры

- `locator`: Определяет локатор элемента. Может быть кортежем, WebElement, словарем или строкой.
    - Кортеж: Локатор в форме ('стратегия', 'значение'), например, ('xpath', '//*'), ('id', 'elem_id') и т.д.
    - WebElement / WebElementExtended: Объект веб-элемента.
    - Словарь: Содержит пары атрибут: значение элемента, например, {'text':'foo', 'enabled':'true'}.
    - Строка: Путь до файла с изображением элемента.
    - По умолчанию: None.
- `by`: Тип локатора для поиска элемента. Используется в связке с параметром `value`. Может быть MobileBy, AppiumBy, By или строкой. По умолчанию: None.
- `value`: Значение локатора или словарь аргументов, если используется AppiumBy.XPATH. Может быть строкой, словарем или None. По умолчанию: None.
- `timeout_elem`: Максимальное время ожидания элемента в секундах. По умолчанию: 10.
- `timeout_method`: Максимальное время ожидания выполнения метода поиска элемента в секундах. По умолчанию: 600.
- `elements_range`: Ограничивает поиск элемента в указанном диапазоне (для поиска по изображению). Может быть кортежем, списком, словарем или None. По умолчанию: None.
- `contains`: Если True, проверяет, содержит ли элемент указанные атрибуты. Если False, проверяет, точно ли соответствует элемент указанным атрибутам. По умолчанию: True.

### Возвращаемое значение

- `WebElementExtended` или `None`: Возвращает WebElementExtended, если элемент был найден в течение указанного времени ожидания, в противном случае возвращает None.

### Примечания

- Этот метод использует внутренний метод для реализации основной логики поиска элементов.

### Пример использования

```python
# Ожидание появления элемента по локатору
inner_element = element.get_element(locator=("id", "foo"), timeout_elem=30)

# Ожидание появления элемента по WebElement
inner_element = element.get_element(locator=element, timeout_elem=20)

# Ожидание появления нескольких элементов и изображений
inner_element = element.get_element(locator={'text': 'foo'}, elements_range={'class':'android.widget.FrameLayout', 'package':'ru.app.debug'}, timeout_elem=40)
```

## Метод: `get_attributes()`

Этот метод получает атрибуты элемента. Если хотя бы один из желаемых атрибутов не найден, метод возвращает все атрибуты элемента.

### Параметры

- `desired_attributes`: Список названий атрибутов, которые нужно получить. Если параметр не указан, метод вернет все атрибуты элемента. По умолчанию: None.

### Возвращаемое значение

- `dict`: Словарь, содержащий атрибуты элемента и их значения. Если указан `desired_attributes` и соответствующие атрибуты найдены у элемента, возвращает словарь только с запрашиваемыми атрибутами. Если `desired_attributes` не указан или желаемый атрибут не найден, возвращает словарь со всеми атрибутами.

### Пример использования

```python
# Получение атрибутов 'text', 'bounds', 'class' у элемента
attributes = element.get_attributes(['text', 'bounds', 'class'])

# Получение всех атрибутов элемента
all_attributes = element.get_attributes()
```

## Метод: `click()`

Этот метод осуществляет нажатие на заданный элемент.

### Параметры

- `duration`: Время нажатия в секундах. Если параметр равен нулю, осуществляется обычное нажатие, иначе происходит нажатие с удержанием на указанное количество секунд. По умолчанию равно 0.
- `decorator_args`: Параметры для декоратора, включая время ожидания нового окна (`timeout_window`) и количество попыток нажатия (`tries`). Используется только при `wait = True`. По умолчанию None.
- `wait`: Флаг, указывающий, следует ли ожидать изменения окна после нажатия. Если `True`, будет использован метод `_click_to_element_and_wait()`, иначе `_click_to_element()`. По умолчанию False.

### Возвращаемое значение

- Возвращает экземпляр `WebElementExtended`, представляющий элемент, на котором было произведено действие.
- В случае, если не удалось выполнить действие, генерируется AssertionError.

### Примечания

- В случае, если указан `wait = True` и не предоставлены `decorator_args`, используются стандартные параметры декоратора: `timeout_window` равно 5 и `tries` равно 5.

### Пример использования

```python
# Нажатие на элемент с ожиданием изменения окна и кастомными параметрами декоратора
decorator_args = {"timeout_window": 5, "tries": 5}
element.click(duration=0, wait=True, decorator_args=decorator_args)
```

## Метод: `double_click()`

Этот метод выполняет двойное нажатие (double click) на заданный элемент.

### Параметры

- `decorator_args`: Параметры для декоратора, включая время ожидания нового окна (`timeout_window`) и количество попыток нажатия (`tries`). Используется только при `wait = True`. По умолчанию `timeout_window` равно 5 и `tries` равно 5.
- `wait`: Флаг, указывающий, следует ли ожидать изменения окна после нажатия. Если `True`, будет использован метод `_double_click_to_element_and_wait()`, иначе `_double_click_to_element()`. По умолчанию False.

### Возвращаемое значение

- Возвращает экземпляр `WebElementExtended`, представляющий элемент, на котором было произведено действие.
- В случае, если не удалось выполнить действие, генерируется AssertionError.

### Примечания

- В случае, если указан `wait = True` и не предоставлены `decorator_args`, используются стандартные параметры декоратора: `timeout_window` равно 5 и `tries` равно 5.

### Пример использования

```python
# Двойное нажатие на элемент без ожидания изменения окна
element.double_click(wait=False)

# Двойное нажатие на элемент с ожиданием изменения окна и кастомными параметрами декоратора
decorator_args = {"timeout_window": 7, "tries": 3}
element.double_click(wait=True, decorator_args=decorator_args)
```

## Метод: `click_and_move()`

Этот метод нажимает левую кнопку мыши, перемещает курсор к указанной цели и отпускает кнопку.

### Параметры

- `locator`: Локатор для поиска целевого элемента на веб-странице. Он может быть кортежем, `WebElement`, `WebElementExtended`, словарем или строкой. Не обязательный параметр.
- `x`: Абсолютная координата по оси X для перемещения курсора. Не обязательный параметр.
- `y`: Абсолютная координата по оси Y для перемещения курсора. Не обязательный параметр.
- `direction`: Направление в градусах для перемещения курсора, где 0/360 - вверх, 90 - вправо, 180 - вниз, 270 - влево. Не обязательный параметр.
- `distance`: Расстояние в пикселях для перемещения курсора. Не обязательный параметр.

### Возвращаемое значение

- Возвращает экземпляр `WebElementExtended`, представляющий элемент, на котором было произведено действие.
- В случае, если не удалось выполнить действие, генерируется AssertionError.

### Пример использования

```python
# Кликнуть и переместить к элементу, найденному по локатору
element.click_and_move(locator="//button[@id='submit']")

# Кликнуть и переместить на указанные координаты
element.click_and_move(x=100, y=200)

# Кликнуть и переместить в указанном направлении на указанное расстояние
element.click_and_move(direction=90, distance=100)
```

### Примечание

Целью перемещения может быть WebElement, абсолютные координаты (x, y) или направление и расстояние. Если предоставлены направление и расстояние, функция вычисляет целевую позицию на основе вектора, определенного этими значениями. Если предоставлены абсолютные координаты (x, y), курсор перемещается в указанные позиции. Если предоставлен локатор, функция перемещается к найденному элементу на веб-странице.

## Метод: `adb_tap()`

Deprecated!
Метод устарел. Будет удален в следующих версиях.
Вместо него будет реализован метод выполняющий нажатие через driver.execute_script()

Этот метод выполняет нажатие на элемент, используя ADB (Android Debug Bridge).


### Параметры

- `decorator_args`: Дополнительные аргументы для использования в декораторе. Это словарь, который может содержать следующие ключи:
  - `timeout_window`: Время ожидания нового окна (умножается на количество попыток).
  - `tries`: Количество попыток нажатия (по умолчанию 3).
  Этот параметр не обязателен.
- `wait`: Флаг, указывающий, нужно ли ожидать изменения окна. Необязательный параметр, по умолчанию False.

### Возвращаемое значение

- Возвращает экземпляр `WebElementExtended`, представляющий элемент, на котором было произведено действие.
- В случае, если не удалось выполнить действие, генерируется AssertionError.

### Пример использования

```python
# Нажать на элемент с помощью ADB и не ожидать изменения окна
element.adb_tap()

# Нажать на элемент с помощью ADB и ожидать изменения окна
element.adb_tap(wait=True)

# Нажать на элемент с помощью ADB, ожидать изменения окна и установить время ожидания и количество попыток
element.adb_tap(decorator_args={"timeout_window": 5, "tries": 5}, wait=True)
```

### Примечание

ADB (Android Debug Bridge) - это инструмент командной строки, который используется для взаимодействия с устройством. В данном контексте он используется для симуляции взаимодействия пользователя с интерфейсом Android.

## Метод: `adb_multi_tap()`

Этот метод выполняет многократные нажатия (обычно два или три) на элемент, используя ADB (Android Debug Bridge). 

### Аргументы

- `decorator_args (dict, optional)`: Дополнительные аргументы для декоратора. Если `None`, то будут преобразованы в `decorator_args = {"timeout_window": 5, "tries": 5}`, где `timeout_window` - время ожидания изменения окна в секундах, а `tries` - количество попыток выполнения метода для изменения окна.
- `wait (bool, optional)`: Флаг, указывающий, нужно ли ожидать изменение окна после нажатия. По умолчанию `False`.

### Возвращаемое значение

- Возвращает экземпляр `WebElementExtended`, представляющий элемент, на котором было произведено действие.
- В случае, если не удалось выполнить действие, генерируется AssertionError.

### Пример использования

```python
# Выполнить многократные нажатия на элемент с помощью ADB
element.adb_multi_tap(decorator_args={"timeout_window": 10, "tries": 3}, wait=True)
```

### Примечание

ADB (Android Debug Bridge) - это инструмент командной строки, который используется для взаимодействия с устройством. В данном контексте он используется для симуляции взаимодействия пользователя с интерфейсом Android. Многократные нажатия могут быть полезны для выделения текста или активации специальных функций в приложении.

## Метод: `adb_swipe()`

Этот метод выполняет свайп (прокрутку) на элементе или по определенному направлению, используя ADB (Android Debug Bridge). 

### Аргументы

- `locator (Union[Tuple, WebElement, 'WebElementExtended', Dict[str, str], str], optional)`: Локатор элемента, к которому необходимо прокрутить. Это может быть `Tuple`, `WebElement`, `WebElementExtended`, словарь с `str` или просто `str`. Если `None`, прокрутка производится от центра корневого элемента. 
- `x (int, optional)`: Координата X целевой позиции прокрутки. 
- `y (int, optional)`: Координата Y целевой позиции прокрутки. 
- `direction (int, optional)`: Направление прокрутки в градусах (от 0 до 360). 
- `distance (int, optional)`: Расстояние прокрутки в пикселях. 
- `duration (int, optional)`: Длительность прокрутки в секундах. По умолчанию равна 1. 
- `contains (bool, optional)`: Флаг, указывающий, должен ли локатор содержать текст элемента. По умолчанию `True`.

### Возвращаемое значение

- Возвращает экземпляр `WebElementExtended`, представляющий элемент, на котором было произведено действие.
- В случае, если не удалось выполнить действие, генерируется AssertionError.

### Пример использования

```python
# Прокрутить до элемента с текстом "Submit"
element.adb_swipe(locator="Submit", duration=2)

# Прокрутить вниз на 500 пикселей за 1 секунду
element.adb_swipe(direction=180, distance=500, duration=1)
```

### Примечание

ADB (Android Debug Bridge) - это инструмент командной строки, который используется для взаимодействия с устройством. В данном контексте он используется для симуляции взаимодействия пользователя с интерфейсом Android. Прокрутка может быть полезной для навигации по странице или меню приложения.

## Метод: `tap()`

Этот метод выполняет нажатие (tap) на центре данного веб-элемента.

### Аргументы

- `duration (int, optional)`: Длительность нажатия в миллисекундах. По умолчанию равна 0 (моментальное нажатие). 
- `decorator_args (dict, optional)`: Дополнительные аргументы для использования в декораторе. По умолчанию равно `None`. Если необходимо ожидание результата после нажатия, в словаре можно указать "timeout_window" - время ожидания изменения окна, и "tries" - количество попыток для изменения окна.
- `wait (bool, optional)`: Флаг, указывающий, следует ли ожидать результат после нажатия. По умолчанию равно `False`.

### Возвращаемое значение

- Возвращает экземпляр `WebElementExtended`, представляющий элемент, на котором было произведено действие.
- В случае, если не удалось выполнить действие, генерируется AssertionError.

### Пример использования

```python
# Моментальное нажатие на элемент
element.tap()

# Нажатие на элемент на протяжении 500 миллисекунд
element.tap(duration=500)

# Нажатие на элемент с ожиданием изменения окна в течение 5 секунд
element.tap(duration=500, decorator_args={"timeout_window": 5, "tries": 5}, wait=True)
```

### Примечание

Методы `_tap`, `_tap_to_element_and_wait`, `_tap_to_element` и `__tap` используются внутри этого метода для выполнения нажатия и обработки различных сценариев, связанных с ожиданием результатов и обработкой исключений.

## Метод: `double_tap()`

Этот метод выполняет двойное нажатие (double tap) на центре данного веб-элемента.

### Аргументы

- `decorator_args (dict, optional)`: Дополнительные аргументы для использования в декораторе. По умолчанию равно `None`. Если необходимо ожидание результата после нажатия, в словаре можно указать "timeout_window" - время ожидания изменения окна, и "tries" - количество попыток для изменения окна.
- `wait (bool, optional)`: Флаг, указывающий, следует ли ожидать результат после нажатия. По умолчанию равно `False`.
- `pause (float, optional)`: Пауза между двумя нажатиями в секундах. По умолчанию равно 0.2.

### Возвращаемое значение

- Возвращает экземпляр `WebElementExtended`, представляющий элемент, на котором было произведено действие.
- В случае, если не удалось выполнить действие, генерируется AssertionError.

### Пример использования

```python
# Двойное нажатие на элемент с паузой в 0.3 секунды между нажатиями
element.double_tap(pause=0.3)

# Двойное нажатие на элемент с ожиданием изменения окна в течение 5 секунд
element.double_tap(decorator_args={"timeout_window": 5, "tries": 5}, wait=True, pause=0.3)
```

### Примечание

Методы `_double_tap`, `_double_tap_to_element_and_wait`, `_double_tap_to_element` и `__double_tap` используются внутри этого метода для выполнения двойного нажатия и обработки различных сценариев, связанных с ожиданием результатов и обработкой исключений.

## Метод: `tap_and_move()`

Этот метод выполняет операцию "нажать и переместить" на веб-элементе или на указанных координатах.

### Аргументы

- `locator (Union[Tuple, WebElement, 'WebElementExtended', Dict[str, str], str], optional)`: Локатор элемента, на который будет выполнено нажатие и перемещение. По умолчанию равно `None`.
- `x (int, optional)`: Координата X для нажатия и перемещения. По умолчанию равно `None`.
- `y (int, optional)`: Координата Y для нажатия и перемещения. По умолчанию равно `None`.
- `direction (int, optional)`: Направление перемещения в градусах (0 - вверх, 90 - вправо, 180 - вниз, 270 - влево). По умолчанию равно `None`.
- `distance (int, optional)`: Расстояние перемещения в пикселях. По умолчанию равно `None`.

### Возвращаемое значение

- Возвращает экземпляр `WebElementExtended`, представляющий элемент, на котором было произведено действие.
- В случае, если не удалось выполнить действие, генерируется AssertionError.

### Пример использования

```python
# Нажатие и перемещение на элемент с локатором
element.tap_and_move(locator=("xpath", "//div[@class='target']"))

# Нажатие и перемещение к координатам (50, 100)
element.tap_and_move(x=50, y=100)

# Нажатие и перемещение на расстояние 200 пикселей вниз
element.tap_and_move(direction=180, distance=200)
```

### Примечание

Метод `_tap_and_move` используется внутри этого метода для выполнения нажатия и перемещения, обработки различных сценариев в зависимости от предоставленных аргументов и обработки исключений.

## Метод: `get_elements()`

Этот метод обеспечивает поиск элементов в элементе.

### Аргументы

- `locator (Union[Tuple, List[WebElement], Dict[str, str], str], optional)`: Локатор элементов. Может быть кортежем, списком Веб-Элементов, словарем с атрибутом и значением, или строкой как путь до файла с изображением элемента. По умолчанию равно `None`.
- `by (Union[MobileBy, AppiumBy, By, str], optional)`: Тип локатора для поиска элемента (всегда в связке с `value`). По умолчанию равно `None`.
- `value (Union[str, Dict, None], optional)`: Значение локатора или словарь аргументов, если используется `AppiumBy.XPATH`. По умолчанию равно `None`.
- `timeout_elements (int, optional)`: Время ожидания для поиска каждого отдельного элемента. По умолчанию равно `10`.
- `timeout_method (int, optional)`: Общее время ожидания метода. По умолчанию равно `600`.
- `elements_range (Union[Tuple, List[WebElement], Dict[str, str], None], optional)`: Диапазон для поиска элементов. По умолчанию равно `None`.
- `contains (bool, optional)`: Если `True`, то поиск будет осуществляться по фрагменту текста или атрибута, а не их полному соответствию. По умолчанию равно `True`.

### Возвращаемое значение

- Возвращает список экземпляров `WebElementExtended`, представляющих найденные элементы. В случае, если элементы не найдены, возвращает пустой список.

### Пример использования

```python
# Поиск элементов по ID
elements = app.get_elements(locator=("id", "foo"))

# Поиск элементов по тексту
elements = app.get_elements(locator={'text': 'foo'})

# Поиск элементов по изображению
elements = app.get_elements(locator='/path/to/file/pay_agent.png')

# Поиск элементов с использованием типа локатора и значения
elements = app.get_elements(by="id", value="ru.sigma.app.debug:id/backButton")
```

## Метод: `scroll_down()`

Этот метод выполняет скроллинг элемента вниз. Тап и ведение от нижнего внутреннего элемента до верхнего внутреннего элемента.

### Аргументы

- `locator (Union[Tuple, WebElementExtended, Dict[str, str], str], optional)`: Локатор или элемент для прокрутки. Может быть кортежем, экземпляром `WebElementExtended`, словарем с атрибутом и значением, или строкой. Если не указан, то будет вычислен автоматически. По умолчанию равно `None`.
- `duration (int, optional)`: Продолжительность прокрутки в миллисекундах. Если не указана, прокрутка будет произведена без задержки. По умолчанию равно `None`.

### Возвращаемое значение

- Возвращает экземпляр `WebElementExtended`, если скроллинг выполнен успешно. 
- В случае, если не удалось выполнить действие, генерируется AssertionError.

### Пример использования

```python
# Скроллинг элемента с заданным локатором
app.scroll_down(locator=("id", "foo"), duration=1000)

# Скроллинг конкретного элемента
element = app.get_element(locator=("id", "foo"))
app.scroll_down(locator=element, duration=1000)

# Скроллинг элемента с заданным атрибутом и значением
app.scroll_down(locator={'class': 'foo'}, duration=1000)
```

## Метод: `scroll_up()`

Этот метод выполняет скроллинг элемента вверх.  Тап и ведение от верхнего внутреннего элемента до нижнего внутреннего элемента.

### Аргументы

- `locator (Union[Tuple, WebElementExtended, Dict[str, str], str], optional)`: Локатор или элемент для прокрутки. Может быть кортежем, экземпляром `WebElementExtended`, словарем с атрибутом и значением, или строкой. Если не указан, то будет вычислен автоматически. По умолчанию равно `None`.
- `duration (int, optional)`: Продолжительность прокрутки в миллисекундах. Если не указана, прокрутка будет произведена без задержки. По умолчанию равно `None`.

### Возвращаемое значение

- Возвращает экземпляр `WebElementExtended`, если скроллинг выполнен успешно. 
- В случае, если не удалось выполнить действие, генерируется AssertionError.

### Пример использования

```python
# Скроллинг элемента с заданным локатором вверх
app.scroll_up(locator=("id", "foo"), duration=1000)

# Скроллинг конкретного элемента вверх
element = app.get_element(locator=("id", "foo"))
app.scroll_up(locator=element, duration=1000)

# Скроллинг элемента с заданным атрибутом и значением вверх
app.scroll_up(locator={'class': 'foo'}, duration=1000)
```

## Метод: `scroll_to_bottom()`

Этот метод выполняет скроллинг элемента до самого нижнего положения.

### Аргументы

- `locator (Union[Tuple, WebElementExtended, Dict[str, str], str], optional)`: Локатор или элемент для прокрутки. Может быть кортежем, экземпляром `WebElementExtended`, словарем с атрибутом и значением, или строкой. По умолчанию равно `None`.
- `timeout_method (int, optional)`: Время ожидания выполнения метода в секундах. Если время ожидания истекает, а скроллинг не достигает нижнего положения, метод возвращает ошибку. По умолчанию равно `120`.

### Возвращаемое значение

- Возвращает экземпляр `WebElementExtended`, если скроллинг выполнен успешно. В случае ошибки выбрасывает исключение AsserionError.

### Пример использования

```python
# Скроллинг элемента с заданным локатором до нижнего положения
app.scroll_to_bottom(locator=("id", "foo"), timeout_method=120)

# Скроллинг конкретного элемента до нижнего положения
element = app.get_element(locator=("id", "foo"))
app.scroll_to_bottom(locator=element, timeout_method=120)

# Скроллинг элемента с заданным атрибутом и значением до нижнего положения
app.scroll_to_bottom(locator={'class': 'foo'}, timeout_method=120)
```

## Метод: `scroll_to_top()`

Этот метод выполняет скроллинг элемента до самого верхнего положения.

### Аргументы

- `locator (Union[Tuple, WebElementExtended, Dict[str, str], str], optional)`: Локатор или элемент для прокрутки. Может быть кортежем, экземпляром `WebElementExtended`, словарем с атрибутом и значением, или строкой. По умолчанию равно `None`.
- `timeout_method (int, optional)`: Время ожидания выполнения метода в секундах. Если время ожидания истекает, а скроллинг не достигает верхнего положения, метод возвращает ошибку. По умолчанию равно `120`.

### Возвращаемое значение

- Возвращает экземпляр `WebElementExtended`, если скроллинг выполнен успешно. В случае ошибки выбрасывает исключение AssertionError.

### Пример использования

```python
# Скроллинг элемента с заданным локатором до верхнего положения
app.scroll_to_top(locator=("id", "foo"), timeout_method=120)

# Скроллинг конкретного элемента до верхнего положения
element = app.get_element(locator=("id", "foo"))
app.scroll_to_top(locator=element, timeout_method=120)

# Скроллинг элемента с заданным атрибутом и значением до верхнего положения
app.scroll_to_top(locator={'class': 'foo'}, timeout_method=120)
```


## Метод: `scroll_until_find()`

Этот метод выполняет скроллинг элемента вниз и вверх, пока не найдет элемент, указанный в аргументе `locator`, или пока не истечет таймаут.

### Аргументы

- `locator (Union[Tuple, WebElementExtended, Dict[str, str], str])`: Локатор или элемент, который следует найти. Может быть кортежем, экземпляром `WebElementExtended`, словарем с атрибутом и значением, или строкой.
- `roll_locator (Union[Tuple, WebElementExtended, Dict[str, str], str], optional)`: Локатор или элемент, который следует прокручивать. Если не указан, прокручивается первый дочерний элемент. Может быть кортежем, экземпляром `WebElementExtended`, словарем с атрибутом и значением, или строкой. По умолчанию равно `None`.
- `timeout_method (int, optional)`: Время ожидания выполнения метода в секундах. Если время ожидания истекает, а элемент не найден, метод возвращает `None`. По умолчанию равно `120`.

### Возвращаемое значение

- Возвращает экземпляр `WebElementExtended`, если элемент найден. Возвращает `None`, если элемент не найден в течение заданного времени.

### Пример использования

```python
# Поиск элемента с заданным локатором, прокручивая элемент с другим локатором
app.scroll_until_find(locator=("id", "target"), roll_locator=("id", "foo"), timeout_method=120)

# Поиск конкретного элемента, прокручивая другой конкретный элемент
element_to_find = app.get_element(locator=("id", "target"))
element_to_scroll = app.get_element(locator=("id", "foo"))
app.scroll_until_find(locator=element_to_find, roll_locator=element_to_scroll, timeout_method=120)

# Поиск элемента с заданным атрибутом и значением, прокручивая элемент с другим атрибутом и значением
app.scroll_until_find(locator={'class': 'target'}, roll_locator={'class': 'foo'}, timeout_method=120)
```

## Метод: `get_parent()

Этот метод возвращает первый родительский элемент текущего элемента в дереве DOM.

### Аргументы

Метод не принимает никаких аргументов.

### Возвращаемое значение

- Возвращает экземпляр `WebElementExtended`, который представляет родительский элемент.

### Пример использования

```python
# Получение родительского элемента
parent_element = app.get_parent()
```

## Метод: `get_parents()

Этот метод возвращает все родительские элементы текущего элемента в дереве DOM, начиная от ближайшего и до корневого элемента.

### Аргументы

Метод не принимает никаких аргументов.

### Возвращаемое значение

- Возвращает список экземпляров `WebElementExtended`, каждый из которых представляет родительский элемент на различных уровнях вверх по дереву DOM.

### Пример использования

```python
# Получение всех родительских элементов
parent_elements = app.get_parents()
```

## Метод: `get_sibling()

Этот метод возвращает соседний (родственный) элемент текущего элемента, соответствующий заданным атрибутам. Возвращаются только непосредственные соседи (братья или сестры) в пределах того же родительского элемента.

### Аргументы

- `attributes` (`dict`): Словарь, содержащий атрибуты и их значения, которые должны быть найдены у искомого соседнего элемента. Например, `{'class': 'myClass', 'name': 'myName'}` ищет элемент, у которого атрибут `class` равен `myClass` и `name` равен `myName`.

- `contains` (`bool`, необязательный): Флаг, указывающий, использовать ли функцию `contains` XPath для атрибутов. Если `True`, метод будет искать элементы, значение атрибута которых содержит указанное значение (а не полное совпадение). По умолчанию равно `True`.

### Возвращаемое значение

- Возвращает экземпляр `WebElementExtended`, представляющий найденный соседний элемент. Если такой элемент не найден, возвращается `None`.

### Пример использования

```python
# Получение соседнего элемента с классом 'myClass'
sibling_element = app.get_sibling({'class': 'myClass'})

# Получение соседнего элемента, имя которого содержит 'myName'
sibling_element = app.get_sibling({'name': 'myName'}, contains=True)
```

## Метод: `get_siblings()

Этот метод возвращает все соседние (родственные) элементы текущего элемента. Возвращаются только непосредственные соседи (братья или сестры) в пределах того же родительского элемента.

### Аргументы

Метод не требует аргументов.

### Возвращаемое значение

- Возвращает список экземпляров `WebElementExtended`, каждый из которых представляет одного из родственных элементов текущего элемента. Если таких элементов не найдено, возвращается пустой список.

### Пример использования

```python
# Получение всех соседних элементов текущего элемента
sibling_elements = app.get_siblings()
```

## Метод: `get_cousin()

Этот метод предназначен для поиска "кузена" текущего элемента в дереве DOM. Кузен в данном контексте определяется как элемент, находящийся на одинаковом уровне вложенности от общего предка.

### Аргументы

- `ancestor` - Предок, относительно которого определяется "кузенство". Может быть представлен в виде кортежа (списка атрибутов и их значений), экземпляра WebElement или WebElementExtended, словаря (атрибутов и их значений) или строки (XPath выражения).

- `cousin` - Словарь атрибутов, определяющий искомого кузена. Ключи словаря - это названия атрибутов, значения - соответствующие значения этих атрибутов.

- `contains` - Булевый флаг, который определяет, следует ли использовать функцию `contains` при формировании XPath выражения для поиска кузена. Если `True`, то будет искаться частичное совпадение атрибутов. Если `False`, то будет искаться полное совпадение. По умолчанию `True`.

### Возвращаемое значение

- Возвращает экземпляр `WebElementExtended`, представляющий кузена текущего элемента. Если кузен не найден, возвращается `None`.

### Пример использования

```python
# Ищем кузена текущего элемента, имеющего класс 'desired-class' и находящегося на одинаковой глубине вложенности от общего предка с классом 'parent-class'
cousin_element = app.get_cousin(ancestor={'class': 'parent-class'}, cousin={'class': 'desired-class'})
```

## Метод: `get_cousins()

Этот метод предназначен для поиска "кузенов" текущего элемента в дереве DOM. Кузен в данном контексте определяется как элемент, находящийся на одинаковом уровне вложенности от общего предка.

### Аргументы

- `ancestor` - Предок, относительно которого определяется "кузенство". Может быть представлен в виде кортежа (списка атрибутов и их значений), экземпляра WebElement или WebElementExtended, словаря (атрибутов и их значений) или строки (XPath выражения).

- `cousin` - Словарь атрибутов, определяющий искомого кузена. Ключи словаря - это названия атрибутов, значения - соответствующие значения этих атрибутов.

- `contains` - Булевый флаг, который определяет, следует ли использовать функцию `contains` при формировании XPath выражения для поиска кузенов. Если `True`, то будет искаться частичное совпадение атрибутов. Если `False`, то будет искаться полное совпадение. По умолчанию `True`.

### Возвращаемое значение

- Возвращает список экземпляров `WebElementExtended`, представляющих кузенов текущего элемента. Если кузены не найдены, возвращается пустой список.

### Пример использования

```python
# Ищем кузенов текущего элемента, имеющих класс 'desired-class' и находящихся на одинаковой глубине вложенности от общего предка с классом 'parent-class'
cousin_elements = app.get_cousins(ancestor={'class': 'parent-class'}, cousin={'class': 'desired-class'})
```

## Метод: `is_contains()

Этот метод проверяет, содержит ли текущий элемент другой элемент, определенный локатором `locator`. 

### Аргументы

- `locator` - Локатор дочернего элемента. Может быть представлен в виде кортежа (списка атрибутов и их значений), экземпляра WebElement или WebElementExtended, словаря (атрибутов и их значений) или строки (XPath выражения).

- `contains` - Булевый флаг, который определяет, следует ли использовать функцию `contains` при формировании XPath выражения для поиска элемента. Если `True`, то будет искаться частичное совпадение атрибутов. Если `False`, то будет искаться полное совпадение. По умолчанию `True`.

### Возвращаемое значение

- Возвращает `True`, если текущий элемент содержит искомый дочерний элемент, и `False` в противном случае.

### Пример использования

```python
# Проверяем, содержит ли текущий элемент дочерний элемент с классом 'child-class'
if app.is_contains(locator={'class': 'child-class'}):
    print("Child element is present")
else:
    print("Child element is not present")
```

## Метод: `zoom()`

Вызывает `NotImplementedError` так как метод не реализован.
Этот метод в будущем реализует функцию увеличения (zoom) на элементе страницы.

### Аргументы

- `hold` - Булевый параметр, который определяет, следует ли удерживать увеличение после его выполнения. Если `True`, увеличение будет удерживаться. Если `False`, увеличение не будет удерживаться после выполнения действия.

### Возвращаемое значение

- Вызывает `NotImplementedError` так как метод не реализован.

### Пример использования

```python
Метод не реализован
```

## Метод: `unzoom()`

Вызывает `NotImplementedError` так как метод не реализован.
Этот метод в будущем реализует функцию увеличения (zoom) на элементе страницы.

### Аргументы

- `hold` - Булевый параметр, который определяет, следует ли удерживать увеличение после его выполнения. Если `True`, увеличение будет удерживаться. Если `False`, увеличение не будет удерживаться после выполнения действия.

### Возвращаемое значение

- Вызывает `NotImplementedError` так как метод не реализован.

### Пример использования

```python
Метод не реализован
```

## Метод: `get_center() 

Этот метод вычисляет координаты центра текущего элемента страницы.

### Возвращаемое значение

- Возвращает кортеж в формате `(x, y)`, где `x` и `y` - это координаты центра элемента. Если во время выполнения произошла ошибка, метод вернёт `None`.

### Пример использования

```python
# Получаем координаты центра элемента
center_coordinates = element.get_center()

# Печатаем координаты центра
if center_coordinates is not None:
    print("The center of the element is located at: ", center_coordinates)
else:
    print("An error occurred while getting the center of the element.")
```

## Метод: `get_coordinates()

Этот метод используется для получения координат текущего элемента веб-страницы.

### Возвращаемое значение

- Возвращает кортеж в формате `(left, top, right, bottom)`, где:
  - `left` - расстояние от левого края окна браузера до левого края элемента,
  - `top` - расстояние от верхнего края окна браузера до верхнего края элемента,
  - `right` - расстояние от левого края окна браузера до правого края элемента,
  - `bottom` - расстояние от верхнего края окна браузера до нижнего края элемента.
  
  Если во время выполнения произошла ошибка, метод вернёт `None`.

### Пример использования

```python
# Получаем координаты элемента
element_coordinates = element.get_coordinates()

# Печатаем координаты элемента
if element_coordinates is not None:
    print("The coordinates of the element are: ", element_coordinates)
else:
    print("An error occurred while getting the coordinates of the element.")
```


# class AppiumServer

## Описание класса

Класс `AppiumServer` предназначен для управления сервером Appium. Он позволяет запускать и останавливать сервер Appium с заданными параметрами, проверять его доступность и логировать процесс.

## Атрибуты

- `logger`: Объект для записи логов, основанный на настройках, указанных в `config.APPIUM_LOG_NAME`.
    
- `port`: Порт, на котором будет запущен сервер Appium. По умолчанию равен `4723`.
    
- `log_level`: Уровень детализации логирования. По умолчанию равен `'error'`.
    

## Конструктор

### `__init__()`

Инициализирует новый экземпляр класса `AppiumServer`.

**Параметры:**

- `port: int` - Порт, на котором будет запущен сервер Appium. По умолчанию равен `4723`.
    
- `log_level: str` - Уровень детализации логирования. По умолчанию равен `'error'`.

## Метод: `start()`

Этот метод запускает сервер Appium.

### Параметры

Метод не принимает параметров.

### Возвращаемое значение

- `bool`: Возвращает `True`, если сервер Appium был успешно запущен. В противном случае возвращает `False`.

### Пример использования

```python
# Запустить сервер Appium
is_started = app.start()
```

### Дополнительная информация

Метод запускает команду `appium server` с рядом параметров в отдельном подпроцессе, используя `subprocess.Popen`. Если процесс запуска успешен, метод возвращает `True`. В случае исключения типа `subprocess.CalledProcessError` или `OSError`, метод записывает ошибку в лог и возвращает `False`.

## Метод: `is_alive()`

Этот метод проверяет статус сервера Appium.

### Параметры

Метод не принимает параметров.

### Возвращаемое значение

- `bool`: Возвращает `True`, если сервер Appium доступен и готов к использованию. В противном случае возвращает `False`.

### Пример использования

```python
# Проверить статус сервера Appium
is_ready = app.is_alive()
```

### Дополнительная информация

Метод отправляет GET-запрос на "http://127.0.0.1:4723/wd/hub/sessions" для проверки статуса сервера Appium. Если сервер отвечает с кодом статуса 200, метод возвращает `True`. Если сервер отвечает с другим кодом статуса, метод записывает предупреждение в лог и возвращает `False`. В случае исключения `requests.exceptions.RequestException`, метод записывает ошибку в лог и возвращает `False`.

## Метод: `stop()`

Этот метод останавливает сервер Appium.

### Параметры

Метод не принимает параметров.

### Возвращаемое значение

- `bool`: Возвращает `True`, если сервер Appium был успешно остановлен. В противном случае возвращает `False`.

### Пример использования

```python
# Остановить сервер Appium
is_stopped = app.stop()
```

### Дополнительная информация

Метод запускает команду 'taskkill /F /IM node.exe' в подпроцессе, используя `subprocess.check_output`. Если процесс остановки успешен, метод возвращает `True`. В случае исключения типа `subprocess.CalledProcessError`, метод возвращает `False`.

## Метод: `wait_until_alive()`

Этот метод ожидает, пока сервер Appium не станет доступным.

### Параметры

- `timeout` (`int`, необязательный): Максимальное время ожидания в секундах, в течение которого метод будет проверять статус сервера. Значение по умолчанию: `60`.
- `poll` (`int`, необязательный): Интервал времени в секундах между проверками статуса сервера. Значение по умолчанию: `2`.

### Возвращаемое значение

- `bool`: Возвращает `True`, если сервер Appium стал доступным в течение заданного времени ожидания. В противном случае возвращает `False`.

### Пример использования

```python
# Ожидать, пока сервер Appium не станет доступным в течение 60 секунд с интервалом проверки 2 секунды
is_ready = app.wait_until_alive(timeout=60, poll=2)
```

### Дополнительная информация

Метод использует вспомогательный метод `is_alive()` для проверки статуса сервера. Он будет продолжать проверку статуса сервера каждые `poll` секунд в течение `timeout` секунд или до тех пор, пока сервер не станет доступным. Если сервер становится доступным в течение времени ожидания, метод возвращает `True`. Если сервер так и не становится доступным после истечения времени ожидания, метод возвращает `False`.


## class `AppiumNavigator`

Этот класс предоставляет функционал навигации для приложения, управляемого через сервер Appium.

### Атрибуты

- `app` (`AppiumExtended`): Экземпляр класса `AppiumExtended`, который предоставляет API для взаимодействия с сервером Appium.
- `graph_manager` (`AppiumGraph`): Объект для управления графом приложения.
- `logger` (`logging.Logger`): Логгер для записи логов.
- `image` (`AppiumImage`): Объект для работы с изображениями в контексте Appium.

## Конструктор

### `__init__()`

Инициализирует новый экземпляр класса `AppiumNavigator`.

**Параметры:**

- `app` (`AppiumExtended`): Экземпляр класса `AppiumExtended`, который предоставляет API для взаимодействия с сервером Appium.

## Метод: `add_page()`

Этот метод добавляет вершину в граф навигации приложения.

### Параметры

- `page` (`str`): Название страницы (экрана или окна), которую нужно добавить в граф.
- `edges` (`List[str]`): Список страниц (экранов или окон), к которым можно перейти с текущей страницы. Страницы представлены их названиями.

### Возвращаемое значение

Метод не возвращает значения.

### Пример использования

```python
# Добавить новую страницу в граф навигации приложения
navigator.add_page(page='HomePage', edges=['SettingsPage', 'ProfilePage'])
```

### Дополнительная информация

Метод использует `graph_manager` для добавления новой вершины в граф навигации приложения. Вершина представляет собой страницу (экран / окно) в приложении. Метод принимает название страницы и список других страниц, к которым можно перейти с текущей страницы.

## Метод: `navigate()`

Этот метод выполняет навигацию от текущей страницы к указанной целевой странице в приложении.

### Параметры

- `current_page` (`Type[YourPageClass]`): Класс текущей страницы, на которой находится пользователь.
- `destination_page` (`Type[YourPageClass]`): Класс целевой страницы, на которую пользователь хочет перейти.
- `timeout` (`int`, необязательный): Максимальное время ожидания перехода, по умолчанию 55 секунд.

### Возвращаемое значение

Метод не возвращает значения.

### Исключения

- `ValueError`: Если не удается найти путь от текущей страницы к целевой странице.

### Пример использования

```python
# Перейти с главной страницы на страницу настроек
navigator.navigate(current_page=HomePage, destination_page=SettingsPage)
```

### Дополнительная информация

Метод использует поиск пути и последовательное выполнение шагов навигации, чтобы перейти от текущей страницы к целевой. Если указанная целевая страница совпадает с текущей, никаких действий не выполняется.

Вначале метод находит путь от текущей страницы к целевой с использованием `find_path()`. Если путь не найден, генерируется исключение `ValueError`. После того как путь найден, метод `perform_navigation()` выполняет навигацию, следуя найденному пути.

Примечание: `YourPageClass` в параметрах `current_page` и `destination_page` следует заменить на конкретные классы страниц в вашем приложении.

## Метод: `find_path()`

Этот метод использует поиск в ширину (BFS) для нахождения пути от стартовой страницы до целевой. 

### Параметры

- `start_page` (`Any`): Начальная страница поиска пути.
- `target_page` (`Any`): Целевая страница, которую нужно достичь.

### Возвращаемое значение

- `Optional[List[Any]]`: Список страниц, образующих путь от стартовой до целевой страницы. Если путь не найден, возвращает `None`.

### Пример использования

```python
# Найти путь от главной страницы до страницы настроек
path = navigator.find_path(start_page=HomePage, target_page=SettingsPage)
```

### Дополнительная информация

Метод обходит граф переходов между страницами, сохраняя текущий путь и посещенные страницы. Если стартовая страница совпадает с целевой, никаких действий не выполняется.

Вначале метод создает множество для отслеживания посещенных страниц и очередь для выполнения поиска в ширину. Затем, пока очередь не пуста, метод извлекает текущую страницу и путь от стартовой страницы до нее. Получает переходы (соседние страницы) для текущей страницы и проверяет каждую соседнюю страницу. Если соседняя страница является целевой, возвращает полный путь. Если соседняя страница не была посещена, добавляет ее в очередь для дальнейшего поиска. Если путь не найден, возвращает `None`.

Примечание: `start_page` и `target_page` должны быть конкретными классами страниц в вашем приложении.

## Метод: `perform_navigation()`

Этот метод выполняет навигацию по заданному пути.

### Параметры

- `path` (`List[Any]`): Список страниц, образующих путь для навигации. Каждый элемент списка представляет страницу, а порядок элементов в списке определяет последовательность переходов от одной страницы к другой.
- `timeout` (`int`, необязательный): Максимальное время ожидания перехода, по умолчанию 55 секунд.

### Возвращаемое значение

- `None`

### Пример использования

```python
# Предположим, мы уже нашли путь от главной страницы до страницы настроек
path = [HomePage, MenuPage, SettingsPage]
# Выполняем навигацию по этому пути
navigator.perform_navigation(path)
```

### Дополнительная информация

Метод принимает список страниц, который представляет собой путь для навигации. Он выполняет переходы между соседними страницами, чтобы достичь целевой страницы. Проходит по пути и выполняет переходы между соседними страницами. Если метод перехода между текущей и следующей страницами не найден, выводит сообщение об ошибке. После выполнения каждого перехода ожидает появления изображения целевой страницы.

Примечания: 
- Элементы списка `path` должны быть конкретными классами страниц в вашем приложении.
- Рекомендуется вместо него использовать метод navigate()

