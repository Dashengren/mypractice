# 01.格式化字符串

```python
a = 'hello'
#字符串之间也可以进行加法运算
#如果将两个字符串进行相加，则会自动将两个字符串拼接为一个
a = 'abc' + 'haha' + '哈哈'
#a = 123 
#字符串只能不能和其他的类型进行加法运算，如果做了会出现异常 TypeError: must be str, not int
#print("a = "+a) # 这种写法在Python中不常见
a = 123
print('a =',a)

#在创建字符串时，可以在字符串中指定占位符
#%s 在字符串中表示任意字符
#%f 浮点数占位符
#%d 整数占位符
b = 'Hello %s'%'孙悟空'
b = 'hello %s 你好 %s'%('tom','孙悟空')
b = 'hello %3.5s'%'abcdefg' # %3.5s字符串的长度限制在3-5之间
b = 'hello %s'%123.456
b = 'hello %.2f'%123.456
b = 'hello %d'%123.95
b = '呵呵'
#格式化字符串，可以通过在字符串前添加一个f来创建一个格式化字符串
#在格式化字符串中可以直接嵌入变量
c = f'hello {a} {b}'
print(f'a = {a}')
```

# 02.复制字符串

```python
# 创建一个变量来保存你的名字
name = '孙悟空'

# 使用四种方式来输出，欢迎 xxx 光临
# 拼串
print('欢迎 '+name+' 光临！')
# 多个参数
print('欢迎',name,'光临！')
# 占位符
print('欢迎 %s 光临！'%name)
# 格式化字符串
print(f'欢迎 {name} 光临！')
i
# 字符串的复制（将字符串和数字相乘）
a = 'abc'
# * 在语言中表示乘法
# 如果将字符串和数字相乘，则解释器会将字符串重复指定的次数并返回
a = a * 20

print(a)
```

<u></u>

# Python File 方法

​		**truncate()** 方法用于截断文件，如果指定了可选参数 size，则表示截断文件为 size 个字符。 如果没有指定 size，则从当前位置起截断；截断之后 size 后面的所有字符被删除（即清空文件）。



# Python OS文件/目录方法

​		**os.getcwd()** 方法用于返回当前工作目录。