# 事件驱动

### 回调函数
新人进场的时候你要帮忙点炮仗，当然，现在给你的是一串炮仗，不能给你一个点着的炮仗；事件驱动里面，写的是一个函数名，不能是一个函数的调用

```javascript
function dianPao(){
    alert('Peng!Peng!Peng!...')
}

xinren.jinChang( dianPao ); //正确
xinren.jinChang( dianPao() ); //错误
```

注意函数被调用执行的时机
