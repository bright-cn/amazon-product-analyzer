<div align="center">
  <a href="https://www.bright.cn/">
    <img src="https://mintlify.s3.us-west-1.amazonaws.com/brightdata/logo/light.svg" width="300" alt="Bright Data 标志">
  </a>

# 🛍️ 亚马逊产品分析
借助 AI 驱动的洞察、交互式可视化以及覆盖全球站点的可靠数据采集，分析亚马逊产品数据并追踪市场趋势。

<img src="https://img.shields.io/badge/python-3.9+-blue" />
<img src="https://img.shields.io/badge/Gemini-API-blueviolet" />
<img src="https://img.shields.io/badge/License-MIT-blue" />
</div>

<div align="center">

https://github.com/user-attachments/assets/d6248647-4c3d-4bfc-a653-0ec79ae0d4a7

</div>

---

## 🎯 主要特性
- 多站点分析：覆盖 23 个亚马逊站点，获得深度洞察。
- 新鲜数据：通过 Bright Data 的 [Amazon Scraper API](https://www.bright.cn/products/web-scraper/amazon) 获取。
- 交互式仪表板：价格分布、评分分析等可视化图表。
- AI 驱动洞察：支持自然语言提问并给出推荐。
- 优惠检测：识别折扣与促销机会。
- 数据导出：下载 CSV 以便进一步分析与报告。

## 💡 使用场景
- 产品调研：在目标市场中找到性价比最高的产品。
- 价格分析：了解价格分布与竞争定位。
- 优惠挖掘：识别真实折扣与促销机会。
- 质量评估：分析评分与价格关系，寻找最佳平衡点。
- 市场定位：查看产品在搜索结果中的排名。
- 购买决策：获得 AI 驱动的购买建议。

## 🎯 工作原理
- 选择站点：从包含美国、加拿大、英国、德国、日本、印度等在内的 23 个全球站点中选择目标市场。每个站点使用当地货币与定价。
- 搜索产品：输入关键词（例如：“无线耳机”“iPhone 15”“咖啡机”）或从热门搜索中选择。
- 获取智能分析：自动生成全面的市场洞察，包括价格分布模式、质量与价格分析、优惠情报、价值评分、竞争定位以及搜索排名。
- 接收智能推荐：基于 AI 的产品推荐，包括总体性价比最佳、评分最高以及高额优惠的最佳选择。
- 使用 AI 助手：可用自然语言提问，例如“哪款产品性价比最高？”或“给我看看 50 美元以下高评分的选项”。
- 筛选并导出：按价格区间、Prime 资格、评分与优惠进行筛选，并导出为 CSV 进行深度分析。

## 🌍 支持的亚马逊站点
可从 23 个主要站点中选择：
- 北美：美国、加拿大、墨西哥。
- 欧洲：英国、德国、法国、意大利、西班牙、荷兰、瑞典、波兰。
- 亚太地区：日本、澳大利亚、印度、新加坡。
- 其他地区：巴西、爱尔兰、比利时、土耳其、阿联酋、沙特阿拉伯、埃及、南非。

> 注：应用一次仅支持一个站点，以反映本地定价、排名与可用性差异。

## 🚀 快速开始

### 先决条件

- Python 3.9+ – [点击下载](https://www.python.org/downloads/)
- Bright Data API 密钥 – [获取你的 API 密钥](https://docs.brightdata.com/api-reference/authentication#how-do-i-generate-a-new-api-key%3F)
- Google Gemini API 密钥 – [生成 API 密钥](https://aistudio.google.com/apikey)

### 安装

```bash
# 克隆仓库
git clone https://github.com/triposat/amazon-product-analytics.git
cd amazon-product-analytics

# 安装依赖
pip install -r requirements.txt

# 配置 API 凭据
cp .env.example .env
# 编辑 .env 文件并添加你的 API 密钥
```

### 配置

设置环境变量：
```bash
BRIGHT_DATA_API_KEY=your_bright_data_api_key_here
GEMINI_API_KEY=your_google_gemini_api_key_here
```

### 启动应用

```bash
# 启动仪表板
streamlit run streamlit_app.py

# 可选：使用运行脚本
./run_app.sh
```

🎉 在此访问你的仪表板：[http://localhost:8501](http://localhost:8501/)

## 🛠️ 技术栈

| 组件              | 技术                                                                                              | 用途                       |
| ----------------- | ------------------------------------------------------------------------------------------------- | -------------------------- |
| 前端              | [Streamlit](https://streamlit.io/)                                                                | 交互式网页仪表板           |
| 数据来源          | [Bright Data Amazon Scraper API](https://www.bright.cn/products/web-scraper/amazon)              | 可靠的亚马逊数据采集       |
| 处理              | [Pandas](https://pandas.pydata.org/)                                                              | 数据分析与处理             |
| 可视化            | [Plotly](https://plotly.com/python/)                                                              | 交互式图表与图形           |
| AI 集成           | [Google Gemini](https://ai.google.dev/)                                                           | 自然语言洞察               |
| HTTP 与重试       | [Requests](https://pypi.org/project/requests/) + [Tenacity](https://pypi.org/project/tenacity/)   | 稳健的 API 通信            |

## 📚 更多资源
1. 深入示例——在此指南仓库中探索 Bright Data 的 Amazon Scraper 示例与使用模式：[链接](https://github.com/bright-cn/Amazon-scraper)
2. 急需数据？使用 [Amazon Datasets](https://www.bright.cn/products/datasets/amazon) 获取新鲜、已验证的数据，支持多种交付格式
3. 工具对比——查看这篇[热门亚马逊抓取器概览](https://www.bright.cn/blog/web-data/best-amazon-scrapers)及各自适用场景

## 🤝 支持
需要帮助？我们随时为你提供支持。[立即联系我们](https://www.bright.cn/contact)。
