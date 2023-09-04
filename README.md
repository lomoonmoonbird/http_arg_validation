# http_arg_validation
通用http请求参数名，参数类型，默认值限制装饰器，支持必选参数和可选参数。

# usage

## 必选参数page，类型为int型，默认值为1
```python
@arg_parser(page=(int, 1))
async def func(self, request):
  pass
```

## 可选参数

可选参数page，类型为int，无默认值
```python
@arg_parser(("page", int))
async def func(self, request):
  pass

```

