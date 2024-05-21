# 前言

正则表达式是一种模式或模板，允许您以一种自然而模糊的方式定义一组规则，从而使您能够匹配和验证文本。它们在几乎每种现代编程语言中都已经实现。

当处理任何类型的文本输入时，您并不总是知道值是什么，但通常可以假设（甚至要求）您将接收到应用程序中的格式。这些类型的情况正是您需要创建正则表达式来提取和操作此输入的情况。

在本书中，您将学习如何使用 JavaScript 中的正则表达式入门基础知识。我们将从基础知识开始，经过一些特殊模式，然后深入到两个示例中。第一个示例是验证 Web 表单，第二个是从日志文件中提取信息的非常复杂的模式。对于所有示例，我们将采用逐步方法，这将使学习和吸收本书所获得的所有知识变得更容易。

# 这本书涵盖了什么

第一章，“使用正则表达式入门”，介绍了 JavaScript 中正则表达式的概述。它还展示了如何开发用于测试前三章中使用的正则表达式的程序。

第二章，“基础知识”，介绍了 JavaScript 中正则表达式的主要特性，包括模糊匹配、乘法器和范围。

第三章，“特殊字符”，深入探讨了正则表达式的特殊字符模式。它涵盖了为正则表达式定义边界、定义非贪婪量词和定义带有组的正则表达式。

第四章，“实践中的正则表达式”，演示了如何开发 Web 表单并使用自第一章以来学到的正则表达式功能来验证其所有字段。

第五章，“Node.js 和正则表达式”，逐步解释了如何使用 Node.JS 创建一个简单的应用程序来读取和解析 Apache 日志文件。它还演示了如何将日志文件中的信息显示到用户友好的网页中。

附录 A，“JavaScript 正则表达式速查表”，总结了 JavaScript 中正则表达式使用的模式及其描述，以及一些有用的方法列表来测试和创建正则表达式。

# 您需要什么来阅读本书

要开发本书中提供的源代码，您需要任何您喜欢的文本编辑器和一个浏览器（如 Chrome 或 Firefox）。

对于第五章，“Node.js 和正则表达式”，您还需要在计算机上安装 Node.js。所有必需的步骤都在章节中描述。

# 这本书适合谁

这本书非常适合与任何类型的用户输入数据一起工作的 JavaScript 开发人员。本书适用于具有 JavaScript 正则表达式基础到中级技能的 JavaScript 程序员，他们想要第一次学习或加强自己的技能成为专家。

# 惯例

在本书中，您将找到一些区分不同信息类型的文本样式。以下是这些样式的一些示例及其含义的解释。

文本中的代码词、数据库表名、文件夹名、文件名、文件扩展名、路径名、虚拟 URL、用户输入和 Twitter 句柄显示如下：“现在，让我们看一下其中一些辅助函数，从`err`和`clearResultsAndErrors`开始。”

代码块设置如下：

```js
123-123-1234
(123)-123-1234
1231231234
```

任何命令行输入或输出都以以下方式编写：

```js
npm install http-server –g

```

**新术语**和**重要词汇**以粗体显示。屏幕上看到的词语，例如菜单或对话框中的词语，会以这样的方式出现在文本中：“以下图像举例说明了在给定**文本**输入时正则表达式的匹配。”

### 注意

警告或重要说明会显示在这样的框中。

### 提示

提示和技巧会显示为这样。