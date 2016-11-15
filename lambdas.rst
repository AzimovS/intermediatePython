Lambdas
-------

Lmabdas são funções de uma única linha. Elas também são conhecidas como 
funções anônimas em outras linguagens. Você provavelmente irá usar lambda
para evitar utilizar uma mesma função duas vezes em um programa. Elas são como 
uma função normal e se comportam como uma função normal.

**Assinatura**

.. code:: python

    lambda argument: manipulate(argument)

**Exemplo**

.. code:: python

    add = lambda x, y: x + y

    print(add(3, 5))
    # Output: 8

Aqui estão alguns casos de uso de lambdas e alguns jeitos em que elas podem
ser utilizadas:

**Ordenação de Listas**

.. code:: python

    a = [(1, 2), (4, 1), (9, 10), (13, -3)]
    a.sort(key=lambda x: x[1])

    print(a)
    # Output: [(13, -3), (4, 1), (1, 2), (9, 10)]

**Ordenação Paralela de Listas**

.. code:: python

    data = zip(list1, list2)
    data.sort()
    list1, list2 = map(lambda t: list(t), zip(*data))
