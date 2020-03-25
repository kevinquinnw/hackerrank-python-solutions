``` python
def handle(result):
    inpu = input().split()
    command = inpu[0]
    values = inpu[1:]
    if command == 'print':
        print(result)
    else:
        execute = 'result.' + command + "(" + ",".join(values) + ")"
        eval(execute)

    
result =[]
for i in range (int(input())):
    handle(result)
```
