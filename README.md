# prompt-collection

My usual prompt

### 英语单词本

#### 输入：

```xml
将英文单词转换为包括音标、中文翻译、英文释义和3个例句
中文翻译有词性的缩写表示例如 adj.
如果存在多个常用的中文释义，请列出最常用的3个
3个例句请给出完整中文解释
注意如果英文单词拼写有小的错误，请务必在输出的开始，加粗显示正确的拼写，并给出提示信息，这很重要
请检查所有信息是否准确，并在回答时保持简洁，不需要任何其他反馈
第一个单词是“metroplitan”
```

### 输出：

```xml
metropoli****tan 正确的拼写是 metropolitan

metropolitan [ˌmɛtrəˈpɒlɪtn]
adj.大城市的,都会的
n.主教

词根词源:来自希腊语 meter 意为"母亲"和 polis 意为"城市"
助记:metro就是地铁,polis就是城市,这个单词描述的就是大城市

大城市里有许多摩天大楼和商业中心。
Metropolitan areas usually have skyscrapers and business districts.

大都会区往往拥有繁华的夜生活。
Metropolitan areas often have a vibrant nightlife.

纽约是一个主要的国际大都会。
New York is a major international metropolitan area.
```

### 英语语法纠正

#### 输入

```xml
Please optimize the grammar and provide the improved result along with the reasons for the changes. For example, if I provide:
If you want to write data to the database, you will enable the button
Your output should be:
Improved result:
If you wish to save data to the database, you must activate the button.
Reasons for changes:
Replaced "want" with "wish" for a more formal tone.
Changed "write" to "save" for clarity and accuracy.
Strictly follow the following format
Original sentence: ###origin input###
Improved result: ###your out###
Reasons for changes:
    ### changes 1 ### 
    ### changes 2 ### 
    ### changes n ###
    ...
Additional considerations:
    ### consideration content ###
    ### consideration content ###

such as:
my input: If you want to write data to the database, you will enable the button.
your output:

Original sentence: If you want to write data to the database, you will enable the button.
Improved result: To save data to the database, activate the button.
Reasons for changes:
Conciseness: The sentence has been shortened by removing unnecessary words like "if" and "you" while maintaining the original meaning.
Clarity: "Write data" has been replaced with the more precise term "save data," accurately reflecting the action's purpose.
Active voice: The sentence has been changed from passive voice ("you will enable") to active voice ("activate"), making it sound more direct and engaging.
Additional considerations:
Depending on the context, it might be beneficial to specify what kind of data is being saved and what button needs activating.
If the action is conditional, rephrasing with "if" might still be appropriate, but ensuring the sentence structure is clear and concise.
```

#### 输出

```xml
[
{
"Original sentence": "if you want save data to databases, please enable the start button.",
"Improved result": "To save data to the database, please activate the Start button.",
"Reasons for changes": {
"Conciseness and clarity": "Removed unnecessary "if" and "you", changed "save" to the more precise "save data", and specified "the database" instead of the plural "databases".",
"Formality and active voice": "Replaced "enable" with the more formal "activate" and rephrased the sentence to use active voice."
},
"Additional considerations": {
"Capitalization": "Consider capitalizing "Start button" if it refers to a specific button label in the user interface."
}
}
]
```







## 变量命名

"我需要你帮我的代码变量命名，使用清晰、描述性的名称，在不影响可读性的前提下尽量减少字符数。变量名应能清楚地表达它们所代表的值或目的，避免使用单字母或模糊的缩写。确保变量名符合 Python 命名规范，并清楚地表达变量的含义。\n我给你输入一段描述，这段描述可能是这段代码的功能\n你给我输出变量名称，要求在5个单词内，多个单词需要使用_连接,给出多个方案让我备选\n比如：\n我的输入：“数据库名称”\n你的输出: database_name、db_name"

## 代码优化

"优化当前的 Python 代码，确保变量名符合 PEP 8 命名规范，提高代码的可重用性，并尽可能简化代码。请提供优化代码的建议，包括改进变量命名、提高代码重用性和简化代码结构的建议。您的建议应旨在提高代码的整体可读性、可维护性和效率。此外，请考虑提供具体示例或解释，以支持您的优化建议。"

## 代码解释器

作为 Python 专家，您的任务是提供有关 Python 代码和计算机基础知识的详细而清晰的解释。具体来说，你应该\n\n1. 解释代码背后的功能和逻辑推理，包括算法和数据结构的相关知识。\n2. 分析代码在计算机上的执行过程，并解释其基本原理，如内存管理、CPU 指令和操作系统。\n3. 针对代码中的任何性能问题提出优化建议。\n\n我们会向您提供 Python 代码片段或有关代码某些部分的具体问题。您的解释应旨在通过提供详细而清晰的见解，加深对 Python 代码和计算机基础知识的理解。\n\n您的回答应全面且通俗易懂，有助于接收者的学习和成长。\n\n请注意，您的解释应足够灵活，以适应各种与 Python 相关的询问和优化建议。"
