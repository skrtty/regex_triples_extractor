# regex_text_labeler 使用说明

这是一个利用正则表达式对文本进行抽取或者标注的项目。

Python环境：Python 3.7.9

### 一、用户定义文件格式说明

+ **template.json**

  该文件定义属性对应的模板规则，用户可以遵循下列规则修改或添加自己的模板：
  
  1. json数据的内容格式满足{'属性':'属性对应正则表达式'}，不符合格式的数据将导致报错。
  2. 同一属性可以对应多个正则表达式。
  3. 不可以出现重复的规则(即属性和属性对应正则表达式完全一致)，否则会导致报错。


+ **source_data.json**

  该文件定义了需要处理的格式：
  
  1. json数据的内容格式需满足{'实体名':'文本'}，不符合格式的数据将导致报错。

### 使用方式

【开发中...啊吧啊吧啊吧】



### 输出文件

+ **extracted_triple.txt**

  抽取的三元组将会输出至这个txt当中，会以实体;;;;属性;;;;属性值的形式表示三元组，其中每一个三元组占一行，以四个分号“;;;;”作为行内分隔符

+ **labeled_data.json**：

  标注后的数据会以【【属性;;;;内容】】的

在再次运行程序时，目录下已有的同名文件会被覆盖，请注意及时保存。



