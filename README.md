Description:
В наведеному коді було проведено порівняння середнього часу відпрацювання трьох алгоритмів сортування: 
  - злиттям (Merge sort),
  - вставками
  - Timsort (з використанням функції сортування: sorted)
  - Timsort (з використанням функції сортування: sort).
Для порівняння було рандомно створено два набори даних:
  - small data, що містить 1000 записів
  - medium data, що містить 5000 записів.
Для заміру часу виконання алгоритмів використовувався модуль timeit.

В рультаті запуску коду було отримано наступні результати:

розмір 'small data' складає 1000 записів
розмір 'medium data' складає 5000 записів

:------------------- | :------------------- | :-------------------
| Algorithm          | Time small data      | Time medium data
:------------------- | :------------------- | :-------------------
| Merge sort         | 0.01386              | 0.09109
| Insertion sort     | 0.16365              | 4.09372
| Tim sort (sorted)  | 0.00070              | 0.00461
| Tim sort (sort)    | 0.00057              | 0.00440

Проаналізувавчи час відпрацювання кожного з алгоритмів сортування на різних за обсягом даних, 
можна зробити висновок, що Timsort, який поєднує в собі сортування злиттям і сортування вставками, 
є набагато ефективнішим у порівняні з іншими алгоритмами.
Саме тому в більшості випадків слід використовувати вбудовані в Python алгоритми, а не кодувати вручну.
