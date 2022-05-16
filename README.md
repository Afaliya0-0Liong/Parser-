# Parser-
编译原理课程设计：语法分析器

要求：
  创建一个使用LR(1) 方法的语法分析程序，程序有两个输入：1）一个是文本文档，其中包含2º型文法（上下文无关文法）的产生式集合；2）任务1词法分析程序输出的（生成的）token令牌表。程序的输出包括：YES或NO（源代码字符串符合此2º型文法，或者源代码字符串不符合此2º型文法）；错误提示文件，如果有语法错标示出错行号，并给出大致的出错原因。
  
开发环境：
  Windows10、python(PyCharm)环境。

项目简介：
  程序读入上下文无关文法，并进行拓广文法，将产生式依次形成项目进行储存，设定好起点进行处理得到完整的项目集族，按照项目集族之间的转换得到action、goto表，读取词法分析得到的token（详情看我的词法分析器，也可以按照我的格式进行自创，格式：(行数, token分类, token内容)），按照之前得到的action、goto表进行处理，得到语法分析的结果，查看是否符合自己设定的语法，如果出错可以形成缺失者错误导致的错误报告，并输出到result.txt（正确会得到‘YES’）。
  
 详细讲解请移步：
 https://blog.csdn.net/RLIRiong/article/details/124809191?csdn_share_tail=%7B%22type%22%3A%22blog%22%2C%22rType%22%3A%22article%22%2C%22rId%22%3A%22124809191%22%2C%22source%22%3A%22RLIRiong%22%7D&ctrtid=wRASS
