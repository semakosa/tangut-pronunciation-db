[![License: Limited Public Use](https://img.shields.io/badge/License-Limited%20Public%20Use-blue.svg)](https://github.com/semakosa/tangut-tools/blob/main/LICENSE-DATA.md)
[![DOI](https://img.shields.io/badge/DOI-10.25365%2Fphaidra.654-orange.svg)](https://doi.org/10.25365/phaidra.654)

[English](#english) [简体中文](#chinese)

# <a name="english"></a> Tangut Pronunciation Database

## Overview

This repository hosts the Tangut Pronunciation Database, a collection of TSV files providing pronunciation data for Tangut characters. Each file represents a version of the database, identified by its date, and includes multiple transcription systems with evolving accuracy.

In addition to GitHub, this database is permanently archived at [PHAIDRA](https://phaidra.univie.ac.at/detail/o:2122259), the University of Vienna's digital repository, in accordance with the FAIR principles, ensuring its long-term preservation and accessibility, with a DOI ([10.25365/phaidra.654](https://doi.org/10.25365/phaidra.654)) for persistent identification.

## Versioning

Files follow a date-based versioning scheme in the format `YYYYMMDD.tsv`, for example:
- `20250321.tsv` - March 21, 2025 version

The files currently available belong to the **preliminary series** of the database, which still relies on manual corrections and updates. As of early 2025, the data offers better consistency than mainstream dictionaries, but with more limited character coverage. A new **validated series** is currently under development, with pronunciation data mechanically verified from a comprehensive range of sources, ensuring far better character coverage and consistency.

## Data Structure

Each TSV file contains the following fields:

| Field | Description |
|-------|-------------|
| `li` | Number of the character in Li Fanwen's dictionary |
| `unicode` | The Tangut character itself in Unicode encoding |
| `GHC` | Gong Hwang-cherng's phonological reconstruction |
| `homophones` | Initial class number (1-9) as reflected in the chapter number in the native Tangut dictionary _Homophones_ |
| `sea` | Rhyme classification as reflected in the chapter number in the native Tangut dictionary _Sea of Characters_ |
| `GX2021` | GHC system with Xun Gong's 2021 modifications |
| `GX202404` | Xun Gong's transcription system as of April 2024 |
| `GX202411` | Xun Gong's transcription system as of November 2024 |

Further transcription systems may be added in future versions. All pronunciations given in a row correspond to one another, insofar as the systems are commensurable.

* **GHC**: The pronunciations assigned to characters in the widespread GHC system reflect the author's personal judgment. They do not necessarily coincide with the pronunciations given in other dictionaries using the GHC system, just as the dictionaries themselves often differ.
* **homophones**, **sea**: The indices are strictly bibliographic. Thus, if a character actually belongs to a group equivalent to some bibliographic group but is not actually attested in the source, no index is given.

## License

This database, which currently contains only the **preliminary series**, is provided under a **Limited Public Use** license:
- **Free for Research, Teaching, Publication, and Commercial Use** – You may use and cite individual data points in academic research, teaching, publications, and commercial applications. Internal bulk processing is permitted as long as the processed results are not publicly distributed at scale. The license is available at [LICENSE-DATA.md](LICENSE-DATA.md).
- For permissions beyond these terms, please contact the author.

The **validated series**, once completed, will be provided under a more permissive license.

## Citation

When using this database in academic work, you can cite it as follows:

> Gong, Xun (YEAR). Tangut pronunciation database, version [DATE]. University of Vienna. DOI: 10.25365/phaidra.654

For specific reconstruction schemes:

- **GX2021**: Gong, Xun (2021). "Nasal preinitials in Tangut phonology." *Archiv orientální* 89.3: 443-482.
- **GX202411**: Gong, Xun (2025). "Tone values of Tangut." *Bulletin of Chinese Linguistics* 18.1.

## Contributing

Contributions and feedback are welcome from the research community:

- **Data Corrections:** If you find errors or inconsistencies in the data, please open an issue or submit a pull request with corrections.
- **Feature Requests:** Suggestions for new functionality can be submitted as issues.

## Contact

For questions, permission requests, or collaboration opportunities, please contact:

- **Xun Gong**
- **University of Vienna**
- **Email:** xun.gong@univie.ac.at

# <a name="chinese"></a> 西夏文拟音数据库

## 概述

本GitHub仓库（[西夏文拟音数据库](https://github.com/semakosa/tangut-tools)）收录西夏文单字的拟音数据，以一系列TSV文件的形式提供。每个文件代表数据库的一个版本，以日期命名，并包含多个不断完善的转写方案。

本数据库在GitHub之外，同时永久存档于维也纳大学的PHAIDRA系统，确保其长期保存和可访问性，并提供永久标识（DOI: [10.25365/phaidra.654](https://doi.org/10.25365/phaidra.654)）。您可以通过[此链接](https://phaidra.univie.ac.at/detail/o:2122259)访问存档版本。

## 版本管理

文件采用基于日期的版本格式：`YYYYMMDD.tsv`，例如：
- `20241129.tsv` - 2024年11月29日版本

现阶段提供的文件属于数据库的**预发布系列**（preliminary series），其中校订与调整仍依赖手动完成。以2025年初的情况而言，本数据库在数据一致性方面优于主流词典，但缺字较多。另一套**验证稳定系列**（validated series）正在开发中，将基于更全面的来源进行机械校验，以确保字符覆盖率和数据一致性。

## 数据结构

每个TSV文件包含以下字段：

| 字段       | 描述                                                                 |
|------------|----------------------------------------------------------------------|
| `li`       | 李范文《夏汉字典》编号                                               |
| `unicode`  | 字符本身，以Unicode码表示                            |
| `GHC`      | 龚煌城拟音                                                   |
| `homophones` | 声母类别，即《同音》章节号（1-9类）                                      |
| `sea`      | 韵类，即《文海》章节号                                                 |
| `GX2021`   | 龚煌城拟音，龚勋2021年修订版                                              |
| `GX202404` | 龚勋拟音，2024年4月版本                                          |
| `GX202411` | 龚勋拟音，2024年11月版本                                         |

未来版本可能会引入更多的拟音系统。在各系统之间具有可比性的范围内，同一行中的不同拟音相互对应。

* **GHC**: 本数据库中的龚煌城系统拟音反映了作者的个人判断，可能与其他使用龚煌城系统的字典中的拟音不同，正如这些字典之间也常有差异。
* **homophones**, **sea**: 声母类别和韵类严格按照原书。如果某个字实际上属于某个声韵类别，但原书中没有提及，则不予列出。

## 使用授权

本数据库目前仅包含**预发布系列**的内容，按照**有限公共使用许可**提供：**研究、教学、出版及商业应用均可免费使用** - 您可以在学术研究、教学、出版物和商业应用中使用和引用个别数据点。允许内部批量处理，但前提是不在大规模公开分发处理后的结果。许可协议全文见 [LICENSE-DATA.md](LICENSE-DATA.md)。
- 如需超出这些条款的许可，请联系作者。

**验证稳定系列**一旦完成，将以更宽松的许可提供。

## 文献引用

在学术工作中使用本数据库时，可按以下格式引用：

> Gong, Xun (年份). Tangut pronunciation database, version [年月日]. University of Vienna. DOI: 10.25365/phaidra.654

拟音系统的参考文献：
- **GX2021**: Gong, Xun (2021). "Nasal preinitials in Tangut phonology." *Archiv orientální* 89.3: 443-482.
- **GX202411**: Gong, Xun (2025). "Tone values of Tangut." *Bulletin of Chinese Linguistics* 18.1.

## 协作机制

欢迎爱好者朋友和学界同仁参与完善：
- **数据纠错：** 如发现数据错误或不一致，请开启一个问题（issue）或提交带有更正的pull request。
- **功能需求：** 新功能的建议可以作为问题（issue）提交。

## 联系方式

- **龚勋**
- **维也纳大学**
- **邮箱：** xun.gong@univie.ac.at