```python
#用python获取数据  read()
#help(open)
#fp = open("/Users/jinhua/Desktop/train.csv")
with open('/Users/jinhua/Desktop/hello.txt','w') as f:
    f.write('hello!world!\n111111\n222222\n3333333')
    f.close()
with open('/Users/jinhua/Desktop/hello.txt') as f:
    P1 = f.read()
    P2 = f.read()
print(P1)#从头读到尾
print(P2)#输出为空，因为文件指针已经读到文件尾部
with open('/Users/jinhua/Desktop/hello.txt') as f:
    P1 = f.read(5)
    P2 = f.read()#接着向下读
print(P1)
print(P2)
#with 语句在执行后会主动关闭语句句柄，所以不用额外close
```

    hello!world!
    111111
    222222
    3333333
    
    hello
    !world!
    111111
    222222
    3333333



```python
#readlines,readline
with open('/Users/jinhua/Desktop/hello.txt','w') as f:
    f.write('hello!world!\n111111\n222222\n3333333')
    f.close()
with open('/Users/jinhua/Desktop/hello.txt') as f:
    lines1 = f.readlines()
    #lines2 = f.readline()
print(lines1)
#print(lines2)
```

    ['hello!world!\n', '111111\n', '222222\n', '3333333']



```python

```

    



```python

```
