import json
from collections import defaultdict
from datetime import datetime

# Считываем данные из файла
with open("C:/Users/odina/PycharmProjects/skillfactory/orders_july_2023.json","r") as my_file:
    orders = json.load(my_file)

# Инициализация переменных для хранения ответов на вопросы
max_price = 0
max_order = ''
max_quantity = 0
max_quantity_order = ''
order_count_per_day = defaultdict(int)
user_order_count = defaultdict(int)
user_total_price = defaultdict(float)
total_price = 0
total_quantity = 0

# Обработка заказов
for order_num, orders_data in orders.items():
    # Получаем данные заказа
    price = orders_data['price']
    quantity = orders_data['quantity']
    date = orders_data['date']
    user_id = orders_data['user_id']

    # Номер самого дорогого заказа
    if price > max_price:
        max_order = order_num
        max_price = price

    # Номер заказа с самым большим количеством товаров
    if quantity > max_quantity:
        max_quantity_order = order_num
        max_quantity = quantity

    # Подсчет заказов по дням
    order_date = datetime.strptime(date, '%Y-%m-%d').date()
    order_count_per_day[order_date] += 1

    # Подсчет количества заказов от каждого пользователя
    user_order_count[user_id] += 1

    # Подсчет общей стоимости и количества товаров
    user_total_price[user_id] += price
    total_price += price
    total_quantity += quantity

# Находим день с наибольшим количеством заказов
max_orders_day = max(order_count_per_day, key=order_count_per_day.get)

# Находим пользователя с наибольшим количеством заказов
max_user_orders = max(user_order_count, key=user_order_count.get)

# Находим пользователя с наибольшей суммарной стоимостью заказов
max_user_total_price = max(user_total_price, key=user_total_price.get)

# Вычисляем среднюю стоимость заказа и среднюю стоимость товаров
average_order_price = total_price / len(orders) if len(orders) > 0 else 0
average_price_per_item = total_price / total_quantity if total_quantity > 0 else 0

# Печатаем результаты
print(f'Номер заказа с самой большой стоимостью: {max_order}, стоимость заказа: {max_price}')
print(f'Номер заказа с самым большим количеством товаров: {max_quantity_order}, количество товаров: {max_quantity}')
print(f'День с самым большим количеством заказов: {max_orders_day}, количество заказов: {order_count_per_day[max_orders_day]}')
print(f'Пользователь с самым большим количеством заказов: {max_user_orders}, количество заказов: {user_order_count[max_user_orders]}')
print(f'Пользователь с самой большой суммарной стоимостью заказов: {max_user_total_price}, сумма заказов: {user_total_price[max_user_total_price]}')
print(f'Средняя стоимость заказа: {average_order_price}')
print(f'Средняя стоимость товаров: {average_price_per_item}')
