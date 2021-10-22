## python 的参数

* 必须参数

  ```python
  #!/usr/bin/python3
   
  #可写函数说明
  def printme( str ):
     "打印任何传入的字符串"
     print (str)
     return
   
  # 调用 printme 函数，不加参数会报错
  printme()
  ```

* 关键字参数

  ```python
  #可写函数说明
  def printme( str ):
     "打印任何传入的字符串"
     print (str)
     return
   
  #调用printme函数
  printme( str = "菜鸟教程")
  ```

* 默认参数

  ```python
  #可写函数说明
  def printinfo( name, age = 35 ):
     "打印任何传入的字符串"
     print ("名字: ", name)
     print ("年龄: ", age)
     return
   
  #调用printinfo函数
  printinfo( age=50, name="runoob" )
  print ("------------------------")
  printinfo( name="runoob" )
  ```

* 不定长参数

  ```python
  # 可写函数说明
  def printinfo( arg1, *vartuple ):
     "打印任何传入的参数"
     print ("输出: ")
     print (arg1)
     for var in vartuple:
        print (var)
     return
   
  # 调用printinfo 函数
  printinfo( 10 )
  printinfo( 70, 60, 50 )
  加了两个星号 ** 的参数会以字典的形式导入。
  def printinfo( arg1, **vardict ):
     "打印任何传入的参数"
     print ("输出: ")
     print (arg1)
     print (vardict)
   
  # 调用printinfo 函数
  printinfo(1, a=2,b=3)
  如果单独出现星号 * 后的参数必须用关键字传入。
  >>> def f(a,b,*,c):
  ...     return a+b+c
  ... 
  >>> f(1,2,3)   # 报错
  Traceback (most recent call last):
    File "<stdin>", line 1, in <module>
  TypeError: f() takes 2 positional arguments but 3 were given
  >>> f(1,2,c=3) # 正常
  6
  >>>
  ```

  ## python Slice 操作
  
  ```python
  str=str[:-1]#删除最后一个字符串
  ```
  
  