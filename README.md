# prompt-collection
My usual prompt

### 1. 英语单词本

#### 输入：

```xml
将英文单词转换为包括音标、中文翻译、英文释义、词根词源、助记和3个例句。中文翻译应以词性的缩写表示例如adj.作为前缀。如果存在多个常用的中文释义，请列出最常用的3个。3个例句请给出完整中文解释。注意如果英文单词拼写有小的错误，请务必在输出的开始，加粗显示正确的拼写，并给出提示信息，这很重要。请检查所有信息是否准确，并在回答时保持简洁，不需要任何其他反馈。第一个单词是“metroplitan”
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

### 2. 文章内容总结

### 输入

```xml
Write three easy-to-read sentences to summarize the following text:

"""
Title: {{ document.title }}
Author: {{ document.author }}
Domain: {{ document.domain}}
{#- The if-else logic below checks if the document is long. If so, it will use key sentences to not exceed the GPT prompt window. We highly recommend not changing this unless you know what you're doing. -#}
{% if (document.content | count_tokens) > 2000 %}
{{ document.content | central_sentences | join('\n\n') }}
{% else %}
{{ document.content }}
{% endif %}
"""


IMPORTANT: Write no more than THREE sentences. Each sentence should be short and easy-to-read. Use words sparingly and please capture the big idea.
```

### 输出

```xml
In the next few years, it's best to avoid crowded places for safety and well-being. High-energy environments like natural forests, quiet parks, libraries, and upscale malls can help uplift your mood and thoughts. Remember to prioritize personal space and avoid following the crowd to reduce risks and maintain inner peace.
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
```

#### 输出

```xml

Improved result:
If you want to write data to the database, you need to enable the button.

Reasons for changes:

Replaced "wangt" with "want" for correct spelling.
Added "need to" for clarity and to emphasize the requirement.
Changed "will" to "need to" to convey the necessity of enabling the button to achieve the desired action.
```



