### Input

```python
numbers = list(map(int, input().split()))
```

### List and Dict

* Zip: 
    ```python
    stocks = { 
        'Goog' : 520.54, 
        'FB' : 76.45, 
        'yhoo' : 39.28, 
        'AMZN' : 306.21, 
        'APPL' : 99.76
        } 

    zipped_1 = zip(stocks.values(), stocks.keys()) 

    # sorting according to values 
    print(sorted(zipped_1)) 

    zipped_2 = zip(stocks.keys(), stocks.values()) 
    print(sorted(zipped_2)) 
    #sorting according to keys 
    ```

### Lambdas

* Map
    ```python
    # Python code to apply a function on a list 
    income = [10, 30, 75] 

    def double_money(dollars): 
        return dollars * 2

    new_income = list(map(double_money, income)) 
    print(new_income)

    # Output: [20, 60, 150]
    ```
### Itertools
* Permutations:

    ```python
    from itertools import permutations 
    perm = permutations([1, 2, 3], 2) 
    for i in list(perm): 
        print i 

    # Answer->(1, 2), (1, 3), (2, 1), (2, 3), (3, 1), (3, 2) 
    ```

### heapq
* Python code to find 3 largest and 4 smallest elements of a list. 

    ```python
    import heapq 

    grades = [110, 25, 38, 49, 20, 95, 33, 87, 80, 90] 
    print(heapq.nlargest(3, grades)) 
    print(heapq.nsmallest(4, grades))

    #[110, 95, 90]
    #[20, 25, 33, 38] 
    ```
