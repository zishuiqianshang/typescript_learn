# 数据类型

## 布尔值 boolean

let isDo:boolean = false

## 数值 number

let cur_num :number = 1;

注：ES6的二进制和八进制表示会被编译为十进制数字

## 字符串 string

let name:string = 'Tom'

## 空值 void

可用void表示无返回值函数

function noV():void{

​	console.log('该函数无返回值')

}

## Null

定义原始类型，该类型是所有类型的子类型,，可赋值给所有类型的变量

let n:null =null;

## Undefined

定义原始类型，该类型是所有类型的子类型,，可赋值给所有类型的变量

let u:undefined

## 数组

### 表示法1：元素类型 []

let num_list:  number[] = [1,2,3,4,5]

### 表示法2：Array<元素类型>

let num_list: Array<number> = [1,2,3,4,5]



## 元组 Tuple

元组类型允许表示一个已知元素数量和类型的数组，各元素的类型不必相同。 比如，你可以定义一对值分别为`string`和`number`类型的元组。

let x:[string,number]

x = ["hello",1] 

## 枚举 enum

enum类型是对JavaScript标准数据类型的一个补充。 像C#等其它语言一样，使用枚举类型可以为一组数值赋予友好的名字。默认情况下，从`0`开始为元素编号。 你也可以手动的指定成员的数值。 例如，我们将上面的例子改成从`1`开始编号：

enum Color {Red = 1, Green, Blue}

let c: Color = Color.Green;

let colorName: string = Color[2];

## 任意值 any

忽视编译，允许被赋值为任意类型，声明一个变量为任意值之后，对它的任何操作，返回的内容的类型都是任意值。

let list: any[] = [1, true, "free"];