# 创建或更新记录

---

## 请求地址

- /review/v1/tasks/:task/records/:record

## 请求方式

- PUT

## 地址参数

| 参数   | 是否必填 | 描述     |
| :----- | :------- | :------- |
| task   | 是       | `任务`ID |
| record | 是       | `记录`ID |

##  请求参数

| 参数    | 是否必填 | 描述                                                         |
| :------ | :------- | :----------------------------------------------------------- |
| ak      | 是       | `任务`的API访问秘钥                                          |
| time    | 是       | `记录`提交时间，序列化时间<br>&#9;如：1436595149269          |
| content | 是       | `记录`内容，需通过encodeURI()进行RUI编码                     |
| type    | 是       | `记录`类别 <br>&#9;- c : C语言源文件 <br>&#9;- cpp : C++源文件 <br>&#9;- java : Java源文件 <br>&#9;- text : 文本文件 |