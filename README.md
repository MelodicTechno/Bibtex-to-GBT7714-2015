<!-- Improved compatibility of back to top link: See: https://github.com/54dbd/Bibtex-to-gbt7714/pull/73 -->
<a name="readme-top"></a>
<!--
*** Thanks for checking out the Best-README-Template. If you have a suggestion
*** that would make this better, please fork the repo and create a pull request
*** or simply open an issue with the tag "enhancement".
*** Don't forget to give the project a star!
*** Thanks again! Now go create something AMAZING! :D
-->



<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
[![Patreon][patreon-shield]][patreon-url]

<!-- 项目LOGO -->
<br />
<div align="center">
  <img src="https://i.ibb.co/zQvJf2L/Vector.png" alt="Vector" height="200"/>
  <h3 align="center">Bibtex 转 GB/T 7714-2015 转换器</h3>

  <p align="center">
    本项目用于将 bibtex 文件转换为 GB/T 7714 格式
    <br />
    <a href="https://openstd.samr.gov.cn/bzgk/gb/newGbInfo?hcno=7FA63E9BBA56E60471AEDAEBDE44B14C"><strong>了解 GB/T 7714-2015 »</strong></a>
    <br />
    <a href="https://github.com/54dbd/Bibtex-to-gbt7714/issues">报告错误</a>
  </p>
</div>




<!-- 关于本项目 -->

## 关于本项目

本项目旨在将 bibtex 文件转换为 GB/T 7714 格式，该格式是中国学术出版物常用的标准引用格式。  
通过将 bibtex 文件转换为 GB/T 7714 格式，可以更方便地将参考文献集成到中文学术论文中。




<!-- 快速开始 -->

## 快速开始

本项目运行于 Python 3.9+，较低版本未经过测试。

### 环境

* Python 3.9+
* poetry

### 安装步骤

1. 克隆仓库

  ```sh
    git clone https://github.com/54dbd/Bibtex-to-gbt7714-converter.git
```

2. 安装 poetry 依赖

```
 poetry install
 ```

或者使用 pip：

```
 pip install -r requirements.txt
```

3. 运行转换脚本，并以 bibtex 文件作为输入：

```
  poetry run python main.py data/ref.bib
```

或者

```
  python main.py data/ref.bib
```

将 ref.bib 替换为你的 bibtex 文件名。

<!-- 使用示例 -->

## 使用方法

例如，如果你有一个 bibtex 文件 ref.bib，可以运行以下命令将其转换为 GB/T 7714 格式：

```
python main.py data/ref.bib
```

如果你需要添加默认列表中没有的中文姓氏，可以使用以下代码将它们添加到 data/Chinese_surname.csv 文件中：

```
python utility/chineseSurnameCombination.py <name1> <name2> <name3> ...
```

<!-- 开发规划 -->

## 开发规划

- [x] 支持 arXiv 格式输入
- [x] 支持常见格式输入
- [ ] 支持所有现有格式
- [ ] 针对不同类型的媒体进行专门处理
- [ ] 支持多语言输入
  - [x] 英文
  - [x] 中文（未测试，考虑到本项目主要用于将国际参考文献转换为中文学术引用格式）

查看 [open issues](https://github.com/54dbd/Bibtex-to-gbt7714/issues) 了解完整的待实现功能及已知问题。

<!-- 贡献者 -->

## 贡献者

- 54dbd

- Freddie_1946

- Aegis1863

<!-- 许可证 -->

## 许可证

本项目基于 GPL-3.0 许可证分发。详情请查看 LICENSE.txt 文件。


[contributors-shield]: https://img.shields.io/github/contributors/54dbd/Bibtex-to-gbt7714.svg?style=for-the-badge

[contributors-url]: https://github.com/54dbd/Bibtex-to-gbt7714/graphs/contributors

[forks-shield]: https://img.shields.io/github/forks/54dbd/Bibtex-to-gbt7714.svg?style=for-the-badge

[forks-url]: https://github.com/54dbd/Bibtex-to-gbt7714/network/members

[stars-shield]: https://img.shields.io/github/stars/54dbd/Bibtex-to-gbt7714.svg?style=for-the-badge

[stars-url]: https://github.com/54dbd/Bibtex-to-gbt7714/stargazers

[issues-shield]: https://img.shields.io/github/issues/54dbd/Bibtex-to-gbt7714.svg?style=for-the-badge

[issues-url]: https://github.com/54dbd/Bibtex-to-gbt7714/issues

[license-shield]: https://img.shields.io/github/license/54dbd/Bibtex-to-gbt7714.svg?style=for-the-badge

[license-url]: https://github.com/54dbd/Bibtex-to-gbt7714/blob/master/LICENSE.txt

[patreon-shield]: https://img.shields.io/badge/-patreon-black.svg?style=for-the-badge&logo=patreon&colorB=555

[patreon-url]: https://patreon.com/rosszhu?utm_medium=unknown&utm_source=join_link&utm_campaign=creatorshare_creator&utm_content=copyLink
