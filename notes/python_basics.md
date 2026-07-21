#笔记
# Python 基础笔记

## 条件判断（if / elif / else）

```python
pe = 25
if pe < 10:
    print(f"PE={pe}，低估")
elif pe < 25:
    print(f"PE={pe}，合理")
else:
    print(f"PE={pe}，高估")

#字符串格式化
name = "茅台"
price = 1480.5
print(f"{name} 股价 {price:.2f} 元")
