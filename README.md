# prompt-collection
My usual prompt

### 英语单词本

#### 输入：

```xml
将英文单词转换为包括音标、中文翻译、英文释义和3个例句。中文翻译应以词性的缩写表示例如adj.作为前缀。如果存在多个常用的中文释义，请列出最常用的3个。3个例句请给出完整中文解释。注意如果英文单词拼写有小的错误，请务必在输出的开始，加粗显示正确的拼写，并给出提示信息，这很重要。请检查所有信息是否准确，并在回答时保持简洁，不需要任何其他反馈。第一个单词是“metroplitan”
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



