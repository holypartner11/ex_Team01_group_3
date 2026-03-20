# 当当网Python类图书销售分析

本项目基于当当网官网数据，对Python类图书销售情况进行系统性分析，包括销售趋势、热门图书、价格分析等维度。项目旨在帮助教师了解Python相关书籍的市场情况，为编写Python书籍提供参考。

本项目的github地址为（https://github.com/holypartner11/ex_Team01_group_3）

## 数据集

项目使用的数据集来源于当当网官网（[https://search.dangdang.com/](https://search.dangdang.com/)），通过关键词'python'搜索，销量从高到低排序，收集前50条记录。

数据存储在以下文件夹中：
- `data_raw/`：原始数据文件 `dangdang_python_books_raw.csv`
- `data_clean/`：清洗后数据文件 `dangdang_python_books_clean.csv`

数据集包含以下主要字段：
- 书名、作者、年份、出版社、评论数
- 原价、折后价
- 其他相关销售信息

## 分析内容

项目通过数据分析回答以下问题：

1. **销量排名前10的Python类图书清单**
2. **销量前50的Python类图书主要涵盖的领域**（如编程技巧、数据分析、机器学习、深度学习、青少年编程等）
3. **销量前50的Python类图书中，哪些出版社的书籍比较多**
4. **销量前50的Python类图书中，原价和折后价的分布，折扣率的分布特征**
5. **词频分析**：去除无用词汇后，分析销量前50的Python类图书的书名中，哪些词汇出现频率较高
6. **不同类型的Python书籍的售价情况**
7. **书名中的关键词与售价和销量之间是否存在关联**

## 项目结构

- `T1-当当网Python类图书销售分析.md`：项目任务描述和分析目标
- `02_EDA_analysis.ipynb`：探索性数据分析主文件
- `code/`：小组成员的分析代码文件
  - `01_analysis.ipynb`：总体分析
  - `问题3-刘嘉亮.ipynb`：出版社分析
  - `问题5_词频分析.ipynb`：词频分析
  - `问题7-刘桃蹊.ipynb`：其他分析
  - `python_books_classify.ipynb`：书籍分类
- `data_raw/`：原始数据
- `data_clean/`：清洗后数据
- `output/`：分析结果输出文件
  - `01_销量前十书籍分析.md`
  - `分析结论与写书建议.txt`
  - `关键词-售价-销量综合分析表.csv`
  - `问题3.Python书籍出版社分析结果.csv`
  - `python_books_classified.csv`
  - `python_books_classify_summary.csv`
- `intergrated_homework/`：集成作业相关文件

## 代码运行方式

### 运行环境要求

- Python 3.x
- Jupyter Notebook
- 必要的Python包：pandas, numpy, matplotlib, jieba（用于中文分词）等

### 运行步骤

1. 确保安装了Python和相关包
2. 打开终端，导航到项目目录：
   ```
   cd （文件根目录）/ex_Team01_group_3
   ```
3. 启动Jupyter Notebook：
   ```
   jupyter notebook
   ```
4. 打开相应的.ipynb文件运行分析

### 注意事项

- 数据文件较大，请确保有足够的存储空间
- 运行前请检查数据路径是否正确
- 部分分析可能需要较长时间，请耐心等待
- 中文分词分析需要jieba库

## 作者信息

- **组号**：3组
- **组员**：刘桃蹊（组长）、刘嘉亮、冯一帆、张橦菲、杨金梅、马琳琳、蔡柏林、胡雁雄
- **班级**：25MDE-PC