# 已部署参考基因组

截止到2018.5.3，分析平台中总计收录了279套不同物种及版本的参考基因组，其中225套是公开的，54套是用户私有的未公开的，其他用户不可见。279套参考基因组中，gff中带有gene name的有90套，具体的gene id 和 name样式可以参考下表，从表格中可以看出，一般研究比较多的，比较成熟的参考基因组会有gene symbol，而且是大家比较耳熟能详的名称，如人、鼠、水稻等，但是有些版本的参考基因组是没有gene symbol。

没有gene symbol的版本，可能这是该物种第一次发布参考基因组，贡献该基因组的课题组没有进行基因命名，而且即使提供了很可能也不是大家普遍认可的，因此意义不大；另外一类没有gene symbol，应该是课题组组装并注释完成后，没有和已有的版本（带有gene symbol）的版本去做对应，因此没有提供gene symbol，这一类如果要和已有gene symbol去对应，就需要将两个版本的gene序列通过blast进行比对，来获取到gene name。 

部署参考基因组时我们会基于：NR、GO、KEGG、Swiss-Prot、eggNOG、COG、KOG、Pfam这些功能数据库，对已知基因进行功能注释，最大程度保证基因功能信息是完善的。

{% includeCsv src="./public-reference-genome.csv", encoding="utf-8", useHeader="true" %}{% endincludeCsv %}