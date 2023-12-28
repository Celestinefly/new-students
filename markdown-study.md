# 这篇文章主要讲解markdown语法[^1]
（用markdown写文件的时候记得文件后面加后缀.md）
-----

### 第一部分：标题   
代码：
```markdown
# 一级标题   
## 二级标题   
### 三级标题   
#### 四级标题   
##### 五级标题  
###### 六级标题
```  
效果：   
# 一级标题      
## 二级标题      
### 三级标题       
#### 四级标题    
##### 五级标题      
###### 六级标题    
------   

### 第二部分：字体      
|代码|效果图|        
|:----:|:--:|        
|`*斜体*`|*斜体*|   
|`_斜体_`|_斜体_|   
|`**粗体**`|**粗体**|   
|`__粗体__`|__粗体__|    
|`***斜粗体***`|***斜粗体***|   
|`___斜粗体___`|___斜粗体___| 
|`<u>下划线</u>`|<u>下划线</u>|
|`~~删除线~~`|~~删除线~~|
>下划线表示法在github上不可用？

------

### 第三部分：换行   
Markdown换行的方式有很多种     
1.直接在一句话后敲两个空格,在加enter       
2.如果你在编辑的时候，想让一行文字在显示的时候换行，就在中间加`<br/>`   
|方式|代码|效果图|  
|:-:|:-:|:-:|
|1|`你好  `<br/>`世界`|你好<br/>世界|
|2|`你好<br/>世界`|你好<br/>世界| 

------

### 第四部分：引用    
Markdown中引用通过符号`>`来实现。`>`符号后的空格，可有可无。  
代码：  
```markdown
>你好，世界
```  
效果：  
>你好，世界

>注意 :heavy_exclamation_mark:：在引用的区块内，允许换行存在，换行并不会终止引用的区块。如果要结束引用，需要一行空白行，来结束引用的区块。（连续按三下enter键就知道了，你所看到的空白行，在效果图中不会出现，只会表现为换行）


举例说明：   
按三下enter后输入文字"你好"    
![按三下enter后输入文字"你好"](https://github.com/Celestinefly/keep-pictures/blob/0b21fccdcecf90918b18be86a591814c54314cdc/%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202023-12-27%20115123.png)    
效果图   
![效果图](https://github.com/Celestinefly/keep-pictures/blob/0b21fccdcecf90918b18be86a591814c54314cdc/%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202023-12-27%20115139.png)   


此外，引用还可以嵌套使用：<br/>
代码：<br/>
```markdown
>一级引用
>>>二级引用
>>>三级引用
```
效果：
>一级引用
>>二级引用
>>>三级引用
-----

### 第五部分：链接   

表示方法：[链接名称介绍](链接地址）或者<链接地址>  
代码：  
```markdown
[Celestinefly的github地址](https://github.com)
```   
或者      
```markdown
<https://github.com>
```   
效果：  
[Celestinefly的github地址](https://github.com)    
<https://github.com>    

-----    

### 第六部分：图片  
表示方法：! [图片描述，可写可不写，但是中括号要有] (图片地址，本地链接或者URL地址 "图片主题")(!,[],()之间不要空格，这里为了清楚表示，所以分开了.图片主题和图片地址要空格，图片主题可加可不加）       
代码：  
`![华中师范大学](https://pic3.zhimg.com/v2-9a475706794df67266e192e41e9b0f66_r.jpg "CCNU")`  
效果图：  
![华中师范大学](https://pic3.zhimg.com/v2-9a475706794df67266e192e41e9b0f66_r.jpg "CCUN")   
给图片增加链接，请将图像的Markdown 括在方括号中，然后将链接添加在圆括号中  
代码：  
`[把上面的代码放着里](图片的链接）`   
效果：  
[![华中师范大学](https://pic3.zhimg.com/v2-9a475706794df67266e192e41e9b0f66_r.jpg "CCNU")](https://pic3.zhimg.com/v2-9a475706794df67266e192e41e9b0f66_r.jpg）

------

### 第七部分：列表   
1. 无序列表，使用*、+、-，再加一个空格作为列表的标记   
2. 有序列表，使用数字并加上.号，再加一个空格作为列表的标记
>当你输入完第一个列表任务后，后enter会自动进入下一个列表内容书写，这里取消列表和取消引用一样，输入空白行，具体操作是按三下enter键
无序列表代码：
```markdown 
+ 你好   
* 世界   
- 你好
+ 未来
```
无序列表效果：  
+ 你好
+ 世界
+ 你好
+ 未来

有序列表代码：
```markdown
1. 你好   
2. 世界   
3. 你好   
4. 未来   
```
有序列表效果：
1. 你好
2. 世界
3. 你好
4. 未来

多级列表：  
在后一级列表输入*、+、-前，按Tab键   
无序列表二级列表代码： 
```markdown 
+ 你好  
+ 世界  
  + 你好  
  + 未来
```
效果：    
+ 你好
+ 世界

  + 你好
  + 未来
 
-----

### 第八部分：分割线
表示方法：三个及三个以上的`-`或者`*`表示  
代码：
```markdown
---  
--------  
*** 
******
```
效果：

---
---------
***
******
>注意 :heavy_exclamation_mark:：分割线上方必须空一行

当分割线输入是：
```markdown
你好，世界  
--- 
你好，未来  
```
所得到的效果：

你好，世界
---
你好，未来   
（你会发现分割线上下字体发生了变化）    

正确输入：   
```markdown
你好，世界  

---  
你好，未来
```     

所得到的效果：   
你好，世界

---
你好，未来

-----

### 第九部分：代码块  
表示方法：``引起来   
表示代码的代码：  
```markdown
`hello` world
```
效果：  
`hello` world    

表示代码块的代码：  
![golang代码](https://github.com/Celestinefly/keep-pictures/blob/d177fb6c031c467c89cf74e1265f2052f12fd147/%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202023-12-29%20045940.png)  
效果：  
```go
package main
import "fmt"
func main(){
   fmt.Println("hello,world")
}
```
支持的编程语言有：  
```markdown
bash
c，clojure，cpp，cs，css
dart，dockerfile, diff
erlang
go，gradle，groovy
haskell
java，javascript，json，julia
kotlin
lisp，lua
makefile，markdown，matlab
objectivec
perl，php，python
r，ruby，rust
scala，shell，sql，swift
tex，typescript
verilog，vhdl
xml
yaml
```

----

### 第十部分：表格  
|:-:|:-:|表示表格的结构  
+ `:-:`:表示表格里面的内容居中
+ `-:`:表示表格里面的内容居右
+ `:-`:表示表格里面的内容居左
+ `-`:表示表格里面的内容居左

|符号|文字相对单元格的位置|
|:-:|:-:|
|`:-:`|中|
|`-:`|右|
|`:-`|左|
|`-`|左|
>注意 :heavy_exclamation_mark:：`:`是英文的冒号

---

### 第十一部分：脚注  
```markdown
[^1]
```
你好，世界[^2]

---

### 第十二部分：制作待办事项    
表示方法`- [ ]` 表示未完成；`- [x]`表示已完成  
代码：  
```markdown
- [ ] 刷牙
- [ ] 洗脸
- [x] 吃早餐
```
效果：  
- [ ] 刷牙
- [ ] 洗脸
- [x] 吃早餐
>注意 :heavy_exclamation_mark:：`-空格[空格]`,或者`-空格[x]`

---

### 第十三部分：表情    
markdown支持表情包代码[^3]    
代码：   
`:satisfied:`    
效果：    
:satisfied:

[^1]:参考文献有：1.[Markdown官方教程](https://markdown.com.cn/)，2.[手把手教会你使用Markdown【从入门到精通一篇就够了】](https://blog.csdn.net/qq_40818172/article/details/126260661?ops_request_misc=%257B%2522request%255Fid%2522%253A%2522170358207316800213069001%2522%252C%2522scm%2522%253A%252220140713.130102334..%2522%257D&request_id=170358207316800213069001&biz_id=0&utm_medium=distribute.pc_search_result.none-task-blog-2~all~top_positive~default-1-126260661-null-null.142^v98^control&utm_term=markdown&spm=1018.2226.3001.4187)，
3.[CSDN 支持的＜markdown格式＞表情包大全分享](https://blog.csdn.net/m0_50546016/article/details/119087177?ops_request_misc=&request_id=&biz_id=102&utm_term=markdown%E8%A1%A8%E6%83%85%E5%8C%85&utm_medium=distribute.pc_search_result.none-task-blog-2~all~sobaiduweb~default-1-119087177.142^v99^control&spm=1018.2226.3001.4187)
[^2]:hello，world
[^3]:[表情包代码](https://blog.csdn.net/m0_50546016/article/details/119087177?ops_request_misc=&request_id=&biz_id=102&utm_term=markdown%E8%A1%A8%E6%83%85%E5%8C%85&utm_medium=distribute.pc_search_result.none-task-blog-2~all~sobaiduweb~default-1-119087177.142^v99^control&spm=1018.2226.3001.4187)

   










  



























