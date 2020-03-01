# You Don't Know JS: Up & Going

# Chapter 1: Into Programming

欢迎来到 *你不懂的JS* （YDKJS）系列。

Up＆Going是对几个基本编程概念的介绍 - 当然我们专注于JavaScript（通常缩写为JS） - 以及如何处理和理解本系列中的其他标题。特别是如果你刚刚进入编程和/或JavaScript，这本书将简要地探讨你需要什么样的东西来入门和进阶。

本书从很高的层面开始解释编程的基本原理。如果你开始使用YDKJS时几乎没有或根本没有编程经验，并且正在寻找这些书来帮助你开始使用JavaScript来理解编程。

第1章应该作为你想要了解更多内容的快速概述，并练习如何 *进入编程* 。还有许多其他优秀的编程介绍资源可以帮助你进一步深入研究这些主题，我鼓励你在本章之外从中学习。

一旦你对通用编程基础感到满意，第2章将帮助你熟悉JavaScript的编程风格。第2章介绍了JavaScript的用途，但同样，它并不是一本全面的指南 - 这就是YDKJS其他书籍的用途！

如果你对JavaScript已经相当熟悉，请首先查看第3章，简要介绍一下YDKJS的内容，然后直接进入！

## Code

让我们从头开始。

程序通常被称为源代码或仅代码，是一组特殊指令，用于告诉计算机要执行的任务。通常代码保存在文本文件中，但使用JavaScript，你也可以直接在浏览器中的开发者控制台中敲代码，我们将在稍后介绍。

有效格式和指令组合的规则称为计算机语言，有时也称为语法，与英语大致相同，告诉你如何拼写单词以及如何使用单词和标点符号创建有效句子。

### Statements

在计算机语言中，执行特定任务的一组单词，数字和运算符是一个语句。在JavaScript中，语句可能如下所示：

```js
a = b * 2;
```

字符`a`和`b`被称为变量（参见“Variables”），它们就像你可以存储任何内容的简单盒子。在程序中，变量保存程序使用的值（如数字`42`）。将它们视为值本身的象征性占位符。

相比之下，`2`只是一个值本身，称为*字面* 值，因为它独立存在而不存储在变量中。

`=`和`*`字符是运算符(参考"Operators") -- 它们使用值和变量（如赋值和数学乘法）执行操作。

JavaScript中的大多数语句最后都以分号(`;`)结尾。

声明`a = b * 2;`粗略地告诉计算机获取存储在变量`b`中的当前值，将该值乘以`2`，然后将结果存储回另一个我们称之为`a`的变量中。

程序只是许多此类语句的集合，它们共同描述了执行程序目的所需的所有步骤。

### Expressions

语句由一个或多个表达式组成。表达式是对变量或值的任何引用，或与运算符组合的一组变量和值。

例如：

```js
a = b * 2;
```

该语句中有四个表达式：

- `2`是一个字面值表达式
- `b`是变量表达式，表示检索其当前值
- `b * 2`是算术表达式，表示进行乘法运算
- `a = b * 2`是一个赋值表达式，它意味着将`b * 2`表达式的结果赋给变量`a`（稍后有关赋值的更多信息）

一个独立的通用表达式也称为 *表达式语句* ，如下所示： 

```js
b * 2;
```

这种表达式语句不是很常见或有用，因为它通常不会对程序的运行产生任何影响 - 它会检索`b`的值并将其乘以`2`，但他的结果在之后不会做任何事情。

更常见的表达式语句是调用 *表达式语句* （请参阅“Functions”），因为整个语句是函数调用表达式本身：

```js
alert( a );
```

### Executing a Program

那些编程语句集合如何告诉计算机该怎么做？程序需要执行，也称为 *运行* 程序。

像`a = b * 2`这样的语句对于开发人员在阅读和写作时很有帮助，但实际上并不是计算机可以直接理解的形式。因此，计算机上的特殊实用程序（*解释器* 或 *编译器* ）用于将你编写的代码转换为计算机可以理解的命令。

或者一些计算机语言，这种命令的翻译通常是在每次运行程序时从上到下逐行完成，这通常称为 *解释* 代码。

对于其他语言，翻译是提前完成的，称为编译代码，因此当程序在之后运行时，正在运行的是实际已经编译好的计算机指令。

通常断言JavaScript是被 *解释* 的，因为每次运行时都会处理JavaScript源代码。但这并不完全准确。 JavaScript引擎实际上会动态 *编译* 程序，然后立即运行已编译的代码。

**注意：** 有关JavaScript编译的更多信息，请参阅本系列的Scope＆Closures标题的前两章。

## Try It Yourself

本章将用简单的代码片段介绍每个编程概念，所有代码都用JavaScript编写（显然！）。

它不能再被强调：当你完成本章时 - 你可能需要花费时间来重复几次 - 你应该自己输入代码来练习这些概念。最简单的方法是在最近的浏览器（Firefox，Chrome，IE等）中打开开发者工具控制台。

**提示：** 通常，你可以使用键盘快捷键或菜单项启动开发者控制台。有关在你喜欢的浏览器中启动和使用控制台的更多详细信息，请参阅“掌握开发人员工具控制台”（http://blog.teamtreehouse.com/mastering-developer-tools-console）。要一次在控制台中键入多行，请使用`<shift> + <enter>`移动到下一个新行。一旦你敲击`<enter>`，控制台将运行你刚输入的所有内容。

让我们熟悉在控制台中运行代码的过程。首先，我建议在浏览器中打开一个空标签。我更喜欢通过在地址栏中键入`about:blank`来完成此操作。然后，确保你的开发者控制台是打开的，正如我们刚才提到的那样。

现在，键入此代码并查看其运行方式：

```js
a = 21;

b = a * 2;

console.log( b );
```

在Chrome中将上述代码键入控制台应该会产生如下内容：

![](https://github.com/getify/You-Dont-Know-JS/raw/master/up%20%26%20going/fig1.png)

继续，试试吧。学习编程的最好方法是开始编码！

### Output

在前面的代码片段中，我们使用了`console.log()`。简而言之，让我们来看看这行代码是什么。

你可能已经猜到了，但这正是我们在开发者控制台中打印文本（也就是输出给用户）的方式。我们应该解释这个语句的两个特征。

首先，`log( b )`的部分称为函数调用(参考"Functions")。发生的事情是我们将`b`变量交给该函数，该函数要求它取`b`的值并将其打印到控制台。

第二，`console.` 部分是`log(..)`函数所在的对象引用。我们将在第2章中更详细地介绍对象及其属性。

另一种创建输出的方法是运行`alert()`语句。例如：

```js
alert( b );
```

如果你运行它，你会注意到它不是将输出打印到控制台，而是显示一个带有`b`变量内容的弹出“确定”框。但是，使用`console.log()`通常会比使用`alert(..)`更容易学习编码和在控制台中运行程序，因为你可以一次输出多个值而不会中断浏览器界面。

对于本书，我们将使用`console.log()`进行输出。

### Input

在我们讨论输出时，你可能也想知道输入（即，从用户接收信息）。

最常见的方法是HTML页面向用户显示表单元素（如文本框），用户可以输入表单元素，然后使用JS将这些值读取到程序变量中。

但是，有一种更简单的方法可以获得简单的学习和演示目的，例如你将在本书中做的事情。使用`prompt(..)`功能：

```js
age = prompt( "Please tell me your age:" );

console.log( age );
```

正如你可能已经猜到的那样，你传递的消息`prompt(..)` - 在这种情况下，`"Please tell me your age:"` - 将打印到弹出窗口中。

这应该类似于以下内容：

![](https://github.com/getify/You-Dont-Know-JS/raw/master/up%20%26%20going/fig2.png)

通过单击“确定”提交输入文本后，你将看到键入的值存储在`age`变量中，然后我们使用`console.log()`输出：

![](https://github.com/getify/You-Dont-Know-JS/raw/master/up%20%26%20going/fig3.png)

为了在学习基本编程概念时保持简单，本书中的示例不需要输入。但是现在您已经了解了如何使用`prompt(..)`，如果你想挑战自己，可以尝试在对示例的探索中使用输入。

## Operators

运算符是我们如何对变量和值执行操作。我们已经看到了两个JavaScript运算符，`=`和`*`。

`*`运算符执行数学乘法运算。很简单吧？

`=`运算符用于赋值 -- 我们首先计算`=`右侧的值(源值)，然后将其放入我们在左侧指定的变量（目标变量）。

**警告：** 这可能看起来像指定赋值的奇怪的反向顺序。有些人可能更倾向于翻转顺序，因此源代码位于左侧而目标变量位于右侧，如`42 - > a`（这不是有效的JavaScript！），而不是`a = 42`。不幸的是，`a = 42`有序形式和类似的变体在现代编程语言中非常普遍。如果感觉不自然，只需花一些时间排练你心中的顺序就可以习惯它。

考虑下面的代码：

```js
a = 2;
b = a + 1;
```

这里，我们把`2`这个值赋值给变量`a`。然后，我们得到了`a`这个变量的值(仍然是`2`)，然后和`1`相加，我们得到的结果是`3`，然后我们把这个结果存在变量`b`里。

虽然从技术上讲不是运算符，但在每个程序中都需要关键字`var`，因为它是 *声明*（也就是创建）变量的主要方式（参见"Variables"）。

在使用变量之前，应始终按名称声明变量。但是你只需要为每个范围内的变量声明一次（参见"Scope"）;根据需要可以在之后多次使用。例如：

```js
var a = 20;

a = a + 1;
a = a * 2;

console.log( a );	// 42
```

以下是JavaScript中一些最常见的运算符：

- 赋值: 比如`a = 2`中的`=`

- 数学: `+`(加法)，`-`(减法)，`*`(乘法)，`/`(除法)

- 复合赋值: `+=`, `-=`, `*=`, 和 `/=`都是将数学运算与赋值相结合的复合运算符，例如`a += 2`(等同于`a = a + 2`)

- 递增/递减：`++`(递增)，`—`(递减)，比如`a++`(等同于`a = a + 1`)

- 对象属性访问：`.`,例如`console.log()`

  对象是在称为属性的特定命名位置保存其他值的值。`obj.a`意味着一个叫做`obj`的对象值有个名为`a`的属性。也可以将属性作为`obj["a"]`访问。见第2章。

- 相等：`==`(宽松相等)，`===`(严格相等)，`!=`(宽松不相等)，`!==`(严格不相等)。

  请参考"Values & Types" 和第2章

- 对比：`<`(小于)，`>`(大于)，`<=`(小于或宽松相等)，`>=`(大于或宽松相等)

  请参考"Values & Types" 和第2章

- 逻辑：`&&`(并且)，`||`(或)，例如在`a || b`中选择`a`或`b`

  这些运算符用于表示复合条件（参见"Conditionals"），就像`a`或`b`是真。

**注意：** 有关更多详细信息以及此处未提及的运算符，请参阅Mozilla开发人员网络（MDN）的“表达式和运算符”(<https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators>)

## Values & Types

如果你问一个手机店的员工某个手机的费用是多少，他们说“99,99”（即99.99美元），他们就会给你一个实际的美元数字代表你将需要支付（加税）多少才能购买。如果你想购买其中两部手机，你可以轻松地将心算，以获得199.98美元的基本费用。

如果同一个店员拿起另一部相似的手机说它是“免费的”（也许在用手比划引号），那么他们就不是在给你一个数字，而是你的花费（$0.00）的另一种表达形式 —— “免费”这个词。

当你稍后询问手机是否包含充电器时，该答案可能只是“是”或“否”。

以非常类似的方式，当你在程序中表达值时，你可以根据计划对它们执行的操作为这些值选择不同的表示形式。

这些不同的值表示在编程术语中称为 *类型* 。 JavaScript为每个所谓的原始值都有内置类型：

- 当你需要数学应用时，可能需要`number`
- 当你需要在屏幕上打印值时，你可能需要`string`(一个或多个字符，单词，句子)
- 当你需要在你的程序中做出决定时，你可能需要`boolean`(`true`或者`false`)

直接包含在源代码中的值称为 *字面量*。`string`字面量用双引号`"..."`或者单引号`'...'` — 唯一的区别就是风格偏好。`number`和`boolean`直接表现出来(`42`，`true`)

考虑下面代码：

```js
"I am a string";
'I am also a string';

42;

true;
false;
```

在`string`/`number`/`boolean`值的类型以外，编程语言通常会提供 *数组*，*对象*，*函数* 等更多的类型。在本章和下一章中，我们将更多地介绍值和类型。

### Converting Between Types

如果你有一个`number`但需要在屏幕上打印它，则需要将该值转换为`string`，而在JavaScript中，此转换称为“强制”。同样，如果有人在电子商务页面上的表单(form)中输入一系列数字字符，那就是一个`string`，但如果你需要使用该值进行数学运算，则需要将其强制转换为`number`。

JavaScript提供了几种不同的设施，用于强制 *类型* 之间的转换。例如：

```js
var a = "42";
var b = Number( a );

console.log( a );	// "42"
console.log( b );	// 42
```

使用如图所示的`Number()`（内置函数）是从任何其他类型到`number`类型的 *显式* 强制转换。这应该是非常直接的。

但是一个有争议的话题是当你试图比较两个不属于同一类型的值时会发生什么，这需要 *隐式* 强制转换。

将字符串`"99.99"`与数字`99.99`进行比较时，大多数人都认为它们是等价的。但他们并不完全一样，是吗？它在两种不同的表示形式中是相同的值，但是两种是不同的 *类型* 。你可以说他们“宽松的相等”，不是吗？

为了帮助解决这些常见情况，JavaScript有时会启动并 *隐式* 地将值强制转换为匹配类型。

因此你使用`==`宽松相等运算符去对比`"99.99" == 99.99`，JavaScript会转换左边的`"99.99"`到对于的`number`类型`99.99`。对比就变成了`99.99 == 99.99`，这个结果当然是`true`。

虽然旨在帮助你，但如果你没有花时间学习管理其行为的规则，则 *隐式* 强制可能会造成困扰。大多数JS开发人员都没有去学习，所以大多数的感觉是 *隐式* 强制令人困惑，并使使程序受到意外错误的危害，因此应该避免。

然而，隐式强制是一种可以 *学习* 的机制，而且任何希望认真对待JavaScript编程的人都应该学习。一旦你学会了规则，它不仅不会混淆，它实际上可以使你的程序更好！努力是值得的。

**注意：** 关强制的更多信息，请参阅本标题的第2章和本系列的 **Types & Grammar* * 标题的第4章。

## Code Comments

手机店员工可能会在新发布的手机的功能或公司提供的新计划上记下一些笔记。这些笔记只供员工阅读——不供客户阅读。然而，这些笔记通过记录她应该如何和为什么告诉客户，帮助员工更好地完成她的工作。

关于编写代码，你能学到的最重要的一点是，它不仅仅是为计算机编写的。代码的每一个字节都和写给编译器一样，也是写给开发者的。

你的计算机只关心来自编译的机器代码，一系列二进制0和1。你可以编写的程序数量几乎是无限的，它们产生相同的0和1系列。关于如何编写程序，你所做的选择不仅对你，而且对你的其他团队成员，甚至对你未来的自己都很重要。

你不仅要努力编写能够正常工作的程序，而且应该努力编写在审查时有意义的程序。通过为变量选择好名称（参见"Variables"）和函数（参见"Functions"），你可能有很长的路要走。

但另一个重要的部分是代码注释。些是程序中的一些文本，纯粹是为了向人类解释而插入的。解释器/编译器将始终忽略这些注释。

关于什么是良好注释的代码，有很多意见;我们无法真正定义绝对统一的规则。但是一些意见和指导非常有用：

- 没有注释的代码不是最理想的。
- 太多注释（例如，每行一个）可能是代码写得不好的标志。
- 注释应该解释 *为什么*，而不是 *什么* 。他们可以选择解释如何做，如果代码特别令人困惑。

在JavaScript中，可能有两种类型的注释：单行注释和多行注释。

考虑下面代码：

```js
// This is a single-line comment

/* But this is
       a multiline
             comment.
                      */
```

如果要在单个语句上方或甚至在行尾添加注释，`//`单行注释是合适的。`//`后面的所有内容都被视为注释（因此被编译器忽略），一直到行尾。对单行注释中的内容没有限制。

考虑下面代码：

```js
var a = 42;		// 42 is the meaning of life
```

如果在评论中有几行解释，则`/ * .. * /`多行注释是合适的。

以下是多行注释的常见用法：

```js
/* The following value is used because
   it has been shown that it answers
   every question in the universe. */
var a = 42;
```

它也可以出现在一条线上的任何地方，即使在一条线的中间，因为`* /`结束它。例如：

```js
var a = /* arbitrary value */ 42;

console.log( a );	// 42
```

唯一不能出现在多行注释中的是`* /`，因为这将被解释为结束注释。

你一定要开始学习编程，开始注意代码的习惯。在本章的其余部分中，你将看到我使用注释来解释事物，因此在你自己的实践中也是如此。相信我，每个阅读你代码的人都会感谢你！

## Variables

大多数有用的程序需要跟踪一个值，因为它在程序运行过程中发生变化，并根据程序的预期任务所要求的方式进行不同的操作。

在程序中实现这一点的最简单方法是将一个值赋给一个称为变量的符号容器——之所以这样做是因为该容器中的值可以根据需要随时间变化。

在某些编程语言中，你声明一个变量（容器）来保存特定类型的值，例如`number`或`string`。静态类型，也称为类型强制，通常通过防止意外的值转换来提高程序的正确性。

其他语言强调值的类型而不是变量。弱类型（也称为动态类型）允许变量随时保存任何类型的值。它通常被认为是程序灵活性的一个好处，它允许单个变量表示一个值，无论该值在程序逻辑流程中的任何给定时刻可能采用何种类型。

JavaScript使用后一种方法，*动态类型* ，意味着变量可以保存任何类型的值，而无需任何类型强制。

如前所述，我们使用`var`语句声明一个变量 - 请注意声明中没有其他类型信息。考虑这个简单的程序：

```js
var amount = 99.99;

amount = amount * 2;

console.log( amount );		// 199.98

// convert `amount` to a string, and
// add "$" on the beginning
amount = "$" + String( amount );

console.log( amount );		// "$199.98"
```

`amount`变量开始时是数字`99.99`，然后保存了`amount * 2`的`number`结果，是`199.98`。

第一个`console.log(..)`命令 *隐式* 的强制`number`到`string`，打印出来。

然后`amount = "$" + String(amount)`语句 *显示* 的强制`199.98`到`string`类型，并且在开始处加上了`"$"`字符。此时，`amount`现在保持`string`值`"$199.98"`，因此第二个`console.log()`语句不需要做任何强制来打印出来。

JavaScript开发人员会注意到为`99.99`,`199.98`和`"199.98"`值中的每一个使用`amount`变量的灵活性。态类型爱好者更喜欢像`amountStr`这样的单独变量来持有值`"$199.98"`的最终表示形式，因为它是一个不同的类型。

无论哪种方式，你都会注意到`amount`包含一个在程序运行过程中发生变化的运行值，说明了变量的主要目的：管理程序 *状态* 。

换句话说，*状态* 是在程序运行时跟踪对值的更改。

变量的另一个常见用法是集中设置值。当你声明变量携带值并且打算在整个程序中不更改该值时，这通常称为 *常量*。

你通常在程序的顶部声明这些常量，以便在需要时可以方便地在一个地方来更改使用值。按照惯例，作为常量的JavaScript变量通常是大写的，在多个单词之间使用下划线`_`。

下面是一个例子：

```js
var TAX_RATE = 0.08;	// 8% sales tax

var amount = 99.99;

amount = amount * 2;

amount = amount + (amount * TAX_RATE);

console.log( amount );				// 215.9784
console.log( amount.toFixed( 2 ) );	// "215.98"
```

**注意：** 类似于`console.log()`是作为`console`值上的对象属性访问的函数`log()`，`toFixed()`这里是一个可以在`number`值上访问的函数。JavaScript`number`不会自动格式化为美元 - 引擎不知道你的意图是什么，并且没有货币类型。`toFixed(..)`让我们指定我们想要舍入到的`number`的小数位数，并根据需要生成`string`。

根据惯例，`TAX_RATE`变量只是常量 - 这个程序没有什么特别的东西阻止它被改变。但是，如果城市将销售税率提高到9%，我们仍然可以通过在一个地方将`TAX_RATE`分配值设置为`0.09`来轻松更新我们的计划，而不是在整个计划中发现大量`0.08`的值，并更新所有这些值。

在撰写本文时，最新版本的JavaScript（通常称为“ES6”）包含一种通过使用`const`而不是`var`来声明常量的新方法：

```js
// as of ES6:
const TAX_RATE = 0.08;

var amount = 99.99;

// ..
```

常量就像带有不变的值的变量一样有用，常量还防止在初始设置之后的某些地方意外地改变它的值。如果你在第一次声明后尝试将任何不同的值分配给`TAX_RATE`，则程序将拒绝更改（在严格模式下，失败并显示错误 - 请参阅第2章中的"Strict Mode"）。

顺便说一下，这种针对错误的“保护”类似于静态类型执行，因此你可以看到为什么其他语言中的静态类型具有吸引力！

**注意：** 有关如何在程序中使用变量中的不同值的更多详细信息，请参阅本系列的类型和语法标题。

## Blocks

在购买新手机时，手机店员工必须完成一系列步骤才能完成结账。

同样，在代码中，我们经常需要将一系列语句组合在一起，我们通常称之为 *块* 。在JavaScript中，通过将一个或多个语句包装在大括号对`{...}`中来定义块。考虑：

```js
var amount = 99.99;

// a general block
{
	amount = amount * 2;
	console.log( amount );	// 199.98
}
```

这种独立的`{..}`通用块是有效的，但在JS程序中并不常见。通常，块附加到某些其他控制语句，例如`if`语句（请参阅"Conditionals"）或循环（请参阅"Loops"）。例如：

```js
var amount = 99.99;

// is amount big enough?
if (amount > 10) {			// <-- block attached to `if`
	amount = amount * 2;
	console.log( amount );	// 199.98
}
```

我们将在下一节中解释`if`语句，但正如你所看到的，带有两个语句的`{..}`块附加到`if(amount> 10);`只有在条件通过时才会处理块内的语句。

**注意：** 与大多数其他语句（如`console.log(amount);`）不同，块语句不需要使用分号（`;`）来结束它。

## Conditionals

“你想以9.99美元的价格在购买时增加额外的屏幕保护吗？”乐于助人的手机店员工已要求你做出决定。你可能需要先咨询你钱包或银行账户的当前 *状态* 来回答这个问题。但显然，这只是一个简单的“是或否”问题。

我们可以通过多种方式在程序中表达条件（即决定）。

最常见的是`if`语句。基本上，你会说，“如果这种情况属实，请执行以下操作......”。例如：

```js
var bank_balance = 302.13;
var amount = 99.99;

if (amount < bank_balance) {
	console.log( "I want to buy this phone!" );
}
```

`if`语句需要在括号`()`之间有一个表达式，可以将其视为`true`或`false`。在这个程序中，我们提供了表达式`amount <bank_balance`，它确实将根据`bank_balance`变量中的数量计算为`true`或`false`。

如果条件不成立，你甚至可以提供替代方法，称为`else`子句。考虑：

```js
const ACCESSORY_PRICE = 9.99;

var bank_balance = 302.13;
var amount = 99.99;

amount = amount * 2;

// can we afford the extra purchase?
if ( amount < bank_balance ) {
	console.log( "I'll take the accessory!" );
	amount = amount + ACCESSORY_PRICE;
}
// otherwise:
else {
	console.log( "No, thanks." );
}
```

这里，如果`amount < bank_balance`是`true`，我们将输出`"I'll take the accessory!"`，并且为我们的`amount`变量添加`9.99`。否则，`else`说我们会礼貌地回答`"No, thanks."`。并保持`amount`不变。

正如我们之前在"Values & Types"中讨论的那样，那些尚未达到预期类型的值通常会强制转换为该类型。`if`语句需要一个`boolean`值，但如果你传递的东西不是`boolean`值，那么就会发生强制转换。

JavaScript定义了一个被视为"falsy"的特定值列表，因为当强制转换为`boolean`值时，它们会变为`false` - 这些值包括`0`和`""`等值。不在"falsy"列表上的任何其他值自动被视为"truthy" - 当强制转换为`boolean`值时，它们变为`true`。Truthy值包括`99.99`和`"free"`之类的东西。有关详细信息，请参阅第2章中的"Truthy＆Falsy"。

条件除了`if`之外还存在其他形式。例如，`switch`语句可以用作一系列`if..else`语句的简写（参见第2章）。循环（参见"Loops"）使用条件来确定循环是应该继续还是停止。

**注意：** 有关可能在条件的测试表达式中隐式发生的强制的更深入信息，请参阅本系列的 *Types & Grammar* 标题的第4章。

## Loops

在繁忙时段，有一个等待名单，供需要与手机店员工交谈的客户使用。虽然名单上还有人，但她只需要继续为下一个客户服务。

重复一组动作直到某个条件失败 - 换句话说，只在条件成立时重复 - 就是程序循环的工作；循环可以采用不同的形式，但它们都满足这种基本行为。

循环包括测试条件和块（通常为`{..}`）。每次循环块执行时，都称为迭代。

例如，`while`循环和`do..while`循环形式说明了重复语句块直到条件不再为`true`：

```js
while (numOfCustomers > 0) {
	console.log( "How may I help you?" );

	// help the customer...

	numOfCustomers = numOfCustomers - 1;
}

// versus:

do {
	console.log( "How may I help you?" );

	// help the customer...

	numOfCustomers = numOfCustomers - 1;
} while (numOfCustomers > 0);
```

这些循环之间唯一的实际区别是条件是在第一次迭代（`while`）之前还是在第一次迭代之后（`do..while`）进行测试。

有时你循环用于计算某组数字，例如从`0`到`9`（十个数字）。你可以通过在值`0`处设置循环迭代变量（如`i`）并在每次迭代时将其递增`1`来实现。

**警告：** 由于各种历史原因，编程语言几乎总是以零基础方式计算事物，即从`0`开始而不是`1`开始。如果你不熟悉这种思维模式，一开始可能会让人很困惑。花一些时间从`0`开始练习计数，使变得更加适应！

每次迭代都会测试条件，就像循环中有一个隐含的`if`语句一样。

我们可以使用JavaScript的`break`语句来停止循环。另外，我们可以看到如果没有`break`机制，就会极其容易地创造一个永远运行的循环。

我们来说明一下：

```js
var i = 0;

// a `while..true` loop would run forever, right?
while (true) {
	// stop the loop?
	if ((i <= 9) === false) {
		break;
	}

	console.log( i );
	i = i + 1;
}
// 0 1 2 3 4 5 6 7 8 9
```

**警告：** 这不一定是你想要用于循环的实用形式。它仅供参考。

虽然有`while`（或`do..while`）可以手动完成任务，但还有另一种语法形式称为`for`循环：

```js
for (var i = 0; i <= 9; i = i + 1) {
	console.log( i );
}
// 0 1 2 3 4 5 6 7 8 9
```

如你所见，在两种情况下，条件`i <= 9`对于任一循环形式的前`10`次迭代（`i`值为`0`到`9`）都为`true`，但是当`i`为值`10`时变为`false`。

`for`循环有三个子句：初始化子句（`var i = 0`），条件测试子句（`i <= 9`）和更新子句（`i = i + 1`）。因此，如果要用循环迭代进行计数，`for`是一种更紧凑、更容易理解和编写的形式。

还有其他专门的循环形式，用于迭代特定的值，例如对象的属性（参见第2章），其中隐含的条件测试就是是否处理了所有属性。无论循环的形式如何，“循环直到条件失效”的概念都适用。

## Functions

手机店员工可能不会随身携带计算器来计算税款和最终购买金额。这是一个她需要定义一次的任务，一次又一次地重用。很有可能，该公司有一个内置“功能”的收银台（电脑、平板电脑等）。

同样，你的程序几乎肯定会将代码的任务分解为可重用的部分，而不是反复重复自己（双关语！）。这样做的方法是定义一个`function`。

函数通常是可以按名称“调用”的命名代码段，每次都会运行其中的代码。考虑：

```js
function printAmount() {
	console.log( amount.toFixed( 2 ) );
}

var amount = 99.99;

printAmount(); // "99.99"

amount = amount * 2;

printAmount(); // "199.98"
```

函数可以选择接受参数 - 传入的值。它们也可以选择返回一个值。

```js
function printAmount(amt) {
	console.log( amt.toFixed( 2 ) );
}

function formatAmount() {
	return "$" + amount.toFixed( 2 );
}

var amount = 99.99;

printAmount( amount * 2 );		// "199.98"

amount = formatAmount();
console.log( amount );			// "$99.99"
```

函数`printAmount()`接受一个我们称之为`amt`的参数。函数`formatAmount()`返回一个值。当然，你也可以将这两种技术结合在同一个功能中。

函数通常用于你计划多次调用的代码，但它们也可用于将相关的代码位组织到命名集合中，即使你只打算调用它们一次。

考虑下面的代码：

```js
const TAX_RATE = 0.08;

function calculateFinalPurchaseAmount(amt) {
	// calculate the new amount with the tax
	amt = amt + (amt * TAX_RATE);

	// return the new amount
	return amt;
}

var amount = 99.99;

amount = calculateFinalPurchaseAmount( amount );

console.log( amount.toFixed( 2 ) );		// "107.99"
```

尽管`calculateFinalPurchaseAmount()`仅被调用一次，但将其行为组织到单独的命名函数中会使其逻辑代码（`amount = calculateFinal ...`语句）更清晰。如果函数中有更多的陈述，那么好处将更加明显。

### Scope

如果你向手机店员工询问她的商店没有的手机型号，她将无法向你推销你想要的手机。她只能使用商店存货中的手机。你得去另一家商店看看能不能找到你要找的手机。

编程有一个术语用于这个概念：作用域（技术上称为 *词法范围* ）。在JavaScript中，每个函数都有自己的作用域。作用域基本上是变量的集合以及如何通过名称访问这些变量的规则。只有该函数内的代码才能访问该函数的作用域变量。

变量名在同一范围内必须是唯一的 - 不能有两个不同的`a`变量紧挨着彼此。但是相同的变量名称`a`可能出现在不同的范围内。

```js
function one() {
	// this `a` only belongs to the `one()` function
	var a = 1;
	console.log( a );
}

function two() {
	// this `a` only belongs to the `two()` function
	var a = 2;
	console.log( a );
}

one();		// 1
two();		// 2
```

此外，范围可以嵌套在另一个范围内，就像生日聚会中的小丑在另一个气球内吹出一个气球一样。如果一个范围嵌套在另一个范围内，则最内部范围内的代码可以从任一范围访问变量。

考虑下面代码：

```js
function outer() {
	var a = 1;

	function inner() {
		var b = 2;

		// we can access both `a` and `b` here
		console.log( a + b );	// 3
	}

	inner();

	// we can only access `a` here
	console.log( a );			// 1
}

outer();
```

词法范围规则表示一个范围内的代码可以访问该范围的变量或其范围之外的任何范围。

因此，`inner()`函数中的代码可以访问变量`a`和`b`，但是`outer()`中的代码只能访问`a` - 它不能访问`b`，因为该变量只在`inner()`内部。

回想一下前面的代码片段：

```js
const TAX_RATE = 0.08;

function calculateFinalPurchaseAmount(amt) {
	// calculate the new amount with the tax
	amt = amt + (amt * TAX_RATE);

	// return the new amount
	return amt;
}
```

`TAX_RATE`常量（变量）可以从`calculateFinalPurchaseAmount()`函数内部访问，即使我们没有传入它，因为词法范围的原因。

**注意：** 有关词法范围的更多信息，请参阅本系列的 *Scope & Closures* 标题的前三章。

## Practice

学习编程的实践绝对没有替代品。在我这，我写的再好也不能让你成为一名程序员。

考虑到这一点，让我们尝试练习本章中学到的一些概念。我会给出“要求”，然后先尝试一下。然后查看下面的代码清单，看看我是如何处理它的。

- 编写程序来计算购买手机的总价格。你将继续购买手机（提示：循环！），直到你的银行帐户资金不足为止。只要你的购买金额低于你的心理支出门槛，你还可以为每部手机购买配件。
- 在计算出购买金额后，添加税金，然后打印出计算出的购买金额，格式正确。
- 最后，根据你的银行帐户余额检查金额，看看你是否能负担得起。
- 你应该为“税率”，“手机价格”，“配件价格”和“支出门槛”设置一些常量，以及“银行帐户余额”的变量。
- 你应该定义用于计算税额和使用“$”格式化价格并四舍五入到小数点后两位的函数。
- **奖金挑战：** 尝试将输入合并到此程序中，也许可以使用前面“输入”中提到的 `prompt(..)`。例如，你可以提示用户提供银行帐户余额。玩得开心，有创意！

好的，继续吧。试试吧。在你自己给出一个方案之前，不要偷看我的代码清单！

**注意：** 因为这是一本JavaScript书，我显然会用JavaScript来解决练习练习。但是如果你感觉更舒服的话，你现在可以用另一种语言来做。

这是练习的JavaScript解决方案：

```js
const SPENDING_THRESHOLD = 200;
const TAX_RATE = 0.08;
const PHONE_PRICE = 99.99;
const ACCESSORY_PRICE = 9.99;

var bank_balance = 303.91;
var amount = 0;

function calculateTax(amount) {
	return amount * TAX_RATE;
}

function formatAmount(amount) {
	return "$" + amount.toFixed( 2 );
}

// keep buying phones while you still have money
while (amount < bank_balance) {
	// buy a new phone!
	amount = amount + PHONE_PRICE;

	// can we afford the accessory?
	if (amount < SPENDING_THRESHOLD) {
		amount = amount + ACCESSORY_PRICE;
	}
}

// don't forget to pay the government, too
amount = amount + calculateTax( amount );

console.log(
	"Your purchase: " + formatAmount( amount )
);
// Your purchase: $334.76

// can you actually afford this purchase?
if (amount > bank_balance) {
	console.log(
		"You can't afford this purchase. :("
	);
}
// You can't afford this purchase. :(
```

**注意： ** 运行此JavaScript程序的最简单方法是将其输入到浏览器的开发者控制台中。

你是怎么做的？你已经看过我的代码，再试一次也不会有什么坏处。并且改变一些常量来看看程序如何以不同的值运行。

## Review

学习编程不一定是一个复杂而一边倒的过程。你需要掌握一些基本概念。

些就像积木一样。要建造一座高塔，首先要将块放在块顶部的块顶部。编程也是如此。以下是一些基本的编程构建块：

- 你需要 *运算符* 对值执行操作
- 你需要值和类型来执行不同 *类型* 的操作，例如在`number`上进行数学运算，或者`string`输出
- 在程序执行期间，你需要 *变量* 来存储数据（也称为 *状态* ）。
- 你需要像`if`语句这样的 *条件* 来做决定。
- 你需要 *循环* 来重复任务，直到条件停止为真。
- 你需要使用 *函数* 将代码组织为逻辑和可重用的块。

代码注释是编写更易读代码的一种有效方法，这使得程序在出现问题时更容易理解，维护和修复。

最后，不要忽视实践的力量。学习如何编写代码的最好方法是编写代码。

现在，我很高兴你能够学习如何编码！请保持。不要忘记查看其他初学者编程资源（书籍，博客，在线培训等）。本章和本书是一个很好的开始，但它们只是一个简短的介绍。

下一章将回顾本章中的许多概念，但是从更具体的JavaScript角度来看，这将突出显示在本系列其余部分中更深入细节处理的大多数主要主题。