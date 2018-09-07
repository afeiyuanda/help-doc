# 名词解释
|英文名词|中文名词|英文解释|中文解释|
|:---|:---|:---|:---|
|Clean Data|||Raw data需要进行一系列处理，比如去除测序接头以及引物序列，过滤低质量值数据等等，之后得到的高质量reads，称之为Clean Data。|
|Raw Data|原始数据||一次测序产生的没有经过任何过滤的全部原始数据。|
|Q20|||碱基测序质量值，Q20代表测序准确度在99%。|
|Q30|||碱基测序质量值，Q30代表测序准确度在99.9%。|
|Sequencing by Synthesis, SBS|边合成边测序||第二代测序技术的核心思想是边合成边测序，即通过捕捉新合成的末端的标记来确定DNA的序列。|
|Reads|读长||高通量测序仪产生的一小段测序片段。|
|Quality Score|碱基质量值||是碱基识别（Base Calling）出错的概率的整数映射。碱基质量值越高表明碱基识别越可靠，碱基测错的可能性越小。|
||碱基互补配对原则||在DNA或某些双链RNA分子结构中，由于碱基之间的氢键具有固定的数目和DNA两条链之间的距离保持不变，使得碱基配对必须遵守一定的规律，这就是Adenine与Thymine，在RNA中与Uracil配对，Guanine与Cytosine配对，反之亦然。碱基间的这种一一对应的关系叫做碱基互补配对原则。|
|Base Calling|碱基识别|The process of assigning bases (nucleobases) to chromatogram peaks. One computer program for accomplishing this job is Phred base-calling, which is a widely used basecalling software program by both academic and commercial DNA sequencing laboratories because of its high base calling accuracy|测序时，先成像，成像后根据信噪比确定碱基的类型和质量分数|
|FASTQ|||第一行以@开头，后面是序列标识（ID）以及其他可选的描述信息；第二行为碱基序列，即Reads；第三行以+开头，后面接着是可选的描述信息；第四行是Reads每个碱基对应的质量打分编码，长度必须和Reads的序列长度相同，该行中每个字符对应的ASCII值减去33/64，即为对应的质量值。|
|FASTA|||是以&gt;开始的一行储存序列的描述信息；其余行是序列部分。|
|de novo|||de novo测序也称为从头测序，不需要任何现有的序列资料就可以对某个物种进行测序，利用生物信息学分析手段对序列进行拼接，组装，从而获得该物种的基因组。|
|Mate pair||The sequence obtained from opposite ends of a particular clone are referred to as mate pairs. Knowing that two sequences are derived from the same clone allows these sequences to be linked, even if the full insert of the clone is unavailable. This is key to WGS assemblies.|将很长的DNA进行环化,环化的接口处连接识别序列,然后打断,富集含有识别序列的DNA,再进行双向测序,那么双向测序的插入片段长度就会很长.|
|Pair end|双端测序||直接在DNA两端加上接头进行双向测序,插入片段长度较短|
|Fosmid||A cloning system based on the E. coli F factor. These clones have an average insert size of 40 Kb, with a very small standard deviation.||
|Cosmid||Cloning vector that typically contains insert sizes of 60-120kb. These vectors are hybrids of lambda phages and plasmids and can be propagated as plasmids or packaged like phage. The name comes from the fact that these vectors retain the phage cos sites that are used for lambda head stuffing. These are generally maintained in multiple copies in E. coli.||
|MP-Reseq|多混池全基因组重测序||针对特有的优良地方品种中的不同品种/品系，通过群体内 pooling 建库的方法，进行全基因组重测序，采用生物信息学方法全基因组范围内扫描变异位点，能快速的定位不同混池样品基因组中明显经过人工或自然选择的区域，检测与性状相关的基因区域及其功能基因。|
|Contig|||由reads通过对overlap区域拼接组装成的没有gap的序列段。|
|Scaffold|||通过pair ends信息确定出的contig排列，中间有gap。|
|N50|||把组装出的contigs或scaffolds按照由长到短排列，当其累计长度刚刚超过全部组装序列总长度50%时，最后一个contig或scaffold的大小即为N50的大小。|
|coverage|测序覆盖度||由于基因组中的高GC、 重复序列等复杂结构的存在，测序最终拼接组装获得的序列往往无法覆盖所有的区域，覆盖到的区域占基因组的比例即测序覆盖度，没有获得的覆盖到区域就称为Gap。|
|Draft Sequence|基因组草图|Draft sequence is unfinished genomic or cDNA sequence||
|physical map|物理图谱||利用限制性内切酶将染色体切成片段，再根据重叠序列确定片段间连接顺序，以及遗传标志之间物理距离碱基对(bp) 或千碱基(kb)或兆碱基(Mb)的图谱。|
|Domain|结构域|A domain is a discrete structural unit of a protein. In principle, protein domains are capable of folding independently from the rest of the protein. Domains can often be identified by non-structural approaches based on conserved amino acid sequences.||
|Motif|保守域|A motif is a short, well-conserved nucleotide or amino acid sequence that represents a minimal functional domain. It is often a consensus for several aligned sequences.|指不同的蛋白质的氨基酸序列或不同基因中核苷酸序列的相似区域，就是所谓的保守区。|
|tRNA|转运RNA|Transfer Ribonucleic Acid|是具有携带并转运氨基酸功能的类小分子核糖核酸。|
|rRNA|核糖体RNA||是最多的一类RNA，也是3类RNA（tRNA,mRNA,rRNA)中相对分子质量最大的一类RNA，它与蛋白质结合而形成核糖体，其功能是在mRNA的指导下将氨基酸合成为肽链|
|miRNA|小RNA||MicroRNA (miRNA) 是一类内生的、长度约为20-24个核苷酸的小RNA，其在细胞内具有多种重要的调节作用，参与转录后基因表达调控。每个miRNA可以有多个靶基因，而几个miRNA也可以调节同一个基因。|
|simple-DNA|单拷贝蛋白序列||在单倍体基因组中只出现一次，因而复性速度很慢。|
|4DTV|四倍简并位点||密码子的第三位碱基无论转换为哪种核苷酸，该密码子都编码同一种氨基酸的位点。|
|nonsynonymous mutation, Ka|非同义突变||会导致氨基酸改变的核苷酸变异|
|synonymous mutation, Ks|同义突变||不导致氨基酸改变的核苷酸变异|
|secreted protein|分泌蛋白||是指在细胞内合成后，分泌到细胞外起作用的蛋白质。例如：唾液淀粉酶，胃蛋白酶，消化酶，抗体和一部分激素。|
|signal peptide|信号肽||是引导新合成的蛋白质向分泌通路转移的短（长度5-30个氨基酸）肽链。|
|Secondary metabolism|次级代谢产物||指生物生长到一定阶段后通过次级代谢合成的分子结构十分复杂、对该生物无明显生理功能，或并非是该生物生长和繁殖所必需的小分子物质，如抗生素、毒素、激素、色素等。|
|Cytochrome P450|细胞色素P450||为一类亚铁血红素—硫醇盐蛋白的超家族，它参与内源性物质和包括药物、环境化合物在内的外源性物质的代谢。|
|Proteases|蛋白酶||水解蛋白质肽链的一类酶的总称。按其降解多肽的方式分成内肽酶和端肽酶两类。|
|Nuclear localization signals|核定位信号||蛋白质的一个结构域，通常为一短的氨基酸序列，它能与入核载体相互作用，使蛋白能被运进细胞核。|
|Kinomes|激酶||一类从高能供体分子(如ATP)转移磷酸基团到特定靶分子(底物)的酶，这一过程谓之磷酸化。|
|paralogy|旁系同源||是那些在一定物种中的来源于基因复制的蛋白，可能会进化出新的与原来有关的功能。|
|orthology|直系同源||指的是不同物种之间的同源性，例如蛋白质的同源性，DNA序列的同源性。|
|alternative splicing|可变剪接||有些基因的一个mRNA前体通过不同的剪接方式（选择不同的剪接位点）产生不同的mRNA剪接异构体，这一过程称为可变剪接|
|Gene Flow|基因流||指生物个体从其发生地分散出去而导致不同种群之间基因交流的过程，可发生在同种或不同种的生物种群之间。|
|Optical Mapping|光学映像|A light microscope based technique in which images of single DNA molecules undergoing restriction enzyme digest are recorded and used for the construction of physical maps of large pieces of DNA. Optical maps often serve as scaffolds for the precise alignments of sequence contigs that are generated during genome sequencing projects.||
|HTGS|高通量基因组序列|This is a term to distinguish all genomic sequence generated in a high-throughput manner. In order to release data more rapidly, it became standard for all sequence centers to submit unfinished sequence into public repositories (the &quot;Bermuda Rules&quot;). This sequence is deposited into the HTG division of GenBank/EMBL/DDBJ. In general, these terms are used to describe clone (BAC/PAC/fosmid) based projects.||
|CDS|编码序列|Coding sequence. This is the portion of an mRNA or genomic sequence that encodes for a protein sequence.|在核酸序列中能够翻译成蛋白质氨基酸序列的部分，该段核酸序列要有起始与终止密码子。|
|Transposase|转座酶||执行转座功能的酶，通常由转座子编码，识别转座子两端的特异序列，能把转座子从相邻序列中脱离出来，再插入到新的DNA靶位点，无同源性要求。|
|segmental duplication|基因组复制|A region of genomic DNA ranging from 1 to 400kb that may be found at more than one site in the genome. Segmental duplications often share &gt;90% sequence identity.||
|SVG|可伸缩向量图形||可缩放矢量图形是基于可扩展标记语言（标准通用标记语言的子集），用于描述二维矢量图形的一种图形格式|
|ChIP-Seq, Chromatin Immunoprecipitation|染色质免疫沉淀|A technique involving size selection, high throughput sequencing (typically using next generation sequencing technologies that produce millions of reads in a run) and mapping of ChIP purified DNA onto a reference genome to achieve genome-wide identification of protein-DNA interactions.|是一种适用于研究蛋白质与生物体细胞中 DNA 相互作用的经典方法，将 ChIP 与第二代测序技术相结合的 ChIP-Seq 技术，能够高效地在全基因组范围内检测与组蛋白、转录因子等互作的 DNA 区段，研究体内转录因子和靶基因启动子区域直接相互作用的方法，对于调控蛋白在基因组上的结合靶点筛选、差异化表观遗传变异的原理揭示提供了重要的解决思路。|
|Linkage Mapping|遗传图|连锁分析|This type of mapping measures meiotic recombination using polymorphic markers to produce the relative order of markers with respect to each other. Distance between markers is measured in centiMorgans (cM). A centiMorgan is equivalent to a 1% cross-over rate.||
|EST Expressed sequence tag|表达序列标签|These are single-pass sequences of cDNA clones. Databases of EST sequences are highly redundant but quite useful for gene identification. There are many efforts to cluster EST sequences to remove the redundancy and low-quality sequences.|是从一个随机选择的cDNA 克隆，进行5’端和3’端单一次测序挑选出来获得的短的cDNA 部分序列。|
|Phenotype|表型|An observable characteristic displayed by an organism. These characteristics can be controlled by genes, by the environment, or a combination of both. The characteristic can be directly observable, such as having brown eyes. In some cases, the phenotype will be measurable, such as having high blood pressure.|指个体形态、功能等各方面的表现，如身高、肤色、血型、酶活力、药物耐受力乃至性格等等。 就是说个体外表行为表现和具有的行为模式。|
|RFLP|限制性片段长度多态性|Restriction fragment length polymorphism. A type of polymorphism detectable in a genome by the size differences in DNA fragments generated by restriction enzyme analysis.||
|WGAC|全基因组组装|A computational method that detects identity between long stretches of genomic sequence, revealing regions of segmental duplication.||
|WGS|全基因组鸟枪法|Whole Genome Shotgun. A sequencing method by which an entire genome is cut into chunks of discrete sizes (usually 2,10, 50 and 150 Kb) and cloned into an appropriate vector. The ends of these clones are sequenced. The two ends from the same clone are referred to as mate pairs. The distance between two mate pairs can be inferred if the library size is known and should have a narrow window of deviation.|是在获得一定的遗传及物理图谱信息的基础上，绕过bac克隆逐个排序的过程，将基因组dna分解成2kb左右的小片段进行随机测序，辅以一定数量的10kb的克隆和bac克隆的末端测序，利用超级计算机进行整合进行序列组装。|
|YAC|酵母人工染色体|Yeast artificial chromosome. These cloning vectors were developed using yeast centromere and telomere sequences. The average insert size of these clones ranges from 100-1000 Kb. These clones can span large portions of the genome but can be highly unstable.||
|Stem Cells|干细胞|Most cells of the adult body are terminally differentiated, that is, they are no longer able to replace themselves or to become another cell type. Stem cells are undifferentiated cells that are able to both proliferate and differentiate into numerous cell types. For example, embryonic stem cells are able to differentiate into any cell type found within the embryo, where as hematopoietic stem cells can differentiate into any blood cell.|是一类具有自我复制能力的多潜能细胞。在一定条件下，它可以分化成多种功能细胞。|
|Haplotype|单体型|A set of closely linked genetic markers present on one chromosome that tend to be inherited together. A haplotype may also refer to a set of single nucleotide polymorphisms (SNPs) on a single chromatid that are statistically associated with one another.||
|BLAT||A hashing algorithm developed by Jim Kent to allow rapid searching of large amounts of genome sequence. A hashing algorithm divides the database into words of a prescribed size (often 12-14 bases). The locations of these words are stored in memory. The query sequence is scanned for exact matches to words stored in memory. These types of algorithms tend to be very fast and effective for closely related sequences, but fail as sequences diverge. In addition to nucleotide BLAT, translated BLAT allows for comparison of protein sequences. This sequence aligner also allows for accurate alignment of transcribed sequences by looking at splice site information.|可以称为类BLAST 比对工具，对于DNA序列，BLAT是用来设计寻找95%及以上相似至少40个碱基的序列。|
|BLAST||Basic Local Alignment Search Tool. A method for performing sequence comparisons. Either protein sequences or nucleotide sequences can be used. This algorithm has been extended and now includes a suite of programs including megaBLAST and discontiguous megaBLAST.|局部序列比对基本检索工具|
|Accession number|登录号|An accession number is a unique identifier given to a sequence when it is submitted to one of the DNA repositories (GenBank, EMBL, DDBJ). The initial deposition of a sequence record is referred to as version 1. If the sequence is updated, the version number is incremented but the accession number will remain constant.||
|degeneracy|密码子的简并||指同一种氨基酸具有两个或者更多个密码子的现象|
|SNP|单核苷酸多态性|Single Nucleotide Polymorphism. A single base difference found when comparing the same DNA sequence from two different individuals.|主要是指在基因组水平上由单个核苷酸的变异所引起的DNA序列多态性。|
|InDel|插入缺失||指的是两种亲本中在全基因组中的差异，相对另一个亲本而言，其中一个亲本的基因组中有一定数量的核苷酸插入或缺失，根据基因组中插入缺失位点，设计一些扩增这些插入缺失位点的PCR 引物。|
|CNV, copy number variation|拷贝数变异|Large-scale structural changes in DNA that vary from individual to individual. These include insertions, deletions, duplications and complex multi-site variants that range from kilobases to megabases in size.|指在人类基因组中广泛存在的，从1000bp(碱基对)到数百万bp范围内的缺失、插入、重复和复杂多位点的变异。|
|allele frequency|等位基因频率||是群体遗传学的术语，用来显示一个种群中基因的多样性，或者说是基因库的丰富程度。|
|QTL quantitative trait locus|数量性状基因座||指的是控制数量性状的基因在基因组中的位置。|
|inkage disequilibrium|连锁不平衡（LD）||在某一群体中，不同座位上某两个基因同时遗传的频率明显高于预期的随机频率的现象|
|Chromosomal rearrangement|染色体重排|These are events that are mediated by double-strand breaks and subsequent repair occurring in the genome. When these breaks are repaired the location of landmarks in the genome have often changed or have been removed completely.||
|SLAF-seq|简化基因组测序|Specific-Locus Amplified Fragment Sequencing|是特异位点扩增片段测序，是基于酶切的简化基因组测序技术，通过对酶切获得的SLAF tag进行高通量测序，大幅降低基因组的复杂度，操作简便，同时不受参考基因组的限制，可快速鉴定出高密度的SNP位点，性价比高、稳定性好。该技术可用 来研究群体进化、遗传图谱构建及QTL定位以及目标性状关联分析。|
|GWAS, Genome-wide association study|全基因组关联分析||通过重测序对动植物重要种质资源进行全基因组基因型鉴定，与关注的表型数据进行全基因组关联分析，找出与关注表型相关的SNP位点，定位数量性状基因，与数量性状相关的基因紧密连锁的SNP标记，后续可用于分子标记辅助育种，助力育种进程。|
|Microbime diversity|微生物多样性测序||环境微生物多样性分析是直接从样品中提取基因组 DNA 后进行测序分析。它是通过对环境中微生物 16S/18S/ITS rDNA高变区 的 PCR扩增产物进行高通量测序，分析该环境下微生物群落的多样性和分布规律，对于我们研究微生物与环境的关系，环境治理和微生物资源的利用有着重要的理论和现实意义。|
|Metagenome|宏基因组||是由 Handelsman 等 1998 年提出的新名词, 其定义为 the genomes of the total microbiota found in nature, 即生境中全部微小生物遗传物质的总和。它包含了可培养的和未可培养的微生物的基因组，目前主要指环境样品中的细菌和真菌的基因组总和。|
|Super BSA, Super bulk segregant analysis|超级混池分离分析法||是快速有效地寻找与目的基因紧密连锁分子标记的经典方法，广泛应用于作物育种。将简化基因组测序SLAF-seq与传统BSA相结合的Super BSA，能更快速、准确、精细定位目标性状，具有混池规模大、标记密度高、数字化定量统计基因型频率等诸多优点。|
|domestication|驯化||是指外来植物通过改变其遗传性状以适应新环境的过程，如将动物从野生状态改变为家养或栽培的过程就称为驯化。|
|evolution|进化||是指一些生命形态发生、发展的演变过程。|
|Association Region|关联区域||通过关联分析分析得到的与目标性状相关联的区域|
|Enrichment Analysis|富集分析||对关联区域内的注释基因进行功能分类，增加研究的可靠性，并获得可能与性状相关的生物过程|
|cDNA|互补DNA||与RNA链互补的单链DNA，以其RNA为模板，在适当引物的存在下，由RNA与DNA进行一定条件下合成的，就是cDNA。|
|TopHat2|||TopHat2将Clean Reads与参考基因组进行序列比对，获取在参考基因组或基因上的位置信息，以及测序样品特有的序列特征信息。TopHat2是以比对软件Bowtie2为基础，将转录组测序Reads比对到基因组上，通过分析比对结果识别外显子之间的剪接点（Splicing Junction）。这不仅为可变剪接分析提供了数据基础，还能够使更多的Reads比对到参考基因组，提高了测序数据的利用率。|
|Bowtie2|||Bowtie2是将测序reads比对到长参考序列上的常用生物信息学分析软件，将50~1,000bp的reads比对到相对较长的基因组上时表现最佳。|
|Splicing Junction|剪接点||外显子与内含子的分界点。|
|mRNA|信使RNA||信使核糖核酸，携带遗传信息，在蛋白质合成时充当模板的RNA。它在核糖体上作为蛋白质合成的模板，决定肽链的氨基酸排列顺序。|
|Exon|外显子||是真核生物基因的一部分，它在剪接后仍会保存下来，并可在蛋白质生物合成过程中被表达为蛋白质。|
|Intron|内含子||内含子是真核生物细胞DNA中的间插序列。这些序列被转录在前体RNA中，经过剪接被去除，最终不存在于成熟RNA分子中。|
|intergenic region|基因间区||指基因与基因之间的间隔序列，不属于基因结构，不直接决定氨基酸，可能通过转录后调控影响性状的区域。|
|split gene|断裂基因||真核生物结构基因，由若干个编码序列和非编码序列互补间隔开但又连续镶嵌而成，去除非编码序列再连接后，可翻译出由连续氨基酸组成的完整蛋白质，这些基因称为断裂基因。|
|RNA editing|RNA编辑||是指在mRNA水平上改变遗传信息的过程。具体来说，指基因转录产生的mRNA分子中，由于核苷酸的缺失，插入或置换，基因转录物的序列不与编码序列互补，使翻译生成的蛋白质的氨基酸组成，不同于基因序列中的编码信息现象。|
|RPKM, Reads Per Kilobase Million|||将map到基因的read数除以map到genome的所有read数(以million为单位)与RNA的长度(以KB为单位)。|
|FPKM, Fragments Per Kilobase Million|||将map到基因的fragment数除以map到genome的所有fragment数(以million为单位)与RNA的长度(以KB为单位)。|
|up regulation|上调||调控结果使基因表达水平提高的称为正向调控，即上调。|
|Down regulation|下调||调控结果使基因表达水平降低的称为负向调控，即下调。|
|differential expression gene|差异表达基因||指在两个不同条件（如对照与处理、野生型和突变型、不同时间点、不同组织等）下，表达水平存在显著差异的基因，称之为差异表达基因。|
|differential expression of transcription|差异表达转录本||指表达水平存在显著差异的转录本。|
|Pearson correlation coefficient|皮尔逊相关系数||用于度量两个变量X和Y之间的相关（线性相关），其值介于-1与1之间。其中，1表示变量完全正相关，0表示无关，-1表示完全负相关。在高通量测序中，将皮尔逊相关系数作为生物学重复相关性的评估指标。越接近1，说明两个重复样品相关性越强。|
|Benjamini-Hochberg|Benjamini-Hochberg矫正方法||1995年Benjamini和Hochberg提出了FDR的概念,并给出了在多重检验中对它的控制方法(简称BH方法)，FDR(false discovery rate)，是统计学中常见的一个名词，翻译为伪发现率，其意义为是 错误拒绝（拒绝真的（原）假设）的个数占所有被拒绝的原假设个数的比例的期望值。|
|Biological Process|生物学过程||生物学过程系指由一个或多个分子功能有序组合而产生的系列事件。|
|Molecular Function|分子功能||可以描述为分子水平的活性（activity），如催化（catalytic）或结合（binding）活性。|
|Cellular Component|细胞组分||细胞的每个部分和细胞外环境。|
|Transcripts Per Million|TPM算法||Transcripts Per Million，公式为：单一miRNA reads数*10^6/总reads数。在做miRNA的差异表达分析时，用来校准miRNA的表达量。|
|Enrichment Factor|富集因子|Enrichment Factor is used to describe bodies of mineral ore. It is defined as the minimum factor by which the weight percent of mineral in an orebody is greater than the average occurrence of that mineral in the Earth's crust. It can be used to compare the necessary enrichment of different types of minerals for their recovery to be economically viable.||
|Fisher Test|Fisher精确检验||Fisher's exact test，用来判断两个变量之间是否存在非随机相关性的一种统计学检验方法。|
|STRING|||蛋白质间预测的功能相关性的一个数据库, 蛋白质间的功能链接通常能够从编码它们的基因间的基因组相关性中推断：相同功能所需要的一群基因趋向于显示相似的物种覆盖，通常定位在基因组(在原核生物中)上非常邻近的位置，并且趋向于参与基因融合事件。STRING数据库是用来浏览和分析这些相关性的一个预计算的全局资源。|
|Cytoscape|||Cytoscape是一款图形化显示网络并进行分析和编辑的软件，它支持多种网络描述格式，也可以用以Tab制表符分隔的文本文档或Microsoft Excel文件作为输入，或者利用软件本身的编辑器模块直接构建网络。|
|DEU|||exon水平的差异分析。|
|UTR|||非翻译区域，是信使 RNA（mRNA）分子两端的非编码片段。5'-UTR从mRNA起点的甲基化鸟嘌呤核苷酸帽延伸至 AUG 起始密码子，3'-UTR从编码区末端的终止密码子延伸至多聚 A 尾巴（Poly-A）的前端。|
|ORF|||开放阅读框或开放读码框。是结构基因的正常核苷酸序列，从起始密码子到终止密码子的阅读框可编码完整的多肽链，其间不存在使翻译中断的终止密码子。|
|Unigene|||Unigene Gene的英文缩写，意为广泛通用的基因数据库，通过电脑对相同基因座（Locus）的收集整理集合形成一个非冗余的基因数据库。|
|Trinity|||Trinity是一款专门为高通量转录组测序设计的组装软件。Trinity软件首先将测序reads打断为较短的片段K-mer，然后将这些小片段延伸成较长的片段Contig，并利用这些片段之间的重叠，得到片段集合Component，最后利用De Bruijin图的方法和测序reads信息，在各个片段集合中分别识别转录本序列。|
|K-mer|||长度为k的核苷酸序列。|
|De Bruijn图|||在 De Bruijn 图中,每一个 read 被切分成长度为 k 的小片段,称为 k-mer.每个 k-mer 为一个顶点.如果存在 read,使得两个 k-mers 相邻且重叠 k−1 个字符,那么它们之间存在一条有向边.这样,每个 read 被映射成图中的一条路径.这样序列组装问题变成了在 De Bruijn 图中寻找一条包含所有 read 的路径.|
|SSR|||即简单重复序列，又叫微卫星序列，指的是基因组中由1-6个核苷酸组成的基本单位重复多次构成的一段DNA，广泛分布于基因组的不同位置，长度一般在200bp以下。|
|BSR(Bulked Segregant RNA sequencing)|||将转录组测序与集群分离分析相结合，在转录组范围内开发SNPs，筛选与性状紧密连锁的SNPs，进行功能基因的定位，同时进行基因差异表达分析等转录组常规分析的技术。|
|Nanodrop|||分光光度计，应用液体的表面张力特性，样品体积只需要0.5~2ul，在检测台上，经上下臂的接触拉出固定的光径达到快速、微量、高浓度、兔石英管、兔毛细管等耗材检测吸收值的优点。|
|Qubit|||新一代核酸和蛋白定量仪，实验台上对DNA和RNA进行精准定量。|
|Agilent 2100 bioanalyzer|||Agilent 2100生物分析仪是最成功 的基于微流控技术的DNA、RNA、蛋白质和细胞分析检测平台，可用于从疾病探索、药物研发到生物药剂的质量保证和质量控制(QA/QC)的整个工作流程中的多种用途。|
|miRDeep2|||miRDeep2软件是一款已知miRNA鉴定和新miRNA预测的综合软件包，通过将reads比对到基因上得到可能的前体序列，基于reads在前体序列上的分布信息(基于miRNA产生特点，mature,star,loop)及前体结构能量信息(RNAfold randfold)采用贝叶斯模型经打分最终实现miRNA的鉴定。|
|isomiRID||Standardizes and automatizes the search for miRNAs isoforms in high-throughput small RNA sequencing libraries. isomiRID provides a tool to automate, standardize and simplify the searches for isomiRs and non-templated nucleotides in 3’and 5’miRNA ends, using as input single or multiple sequencing data files in a comparative way. The output files produced from this workflow are understandable tab delimited.txt files, which can be easily imported for spreadsheet or statistical suits, as R package. Also, the aligned output provides a broad view of particular miRNAs and the abundance of their isomiRs sequences in different sequencing datasets.||
|Q-PCR|||指在PCR反应体系中加入荧光基团，利用荧光信号累积实时监测整个PCR进程，最后通过标准曲线对未知模板进行定量分析的方法。利用荧光信号的变化实时检测PCR扩增反应中每一个循环扩增产物量的变化，通过Ct值和标准曲线的分析对起始模板进行定量分析。|
|SpliceGrapher||SpliceGrapher is a Python package for creating splice graphs from RNA-Seq data, guided by gene models and EST data (when available). Starting with version 0.2.2 we introduced SpliceGrapherXT that can convert splice graph predictions into transcript predictions.||
|CPC|||CPC (Coding Potential Calculator)分析是一种基于序列比对的蛋白质编码潜能计算工具。通过转录本与已知蛋白数据库比对，根据转录本各个编码框的生物学序列特征评估其编码潜能。|
|CNCI|||CNCI(Coding-Non-Coding Index)分析是一种通过相邻核苷酸三联体特征区分编码-非编码转录本的方法。|
|DESeq|||DESeq是一个基于reads count来进行差异分析的R包。|
|EBSeq|||一个进行RNA-Seq实验推断的经验贝叶斯层次模型。|
|Fold Change|||差异表达倍数。|
|FDR|||错误发现率，定义为在多重假设检验过程中，错误拒绝(拒绝真的原(零)假设)的个数占所有被拒绝的原假设个数的比例的期望值，通过控制FDR来决定P值的阈值。|
|Cufflinks|||cufflinks利用tophat比对的结果来组装转录本，估计这些转录本的丰度，并且检测样本间的差异表达及可变剪接。这个软件其实是个套餐，包括四个部分分别命名为：cufflinks, cuffcompare, cuffmerge及cuffdiff。|
|Asprofile|||Asprofile由多个程序组成，可用于提取，定量和比较由RNA-seq数据组装得到的转录本的可变剪切事件。|
|NR|||NR是NCBI官方的蛋白序列数据库，它包括了 GenBank基因的蛋白编码序列，PDB(Protein Data Bank)蛋白数据库、SwissProt蛋白序列及来自PIR（Protein Information Resource）和PRF（Protein Research Foundation）等数据库的蛋白序列。根据 nr注释信息我们能得到 GO 功能注释。|
|Swiss-Prot|||搜集、整理、分析、注释、发布，力图提供高质量的蛋白质序列和注释信息。SwissProt数据库的每个条目都有详细的注释，包括结构域、功能位点、跨膜区域、二硫键位置、翻译后修饰、突变体等。该数据库中还包括了与核酸序列数据库EMBL/GenBank/DDBJ、蛋白质结构数据库PDB以及Prosite、PRINTTS等十多个二次数据库的交叉引用代码。|
|GO|||基因本体联合会（Gene Ontology Consortium）所建立的数据库，旨在建立一个适用于各种物种的，堆积因何蛋白质功能进行限定和描述的，并能随着研究不断深入而更新的语言词汇标准。GO 是多种生物本体语言中的一种，提供了三层结构（分子功能、生物学途径、细胞组件）的系统定义方式，用于描述基因产物的功能。|
|COG, KOG|||COG是Clusters of Orthologous Groups of proteins的简称，KOG 为euKaryotic Ortholog Groups。这两个注释系统都是NCBI中基于基因直系同源关系的数据库，其中COG针对原核生物，KOG针对真核生物。COG/KOG结合进化关系将来自不同物种的同源基因分为不同的 Ortholog簇，目前COG有4873个分类，KOG有4852个分类。来自同一 ortholog 的基因具有相同的功能，这样就可以将功能注释直接继承给同一 COG/KOG 簇的其他成员。详见http://www.ncbi.nlm.nih.gov/COG/。|
|Pfam|||pfam数据库是一个蛋白质家族数据库，依赖于多序列比对和隐马尔科夫模型。|
|KEGG|||是系统分析基因产物和化合物在细胞中的代谢途径以及这些基因产物的功能的数据库。它整合了基因组、化学分子和生化系统等方面的数据,包括代谢通路（KEGG PATHWAY）、药物（KEGG DRUG）、疾病（KEGG DISEASE）、功能模型（KEGG MODULE）、基因序列（KEGG GENES）及基因组（KEGG GENOME）等等。KO（KEGG ORTHOLOG）系统将各个KEGG注释系统联系在一起，KEGG已建立了一套完整KO注释的系统，可完成新测序物种的基因组或转录组的功能注释。详见http://www.genome.jp/kegg/。|
|KOBAS|||一个提供注释和识别富集通路和疾病的网站。|
|KEGG Orthology|||KEGG建立了KEGG直系同源系统(theKEGG Orthology (KO)system)，这个系统通过把分子网络的相关信息连接到基因组中，从而发展和促进了跨物种注释流程。|
|HMMER|||一款比对软件，可以类似于blast等，但是它提供的比对结果要精确于blast，相应的速度也要慢。|
|GATK|||全称是The Genome Analysis Toolkit, 是Broad Institute开发的用于二代重测序数据分析的一款软件，里面包含了很多有用的工具，主要注重于变异的查找，基因分型且对于数据质量保证高度重视。|
|SnpEff|||一款用于注释变异（SNP、InDel）和预测变异影响的软件。根据变异位点在参考基因组上的位置以及参考基因组上的基因位置信息，可以得到变异位点在基因组发生的区域（基因间区、基因区或CDS区等），以及变异产生的影响（同义非同义突变等）。|
|topGO|||基因本体得分构架，是一款基于分析基因表达数据来计算生物学意义的软件包。它实现了从微矩阵来确定基因本体组的相关性的各种标准和先进的新算法。|
|PDB|||蛋白质数据库，主要由X-射线晶体衍射和核磁共振（NMR）测得的生物大分子三维结构组成，用户可直接查询，调用和观察库中所收录的任何大分子三维结构。|
|small RNA, sRNA|||对长度在18-40bp的短 RNA 进行序列、结构、表达、功能上的分析，主要进行miRNA，siRNA，piRNA 几种类型 sRNA 的分析，可与 mRNA 关联分析。|
|ncRNA, non coding RNA|||非编码RNA，指不编码蛋白质的RNA。其中包括 rRNA，tRNA，snRNA，snoRNA和microRNA 等多种已知功能的 RNA，及未知功能的 RNA。其共同特点是都能从基因组上转录而来，不需要翻译成蛋白即可在 RNA 水平上行使各自的生物学功能。|
|lncRNA, long  non coding RNA|||长链非编码RNA，在长度200-100000nt之间，不具有编码蛋白功能的转录本。|
||PCR 产物测序||针对 DNA PCR 扩增产物进行序列检测或拼接，提供序列信息及相应分子标记结果，有助于多样性分类或其他 DNA 片段研究。|
||光学图谱||来源于单个DNA分子有序的全基因组限制性内切酶酶切位点图谱|
||单碱基的错误率||组装错误的碱基占基因组全长的比例。|
||基因区覆盖度||基因区组装的完整度评估指标。|
||基因融合||指将两个或多个基因的编码区首尾相连,置于同一套调控序列(包括启动子、增强子、核糖体结合序列、终止子等)控制之下,构成的嵌合基因.融合基因的表达产物为融合蛋白|
|Molecular marker|分子标记||是以个体间遗传物质内核苷酸序列变异为基础的遗传标记，是DNA水平遗传多态性的直接反映。|
||全基因组个体重测序||基于全基因组重测序的变异图谱通过测序手段结合生物信息分析研究同一物种不同个体之间的变异情况，获得大量的变异信息，如 SNP、 Indel、 SV 等。主要可以快速地获得大量的分子标记以及不同个体在基因组水平上的差异。|
||亚种||是某种生物分布在不同地区的种群，由于受所在地区生活环境的影响，他们在形态构造或生理机能上发生某些变化，这个种群就称为某种生物的一个亚种。|
||BAM格式||BAM是SAM的二进制文件。|
|IGV|基因组浏览器||是一种高性能的可视化工具，用来交互式地探索大型综合基因组数据。它支持各种数据类型，包含array-base的和下一代测序的数据和基因注释。|
||SNP位点密度||将每个基因的SNP位点数目除以基因的长度，得到每个基因的SNP位点密度值。|
||可变剪切||有些基因的一个mRNA前体通过不同的剪接方式（选择不同的剪接位点）产生不同的mRNA剪接异构体，这一过程称为可变剪接(或选择性剪接，alternative splicing)。可变剪接是调节基因表达和产生蛋白质组多样性的重要机制，是导致真核生物基因和蛋白质数量较大差异的重要原因。在生物体内，主要存在7种可变剪接类型：A）Exon skipping；B）Intron retention；C) Alternative 5' splice site；D) Alternative 3' splice site；E) Alternative first exon；F) Alternativelast exon；G) Mutually exclusive exon|
||负二项分布||负二项分布是统计学上一种离散概率分布。满足以下条件的称为负二项分布：实验包含一系列独立的实验，每个实验都有成功，失败两种结果，成功的概率是恒定的，实验持续到r次成功，r为正整数。|
||生物学重复||指的是经过相同方式处理的相同样品。|
||差异显著性p值||统计学根据显著性检验方法所得到的P 值，一般以P&lt;0.05为显著，P&lt;0.01为非常显著，其含义是样本间的差异由抽样误差所致的概率小于0.05或0.01。|
||超几何检验||基于超几何分布的不放回抽检方式，它描述了由有限个物件中抽取n个物件，成功抽取出指定种类的物件的次数。|
|Microbial diversity|微生物多样性||指环境中微生物物种的多样性，微生物多样性的研究方法有很多，主要分为两大类：传统分离纯培养法及现代分子生物学法。目前常使用的现代分子生物学法是基于高通量测序平台，对核糖体RNA高变区域，比如16S rDNA/18S rDNA/ITS等基因序列进行扩增测序，揭示环境样品中微生物的物种种类、种类间的相对丰度以及进化关系。|
||16S rDNA||指编码原核生物核糖体小亚基rRNA（16S rRNA）的DNA序列,具有良好的进化保守性,适宜的分析长度（约1.5kb）:包括9个可变区、10个保守区。保守区在近缘物种间序列相似，进化速率慢，该区域适合分析亲缘关系较远的物种的进化关系；可变区在亲缘关系较近的物种间也有较大差异，适合分析亲缘关系较近的物种间的进化关系。|
||18S rDNA||指编码真核生物核糖体小亚基rRNA（18SrRNA）的DNA序列。其在物种间比较保守，进化速率较慢，适合在较高的物种分类水平上确定样品的物种分类，但是不适合于区分种或亚种。|
|Internal transcribed spacer|ITS||指真核生物核糖体RNA对应的编码DNA区域的转录间隔区序列，常用作微生物分类研究。常用的ITS为ITS1和ITS2。由于ITS区在核糖体RNA加工过程中被剪切掉，不发挥功能，在进化过程中选择压力较小，进化速率约为18S rDNA的10倍，属于中度保守的区域，利用它可研究种及种以下的分类阶元。|
|Internal transcribed spacer 1|ITS1||指真核生物核糖体RNA对应的编码DNA区域的转录间隔区序列，位于真核生物核糖体rDNA序列的18S和5.8S之间。由于ITS1区在核糖体RNA加工过程中被剪切掉，不发挥功能，在进化过程中选择压力较小，进化速率约为18S rDNA的10倍，属于中度保守的区域，利用它可研究种及种以下的分类阶元。|
|Internal transcribed spacer 2|ITS2||指真核生物核糖体RNA对应的编码DNA区域的转录间隔区序列，位于真核生物核糖体rDNA序列5.8S和28S之间。由于ITS2区在核糖体RNA加工过程中被剪切掉，不发挥功能，在进化过程中选择压力较小，进化速率约为18S rDNA的10倍，属于中度保守的区域，利用它可研究种及种以下的分类阶元。|
|Chimeric DNA sequences|嵌合体||指微生物多样性的样品在进行PCR时，多数序列都是由单条序列进行扩增的，如Read1扩增产生新的Read1，Read2扩增产生新的Read2。但有时两条序列也可能缠在一起，扩增时产生的新序列前半段可能属于Read1，后半段属于Read2，形成了拥有两条序列信息的嵌合体序列。这样的嵌合体序列在后续分析中会被错误地认为是新的物种，从而导致样品的物种多样性被高估，并影响样品间多样性的比较，必须在分析之前去除嵌合体。|
|Operational taxonomic unit|OTU||即操作分类单元，是在系统发生学研究或群体遗传学研究中，为了便于进行分析，人为给某一个分类单元（品系，种，属，分组等）设置的同一标志。一般情况下，如果序列之间，相似性高于97% 就可以把它定义为一个OTU，每个OTU对应一种代表性的序列。|
|alpha diversity, α-diversity|Alpha多样性||指某个取样环境中的物种的多样性，通过一些根据样品中物种的种类及丰度计算出的指数来反映，指数的大小反映单个样品中物种的多样性。|
|rarefaction curve|稀释性曲线||指从样本中随机抽取一定数量的序列，统计这些序列所代表的物种数目，并以序列数与物种数来构建的曲线，用于验证测序数据量是否足以反映样品中的物种的多样性，并间接反映样品中物种的丰富程度。稀释性曲线可以判断各样本测序量是否充分,曲线一直急剧上升表明测序量不足，需要增加序列条数；如果曲线最终趋于平坦，则表明样品序列充分，可以进行数据分析。|
|rank abundance curve|等级丰度曲线||指将各样品的OTU丰度按大小排序并基于其相对丰度绘制的曲线图，主要用于同时解释样品所含物种的丰富度和均匀度，物种的丰富度由曲线在横轴上的长度来反映，曲线越宽，表示物种的组成越丰富；物种组成的均匀度由曲线的形状来反映，曲线越平坦，表示物种组成的均匀程度越高。|
|shannon index curve|香农指数曲线||指由各在不同测序深度时各样品的Shannon指数（反映样品中微生物多样性的指数）绘制的Shannon多样性指数稀释曲线，以此反映各样本在不同测序数量时的微生物多样性。当曲线趋向平坦时，说明测序数据量足够大，OTU种类不会再随测序量增加而增长；如果曲线没有趋于平坦，则表明不饱和，增加数据量可以发现更多OTU。|
|beta diversity, β-diversity|Beta多样性||比较不同样品之间在物种多样性方面（群落组成及结构）存在的差异大小。|
|principal component analysis|PCA||即主成分分析，是一种应用方差分解，对多维数据进行降维，从而提取出数据中最主要的元素和结构的方法。样品间距离越近，表示这两个样品的组成越相似。|
|principal coordinates analysis|PCoA||一种与PCA类似的降维排序方法，原理是假设对N个样品有衡量它们之间差异或距离的数据，就可以用此方法找出一个直角坐标系，将N个样品表示成N个点，而使点间的欧式距离的平方正好等于原来的差异数据，实现定性数据的定量转换，从多维数据中提取出最主要的元素和结构。样品间距离越近，表示这两个样品的组成越相似。|
|Non-MetricMulti-Dimensional Scaling|NMDS||一种适用于生态学研究的排序方法，主要是将多维空间的研究对象（样本或变量）简化到低维空间进行定位、分析和归类，同时又保留对象间原始关系的数据分析方法。样品间距离越近，表示这两个样品的组成越相似。NMDS设计的目的是为了克服以前排序方法（包括PCA、PCoA在内）使用线性模型的缺点。NMDS的模型是非线性的，能更好地反映生态学数据的非线性结构。|
|unweighted pair-group method with arithmetic mean|UPGMA||即非加权组平均法，也可理解为样品层次聚类，是一种常用的聚类分析方法。其假定的前提条件是在进化过程中，每一世系发生趋异的次数相同，即核苷酸或氨基酸的替换速率是均等且恒定的。通过UPGMA法所产生的系统发生树可以说是物种树的简单体现，在每一次趋异发生后，从共同祖先节点到2个分支的长度一样。|
|Line Discriminant Analysis Effect Size|LEfSe||即使用软件LEfSe进行多个分组之间的比较分析。其原理是：首先在多组样本中采用的非参数因子Kruskal-Wallis秩和检验检测不同分组间丰度差异显著的物种，然后基于上一步中获得的显著差异物种，用成组的Wilcoxon秩和检验来进行组间差异分析，最后用线性判别分析（LDA）对数据进行降维和评估差异显著的物种的影响力（即LDA score），一般将LDA Score大于设定阈值的物种确定为biomarker。|
|analysis of variance|ANOVA||方差分析,又称“变异数分析”或“F检验”，是R.A.Fisher发明的，用于两个及两个以上样本均数差异的显著性检验。|
|Wilcoxon rank sum test|Wilcoxon秩和检验||两组独立样本非参数检验的一种方法。其原理是假设两组独立样本的总体分布无显著差异，通过对两组样本平均秩的比较达到判断两总体的分布是否存在差异的目的，该分析可以对两组样品的物种进行显著性差异分析，并计算其p值。|
|ternary　phase　diagram|三元相图||用一个等边三角形描述三个变量的不同属性的比率关系，在分析中可以根据物种分类信息对三个或三组样品的物种组成进行比较分析，通过三角图可以直观的显示出不同物种在样品中的比重和关系。|
|Genetic Map|遗传连锁图谱||分子标记在染色体上的相对位置与遗传距离|
|Bin map|||某个样本中出现分型转变认为出现了重组断点，然后根据重组断点间的标记进行划分Bin|
|linkage group|连锁群||一对或一条染色体上的所有基因总是联系在一起而遗传，这些基因统称为一个连锁群|
||表型值||在数量遗传学中,一个数量的表型值就是在实践中所度量或观察到的值|
|Chi-square test|卡方检验||它属于非参数假设检验，主要是比较两个及两个以上样本率( 构成比）以及两个分类变量的关联性分析|
||偏分离||观察到的基因型比例偏离预期的孟德尔频率的分离方式|
||遗传距离||两个基因在同一染色体上的相对距离,通常用重组率表示|
|R/qtl|||R/qtl是在遗传群体中定位数量性状位点的一个可扩展的交互环境|
|Permutation Test|PT检验||PT检验是Fisher于20世纪30年代提出的一种基于大量计算（computationally intensive），利用样本数据的全（或随机）排列，进行统计推断的方法|
||PCR引物设计||一小段单链DNA或RNA，在核酸合成反应时，作为每个多核苷酸链进行延伸的出发点而起作用的多核苷酸链|
|Log of the likelihood ratio|LOD值||估计值在观察结果中出现这种概率的可能性，用来反映重组率估计值的可靠性程度或作为连锁是否真实存在的一种判断尺度|
|Recombinant Inbred Lines|RIL群体||RIL（Recombinant Inbred Lines） 重组自交系 ，将F2个体连续自交或同胞交配，或群体内随机交配，使得杂种的基因得以分离并进行重组，直至家系内个体基因型纯合稳定，家系间基因型各异，这些家系就构成了重组自交系群体|
|F2|||由两个不同基因型的纯合双亲杂交产生F1代，又自交而形成F2代所构成的群体|
|DH|||通过F1诱导单倍体并加倍形成的群体|
|DISTANCE|||在窗口内按照步长的大小滑动窗口|
|SNPNUM|||对每一个SNP，拟合后的关联值=前后各n个SNP的关联值的中值，即窗口大小为2n|
|LOESS|||取预测变量附近一个数据子集，对其进行回归分析估计，越靠近估计点的值，权重越大|
|FRAME SHIFT|移码突变||DNA分子中每一个碱基都是三联密码子中的一个成员，而且遗传信息为DNA链上排列成特定序列的密码子所控制，在这种碱基序列中有一个或几个碱基增加或减少而产生的变异|
|Silva|||一个rRNA数据库|
|GtRNAdb|||一个tRNA数据库|
|Rfam|||非编码RNA数据库|
|Repbase|||重复序列数据库|
|miRbase|||已知miRNA数据库|
|HMDD, Human microRNA Disease Database|||人类miRNA疾病数据库|
|WGCNA, Weighted Correlation Network analysis|||是一个基于基因表达网络权重构建，描述基因表达的关联模式的R包。|
