## TypeScript

[toc]

### 基础类型

####  1. Number类型

> ```typescript
> let age: number = 18;
> ```

#### 2. String类型

> ```typescript
> let name: string = 'youngxin'
> ```

#### 3. Boolean类型

> ``` typescript
> let isMan: boolean = true;
> ```

#### 4. Array类型

> // 数字数组，`元素类型[]`
>
> ``` typescript
> let numberList: number[] = [1,2,3]; 
> ```
>
> // 数组泛型，`Array<元素类型>`
>
> ``` typescript
> let stringList: Array<string> = ['1','2','3'];
> ```

#### 5. Tuple类型

> 元组类型允许表示一个已知元素数量和类型的数组，各元素的类型不必相同。
>
> ``` typescript
> let mixArr:[string, number];
> mixArr = ['hello', 18];
> ```

#### 4. Enum类型

> 枚举类型是对JavaScript标准数据类型的一个补充。使用枚举类型可以为一组数值赋予友好的名字。
>
> * 基础用法
>
> ``` typescript
> enum Color {Red, Green, Blue}
> let c: Color = Color.Green;
> ```

#### 5. Any类型

> any类型标记的变量将跳过类型检查

#### 6. Void类型

> 通常用户函数返回值，表示没有任何类型，及当函数没有返回值的时候。
>
> ``` typescript
> function hellow(): void {
>     console.log('HELLO WORLD!');
> }
> ```

#### 7. Null 和 Undefined

> ``` typescript
> let u: undefined = undefined;
> let n: null = null;
> ```
>
> 默认情况下`null`和`undefined`是所有类型的子类型。
>
> 在项目中，推荐在配置文件中添加`strictNullChecks: true `，使使`null`和`undefined`只能赋值给`void`和它们各自，来避免很多常见问题。
>
> 如果需要使用`undefined`搭配其他的数据类型推荐使用联合类型：string | number | undefined；

#### 8. Nerver类型

> `never`类型表示的是那些永不存在的值的类型。
>
> 常见的有
>
> * 抛出异常
> * 死循环

#### 9. Object类型

#### 类型断言

​	在开发过程中，我们可能比TypeScript的类型推断更明确一个变量的值，可以通过类型断言的语法告诉编辑器，`相信我，我知道自己在干什么`。

* `<>`语法

  > ``` typescript
  > 
  > ```
  >
  > 

* `as`语法
