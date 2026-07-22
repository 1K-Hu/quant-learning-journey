# 记得循环字符后面加冒号
input('请输入: ')
    if number < answer:
        print('大一点')
    elif number > answer:
        print('小一点')
    else:
        print('恭喜你猜对了!')
        break
#当退出while循环的时候显示用户一共猜了多少次
print(f'你总共猜了{counter}次')




#下一个：找公倍数公因数
x = int(input('x = '))
y = int(input('y = '))
for factor in range(x, 0, -1):
    if x % factor == 0 and y % factor == 0:
        print(f'{x}和{y}的最大公约数是{factor}')
        print(f'{x}和{y}的最小公倍数是{x * y // factor}')
        break
## 枚举搜索
for num in range(100,1000):
    low = num % 10
    mid = (num // 10) % 10
    high = num // 100
    if num == low ** 3 + mid ** 3 + high ** 3:
        print(num)  
## 另一个
for x in range (20):
    for y in range (34):
        z = 100 - x - y
        if 5 * x + 3 * y + z//3 == 100 and z %3 == 0:
            print(f"公鸡: {x}, 母鸡: {y}, 小鸡: {z}")  