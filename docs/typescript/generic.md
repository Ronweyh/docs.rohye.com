## 泛型之 Hello World

下面来创建第一个使用泛型的例子：identity 函数。 这个函数会返回任何传入它的值。 你可以把这个函数当成是`echo`命令。

不用泛型的话，这个函数可能是下面这样：

```typescript
function identity(arg: number): number {
  return arg;
}
```

因此，我们需要一种方法使返回值的类型与传入参数的类型是相同的。 这里，我们使用了_类型变量_，它是一种特殊的变量，只用于表示类型而不是值。

```typescript
function identity<T>(arg: T): T {
    return arg;
}
```
