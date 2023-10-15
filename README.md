# Постановка задачи
На DNS сервер поступают запросы. Длины запросов имеют равномерное распределение с нижней границей
в 10 и верхней в 1000 байт. Одновременно сервер может обрабатывать A запросов в секунду. Обработка одного
запроса занимает от С секунд. Для необработанных запросов создается очередь, которая записывается
на жесткий диск сервера емкостью B Мб. Интенсивность запросов меняется в зависимости от времени суток:
- День: в среднем 30 зап./с
- Вечер: 100 зап./с
- Ночь: 2 зап./с

Задача: найти оптимальный объем накопителя, определить оптимальную пропускную способность (пропускная способность
не может изменяться не более чем на 50%). Определить оптимальное время на обработку запроса в различное время суток.