# python中时间日期操作

标签（空格分隔）： datetime,time

---
更加详细的内容参见              [datetime官方文档](https://docs.python.org/2/library/datetime.html)
python 中常用的关于时间日期的包有datetime,time。其中datetime是对time的进一步封装，因此datetime使用起来比time更加方便一点。

##常见的用法
    import datetime
    today=datetime.date.today()#获取今天日期 
    nowtime=datetime.datetime.now() #获取当前时间
    lasttime0=nowtime+datetime.timedelta(days=-10)#获取10天前的日期
    lasttime0=lasttime0.strftime('%Y-%m-%d')#日期格式化
##datetime中常用的类
###datetime.timedelta类
1.class datetime.timedelta(days=0, seconds=0, microseconds=0, milliseconds=0, minutes=0, hours=0, weeks=0)
2.类属性attributes：days,seconds,microseconds
eg:

    d1=datetime.datetime(2015,2,16)
    d2=datetime.datetime(2015,2,20)
    d2-d1
    Out:datetime.timedelta(4)
    (d2-d1).days
    Out:4
    (d2-d1).minutes
    Out:'datetime.timedelta' object has no attribute 'minutes'
    
下面是几个常用的函数：
1.datetime.weekday()
Return the day of the week as an integer, where Monday is 0 and Sunday is 6
2.datetime.isoweekday()
Return the day of the week as an integer, where Monday is 1 and Sunday is 7


