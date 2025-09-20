### Как заполнять и просматривать документацию в Python

[Хорошая статья по pydoc](https://pythonchik.ru/osnovy/dokumentirovanie-koda-v-python)

##### Заполнение документации - строка """ abc """:
- для пакета с первой строки файла __init.py
- для модуля с первой строки файла модуля
- для класса после объявления класса
- для функции и метода после объявления функции или метода

##### Просмотр документации
- в интерпретаторе Python
	- help() ```python
		import my_module
		 help(my_module)
	- __doc__```python
		import my_module
		my_module.__doc__
		my_module.my_function.__doc__
		my_module.MyClass.__doc__
		my_module.MyClass.my_method.__doc__
- встроенная библиотека pydoc генерирует документацию
		```
```python
python -m pydoc # просмотр доступных функций
python -m pydoc math # просмтр модуля
python -m pydoc -k <keyword> # поиск по ключевому слову в док. доступн. модулей
python -m pydoc -p 331 # создание сервера с документац. на порте 331
# закрыте сервера q
python -m pydoc -b # открытие сервера на свободном порту
python -m pydoc -w sqlite # запись документции по модулю в html файл
```

[[Python]]