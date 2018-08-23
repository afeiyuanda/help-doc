## 说明文档规范

### 文字规范

1. 需要强调的文字**加粗**
2. 平台上的`专用名词`、`按钮名称`、`功能名称`使用该效果进行提示


### 截图规范

1. 图片上用圈1、圈2 等表示步骤，可以在数字旁边用文字简要说明步骤内容；
2. 用红色方框标出需要强调的部分；
3. 尽量不使用箭头，即使使用，不要满屏都是箭头
4. 图片可以和文档放在一起，文档中用相对路径引入图片即可，如：```![fasta](./file-format-intro/fasta.png)```

~~4. 图片素材放到图片服务器，一个文档中的图片放到一个文件夹中，目录结构和文档目录结构保持一致~~
~~使用[filezilla](http://sw.bos.baidu.com/sw-search-sp/software/090246a8f0734/FileZilla_3.24.0.0_win64-setup.exe)等ftp软件~~

~~* 登录sftp://10.3.128.98~~
~~* 账号：img_docs~~
~~* 密码：123.img_docs~~
~~* 上传路径：/share/SYSTEM_biocloud/static.biocloud.net/img/docs/~~
~~* 使用时图片的url：https://img.biocloud.net/docs/picname~~
~~* 例如上传了一张test.png，则图片url为：https://img.biocloud.net/docs/test.png~~

### 格式规范

#### 一般可以分为两个版块
1. 功能模块标题及功能简介
2. 操作使用说明（操作流程及功能特点）

#### 版块标号
1. 功能模块标题是二级标题，其他标题用三级和四级，根据段落层次自己把握
2. 具体的操作步骤需要起一个标题，并使用阿拉伯数字标号，另起段落描述具体的步骤

### 内容规范
#### 包括的内容

1. 功能模块标题，功能模块简介
2. 功能模块操作概要。文字尽量精简
3. 描述中有与其他模块相关连的，可以通过链接的方式进行提示，不属于该功能的就不要再展开说明了，用户可以通过点击链接跳转到相关页面

比如：
* 分析平台与套餐的关系--可以通过链接的方式链接到"会员"的使用说明页面；
* 通用模块说明写到单独页面，在系统介绍中进行引用，如参考基因组的选择需要注意哪些事项，fold change怎么选择，新增差异分组功能说明等等。
4. 需要解释强调和提示的内容按照如下处理方式

重要信息提示：

> ![warn](./basic-img/warning.png)同一份极速体验报告生成之后不会再重复生成了，可先删除再重新提交

### 参考文档
* [Markdown入门指南](http://note.youdao.com/group/#/70235902/(folder/185150327//full:md/185150531)?full=true)
* [极速体验文档](http://note.youdao.com/group/#/70235902/(folder/185150553//full:md/185204644)?full=true)

~~文档编写统一使用`有道云笔记`中的`云协作`进行~~