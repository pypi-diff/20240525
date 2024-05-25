# Comparing `tmp/scrapegraphai-1.5.0b2.tar.gz` & `tmp/scrapegraphai-1.5.0b3.tar.gz`

## Comparing `scrapegraphai-1.5.0b2.tar` & `scrapegraphai-1.5.0b3.tar`

### file list

```diff
@@ -1,285 +1,276 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/.gitattributes
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/.releaserc.yml
--rw-r--r--   0        0        0    46740 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/CHANGELOG.md
--rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/CONTRIBUTING.md
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/Dockerfile
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/SECURITY.md
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/citation.cff
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docker-compose.yml
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/readthedocs.yml
--rw-r--r--   0        0        0     7557 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/requirements-dev.lock
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/requirements-dev.txt
--rw-r--r--   0        0        0     7372 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/requirements.lock
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/requirements.txt
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/.github/ISSUE_TEMPLATE/custom.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/.github/workflows/codeql.yml
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/.github/workflows/dependency-review.yml
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/.github/workflows/pylint.yml
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/.github/workflows/release.yml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/Makefile
--rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/README.md
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/make.bat
--rw-r--r--   0        0        0    60520 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/assets/apikey_1.png
--rw-r--r--   0        0        0   123826 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/assets/apikey_2.png
--rw-r--r--   0        0        0    60775 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/assets/apikey_3.png
--rw-r--r--   0        0        0    86914 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/assets/apikey_4.png
--rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/assets/codespaces-badge.png
--rw-r--r--   0        0        0  1178826 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/assets/logo_authors.png
--rw-r--r--   0        0        0    73949 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/assets/omniscrapergraph.png
--rw-r--r--   0        0        0    58062 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/assets/omnisearchgraph.png
--rw-r--r--   0        0        0    53007 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/assets/project_overview_diagram.fig
--rw-r--r--   0        0        0    83949 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/assets/project_overview_diagram.png
--rw-r--r--   0        0        0    33264 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/assets/scrapegraphai_logo.png
--rw-r--r--   0        0        0    54611 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/assets/searchgraph.png
--rw-r--r--   0        0        0    15508 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/assets/serp_api_logo.png
--rw-r--r--   0        0        0    61095 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/assets/smartscrapergraph.png
--rw-r--r--   0        0        0    49312 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/assets/speechgraph.png
--rw-r--r--   0        0        0   221972 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/assets/transparent_stat.png
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/source/conf.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/source/index.rst
--rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/source/getting_started/examples.rst
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/source/getting_started/installation.rst
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/source/introduction/contributing.rst
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/source/introduction/overview.rst
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/source/modules/modules.rst
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/source/modules/scrapegraphai.graphs.rst
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/source/modules/scrapegraphai.nodes.rst
--rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/source/modules/scrapegraphai.rst
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/source/scrapers/benchmarks.rst
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/source/scrapers/graph_config.rst
--rw-r--r--   0        0        0     5646 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/source/scrapers/graphs.rst
--rw-r--r--   0        0        0     5568 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/source/scrapers/llm.rst
--rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/readme.md
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/anthropic/smart_scraper_haiku.py
--rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/azure/json_scraper_azure.py
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/azure/search_graph_azure.py
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/azure/smart_scraper_azure_openai.py
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/azure/xml_scraper_azure.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/azure/inputs/books.xml
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/azure/inputs/example.json
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/azure/inputs/username.csv
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/bedrock/.env.example
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/bedrock/README.md
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/bedrock/csv_scraper_bedrock.py
--rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/bedrock/custom_graph_bedrock.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/bedrock/json_scraper_bedrock.py
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/bedrock/scrape_plain_text_bedrock.py
--rw-r--r--   0        0        0    82480 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/bedrock/scrapegraphai_bedrock.png
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/bedrock/script_generator_bedrock.py
--rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/bedrock/search_graph_bedrock.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/bedrock/smart_scraper_bedrock.py
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/bedrock/xml_scraper_bedrock.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/bedrock/inputs/books.xml
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/bedrock/inputs/example.json
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/bedrock/inputs/plain_html_example.txt
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/bedrock/inputs/username.csv
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/benchmarks/readme.md
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/benchmarks/GenerateScraper/.env.example
--rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/benchmarks/GenerateScraper/Readme.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/benchmarks/GenerateScraper/benchmark_docker.py
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/benchmarks/GenerateScraper/benchmark_groq.py
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/benchmarks/GenerateScraper/benchmark_llama3.py
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/benchmarks/GenerateScraper/benchmark_mistral.py
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/benchmarks/GenerateScraper/benchmark_openai_gpt35.py
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/benchmarks/GenerateScraper/benchmark_openai_gpt4.py
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/benchmarks/GenerateScraper/inputs/example_1.txt
--rw-r--r--   0        0        0  2590773 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/benchmarks/GenerateScraper/inputs/example_2.txt
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/benchmarks/SmartScraper/.env.example
--rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/benchmarks/SmartScraper/Readme.md
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/benchmarks/SmartScraper/benchmark_docker.py
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/benchmarks/SmartScraper/benchmark_groq.py
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/benchmarks/SmartScraper/benchmark_llama3.py
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/benchmarks/SmartScraper/benchmark_mistral.py
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/benchmarks/SmartScraper/benchmark_openai_gpt35.py
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/benchmarks/SmartScraper/benchmark_openai_gpt4.py
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/benchmarks/SmartScraper/inputs/example_1.txt
--rw-r--r--   0        0        0  2590773 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/benchmarks/SmartScraper/inputs/example_2.txt
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/deepseek/.env.example
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/deepseek/csv_scraper_deepseek.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/deepseek/json_scraper_deepseek.py
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/deepseek/script_generator_deepseek.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/deepseek/search_graph_deepseek.py
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/deepseek/smart_scarper_deepseek.py
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/deepseek/xml_scraper_deepseek.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/deepseek/inputs/books.xml
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/deepseek/inputs/example.json
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/deepseek/inputs/username.csv
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/gemini/.env.example
--rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/gemini/csv_scraper_gemini.py
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/gemini/custom_graph_gemini.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/gemini/json_scraper_gemini.py
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/gemini/readme.md
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/gemini/scrape_plain_text_gemini.py
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/gemini/scrape_xml_gemini.py
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/gemini/script_generator_gemini.py
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/gemini/search_graph_gemini.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/gemini/smart_scraper_gemini.py
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/gemini/xml_scraper_openai.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/gemini/inputs/books.xml
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/gemini/inputs/example.json
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/gemini/inputs/plain_html_example.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/gemini/inputs/username.csv
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/groq/.env.example
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/groq/search_graph_groq_openai.py
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/groq/smart_scraper_groq_ollama.py
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/groq/smart_scraper_groq_openai.py
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/huggingfacehub/smart_scraper_huggingfacehub.py
--rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/knowledge_graph/kg_custom_graph.py
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/knowledge_graph/load_vector.py
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/knowledge_graph/save_vector.py
--rw-r--r--   0        0        0    20332 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/knowledge_graph/input/job_postings.json
--rw-r--r--   0        0        0   399405 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/knowledge_graph/output/faiss_index/index.faiss
--rw-r--r--   0        0        0    14447 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/knowledge_graph/output/faiss_index/index.pkl
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/local_models/csv_scraper_ollama.py
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/local_models/json_scraper_ollama.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/local_models/scrape_plain_text_ollama.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/local_models/scrape_xml_ollama.py
--rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/local_models/script_generator_ollama.py
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/local_models/search_graph_ollama.py
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/local_models/smart_scraper_ollama.py
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/local_models/xml_scraper_ollama.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/local_models/inputs/books.xml
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/local_models/inputs/example.json
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/local_models/inputs/plain_html_example.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/local_models/inputs/username.csv
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/mixed_models/.env.example
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/mixed_models/readme.md
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/mixed_models/search_graph_groq_ollama.py
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/mixed_models/smart_scraper_mixed.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/mixed_models/inputs/books.xml
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/mixed_models/inputs/example.json
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/mixed_models/inputs/plain_html_example.txt
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/openai/.env.example
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/openai/csv_scraper_openai.py
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/openai/custom_graph_openai.py
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/openai/deep_scraper_openai.py
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/openai/json_scraper_openai.py
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/openai/omni_scraper_openai.py
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/openai/omni_search_graph_openai.py
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/openai/pdf_scraper_openai.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/openai/readme.md
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/openai/scrape_plain_text_openai.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/openai/script_generator_openai.py
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/openai/search_graph_openai.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/openai/smart_scraper_multi_openai.py
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/openai/smart_scraper_openai.py
--rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/openai/smart_scraper_schema_openai.py
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/openai/speech_graph_openai.py
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/openai/xml_scraper_openai.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/openai/inputs/books.xml
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/openai/inputs/example.json
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/openai/inputs/plain_html_example.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/openai/inputs/username.csv
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/single_node/fetch_node.py
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/single_node/image2text_node.py
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/single_node/kg_node.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/single_node/robot_node.py
--rwxr-xr-x   0        0        0      986 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/manual deployment/commit_and_push.sh
--rwxr-xr-x   0        0        0      611 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/manual deployment/commit_and_push_with_tests.sh
--rwxr-xr-x   0        0        0      169 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/manual deployment/deploy_on_pip.sh
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/manual deployment/installation.sh
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/__init__.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/builders/__init__.py
--rw-r--r--   0        0        0     6653 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/builders/graph_builder.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/docloaders/__init__.py
--rw-r--r--   0        0        0     4649 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/docloaders/chromium.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/graphs/__init__.py
--rw-r--r--   0        0        0    14947 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/graphs/abstract_graph.py
--rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/graphs/base_graph.py
--rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/graphs/csv_scraper_graph.py
--rw-r--r--   0        0        0     5748 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/graphs/deep_scraper_graph.py
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/graphs/json_scraper_graph.py
--rw-r--r--   0        0        0     4501 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/graphs/omni_scraper_graph.py
--rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/graphs/omni_search_graph.py
--rw-r--r--   0        0        0     3397 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/graphs/pdf_scraper_graph.py
--rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/graphs/script_creator_graph.py
--rw-r--r--   0        0        0     3954 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/graphs/search_graph.py
--rw-r--r--   0        0        0     3868 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/graphs/smart_scraper_graph.py
--rw-r--r--   0        0        0     3733 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/graphs/smart_scraper_multi_graph.py
--rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/graphs/speech_graph.py
--rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/graphs/xml_scraper_graph.py
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/helpers/__init__.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/helpers/generate_answer_node_csv_prompts.py
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/helpers/generate_answer_node_omni_prompts.py
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/helpers/generate_answer_node_pdf_prompts.py
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/helpers/generate_answer_node_prompts.py
--rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/helpers/models_tokens.py
--rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/helpers/nodes_metadata.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/helpers/robots.py
--rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/helpers/schemas.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/models/__init__.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/models/anthropic.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/models/azure_openai.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/models/bedrock.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/models/deepseek.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/models/gemini.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/models/groq.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/models/hugging_face.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/models/ollama.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/models/openai.py
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/models/openai_itt.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/models/openai_tts.py
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/nodes/__init__.py
--rw-r--r--   0        0        0     8903 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/nodes/base_node.py
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/nodes/blocks_identifier.py
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/nodes/conditional_node.py
--rw-r--r--   0        0        0     6553 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/nodes/fetch_node.py
--rw-r--r--   0        0        0     5779 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/nodes/generate_answer_csv_node.py
--rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/nodes/generate_answer_node.py
--rw-r--r--   0        0        0     5301 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/nodes/generate_answer_omni_node.py
--rw-r--r--   0        0        0     5757 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/nodes/generate_answer_pdf_node.py
--rw-r--r--   0        0        0     4424 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/nodes/generate_scraper_node.py
--rw-r--r--   0        0        0     3757 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/nodes/get_probable_tags_node.py
--rw-r--r--   0        0        0     4603 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/nodes/graph_iterator_node.py
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/nodes/image_to_text_node.py
--rw-r--r--   0        0        0     3970 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/nodes/knowledge_graph_node.py
--rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/nodes/merge_answers_node.py
--rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/nodes/parse_node.py
--rw-r--r--   0        0        0     4565 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/nodes/rag_node.py
--rw-r--r--   0        0        0     6342 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/nodes/robots_node.py
--rw-r--r--   0        0        0     4218 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/nodes/search_internet_node.py
--rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/nodes/search_link_node.py
--rw-r--r--   0        0        0     4992 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/nodes/search_node_with_context.py
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/nodes/text_to_speech_node.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/utils/__init__.py
--rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/utils/cleanup_html.py
--rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/utils/convert_to_csv.py
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/utils/convert_to_json.py
--rw-r--r--   0        0        0     6364 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/utils/knowledge_graph.py
--rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/utils/logging.py
--rw-r--r--   0        0        0     4638 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/utils/parse_state_keys.py
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/utils/prettify_exec_info.py
--rw-r--r--   0        0        0     6404 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/utils/proxy_rotation.py
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/utils/research_web.py
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/utils/save_audio_from_bytes.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/utils/sys_dynamic_import.py
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/utils/token_calculator.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/tests/Readme.md
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/tests/graphs/scrape_json_ollama.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/tests/graphs/scrape_plain_text_llama3_test.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/tests/graphs/scrape_plain_text_mistral_test.py
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/tests/graphs/scrape_xml_ollama_test.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/tests/graphs/script_generator_test.py
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/tests/graphs/smart_scraper_ollama_test.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/tests/graphs/inputs/books.xml
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/tests/graphs/inputs/example.json
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/tests/graphs/inputs/plain_html_example.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/tests/graphs/inputs/username.csv
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/tests/nodes/fetch_node_test.py
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/tests/nodes/robot_node_test.py
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/tests/nodes/search_link_node_test.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/tests/nodes/inputs/books.xml
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/tests/nodes/inputs/example.json
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/tests/nodes/inputs/plain_html_example.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/tests/nodes/inputs/username.csv
--rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/tests/utils/test_proxy_rotation.py
--rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/tests/utils/test_sys_dynamic_import.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/LICENSE
--rw-r--r--   0        0        0     9182 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/README.md
--rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/pyproject.toml
--rw-r--r--   0        0        0    10804 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/.gitattributes
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/.releaserc.yml
+-rw-r--r--   0        0        0    47020 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/CHANGELOG.md
+-rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/CONTRIBUTING.md
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/Dockerfile
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/SECURITY.md
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/citation.cff
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docker-compose.yml
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/readthedocs.yml
+-rw-r--r--   0        0        0     7557 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/requirements-dev.lock
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/requirements-dev.txt
+-rw-r--r--   0        0        0     7372 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/requirements.lock
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/requirements.txt
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/.github/ISSUE_TEMPLATE/custom.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/.github/workflows/dependency-review.yml
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/.github/workflows/release.yml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/Makefile
+-rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/README.md
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/make.bat
+-rw-r--r--   0        0        0    60520 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/assets/apikey_1.png
+-rw-r--r--   0        0        0   123826 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/assets/apikey_2.png
+-rw-r--r--   0        0        0    60775 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/assets/apikey_3.png
+-rw-r--r--   0        0        0    86914 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/assets/apikey_4.png
+-rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/assets/codespaces-badge.png
+-rw-r--r--   0        0        0  1178826 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/assets/logo_authors.png
+-rw-r--r--   0        0        0    73949 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/assets/omniscrapergraph.png
+-rw-r--r--   0        0        0    58062 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/assets/omnisearchgraph.png
+-rw-r--r--   0        0        0    53007 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/assets/project_overview_diagram.fig
+-rw-r--r--   0        0        0    83949 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/assets/project_overview_diagram.png
+-rw-r--r--   0        0        0    33264 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/assets/scrapegraphai_logo.png
+-rw-r--r--   0        0        0    54611 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/assets/searchgraph.png
+-rw-r--r--   0        0        0    15508 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/assets/serp_api_logo.png
+-rw-r--r--   0        0        0    61095 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/assets/smartscrapergraph.png
+-rw-r--r--   0        0        0    49312 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/assets/speechgraph.png
+-rw-r--r--   0        0        0   221972 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/assets/transparent_stat.png
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/source/conf.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/source/index.rst
+-rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/source/getting_started/examples.rst
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/source/getting_started/installation.rst
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/source/introduction/contributing.rst
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/source/introduction/overview.rst
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/source/modules/modules.rst
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/source/modules/scrapegraphai.graphs.rst
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/source/modules/scrapegraphai.nodes.rst
+-rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/source/modules/scrapegraphai.rst
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/source/scrapers/benchmarks.rst
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/source/scrapers/graph_config.rst
+-rw-r--r--   0        0        0     5646 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/source/scrapers/graphs.rst
+-rw-r--r--   0        0        0     5568 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/source/scrapers/llm.rst
+-rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/readme.md
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/anthropic/smart_scraper_haiku.py
+-rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/azure/json_scraper_azure.py
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/azure/search_graph_azure.py
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/azure/smart_scraper_azure_openai.py
+-rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/azure/xml_scraper_azure.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/azure/inputs/books.xml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/azure/inputs/example.json
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/azure/inputs/username.csv
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/bedrock/.env.example
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/bedrock/README.md
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/bedrock/csv_scraper_bedrock.py
+-rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/bedrock/custom_graph_bedrock.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/bedrock/json_scraper_bedrock.py
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/bedrock/scrape_plain_text_bedrock.py
+-rw-r--r--   0        0        0    82480 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/bedrock/scrapegraphai_bedrock.png
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/bedrock/script_generator_bedrock.py
+-rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/bedrock/search_graph_bedrock.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/bedrock/smart_scraper_bedrock.py
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/bedrock/xml_scraper_bedrock.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/bedrock/inputs/books.xml
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/bedrock/inputs/example.json
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/bedrock/inputs/plain_html_example.txt
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/bedrock/inputs/username.csv
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/benchmarks/readme.md
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/benchmarks/GenerateScraper/.env.example
+-rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/benchmarks/GenerateScraper/Readme.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/benchmarks/GenerateScraper/benchmark_docker.py
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/benchmarks/GenerateScraper/benchmark_groq.py
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/benchmarks/GenerateScraper/benchmark_llama3.py
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/benchmarks/GenerateScraper/benchmark_mistral.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/benchmarks/GenerateScraper/benchmark_openai_gpt35.py
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/benchmarks/GenerateScraper/benchmark_openai_gpt4.py
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/benchmarks/GenerateScraper/inputs/example_1.txt
+-rw-r--r--   0        0        0  2590773 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/benchmarks/GenerateScraper/inputs/example_2.txt
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/benchmarks/SmartScraper/.env.example
+-rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/benchmarks/SmartScraper/Readme.md
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/benchmarks/SmartScraper/benchmark_docker.py
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/benchmarks/SmartScraper/benchmark_groq.py
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/benchmarks/SmartScraper/benchmark_llama3.py
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/benchmarks/SmartScraper/benchmark_mistral.py
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/benchmarks/SmartScraper/benchmark_openai_gpt35.py
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/benchmarks/SmartScraper/benchmark_openai_gpt4.py
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/benchmarks/SmartScraper/inputs/example_1.txt
+-rw-r--r--   0        0        0  2590773 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/benchmarks/SmartScraper/inputs/example_2.txt
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/deepseek/.env.example
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/deepseek/csv_scraper_deepseek.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/deepseek/json_scraper_deepseek.py
+-rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/deepseek/script_generator_deepseek.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/deepseek/search_graph_deepseek.py
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/deepseek/smart_scarper_deepseek.py
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/deepseek/xml_scraper_deepseek.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/deepseek/inputs/books.xml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/deepseek/inputs/example.json
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/deepseek/inputs/username.csv
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/gemini/.env.example
+-rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/gemini/csv_scraper_gemini.py
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/gemini/custom_graph_gemini.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/gemini/json_scraper_gemini.py
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/gemini/readme.md
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/gemini/scrape_plain_text_gemini.py
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/gemini/scrape_xml_gemini.py
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/gemini/script_generator_gemini.py
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/gemini/search_graph_gemini.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/gemini/smart_scraper_gemini.py
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/gemini/xml_scraper_openai.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/gemini/inputs/books.xml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/gemini/inputs/example.json
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/gemini/inputs/plain_html_example.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/gemini/inputs/username.csv
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/groq/.env.example
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/groq/search_graph_groq_openai.py
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/groq/smart_scraper_groq_ollama.py
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/groq/smart_scraper_groq_openai.py
+-rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/huggingfacehub/smart_scraper_huggingfacehub.py
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/local_models/csv_scraper_ollama.py
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/local_models/json_scraper_ollama.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/local_models/scrape_plain_text_ollama.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/local_models/scrape_xml_ollama.py
+-rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/local_models/script_generator_ollama.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/local_models/search_graph_ollama.py
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/local_models/smart_scraper_ollama.py
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/local_models/xml_scraper_ollama.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/local_models/inputs/books.xml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/local_models/inputs/example.json
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/local_models/inputs/plain_html_example.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/local_models/inputs/username.csv
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/mixed_models/.env.example
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/mixed_models/readme.md
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/mixed_models/search_graph_groq_ollama.py
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/mixed_models/smart_scraper_mixed.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/mixed_models/inputs/books.xml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/mixed_models/inputs/example.json
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/mixed_models/inputs/plain_html_example.txt
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/openai/.env.example
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/openai/csv_scraper_openai.py
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/openai/custom_graph_openai.py
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/openai/deep_scraper_openai.py
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/openai/json_scraper_openai.py
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/openai/omni_scraper_openai.py
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/openai/omni_search_graph_openai.py
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/openai/pdf_scraper_openai.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/openai/readme.md
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/openai/scrape_plain_text_openai.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/openai/script_generator_openai.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/openai/search_graph_openai.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/openai/smart_scraper_multi_openai.py
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/openai/smart_scraper_openai.py
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/openai/smart_scraper_schema_openai.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/openai/speech_graph_openai.py
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/openai/xml_scraper_openai.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/openai/inputs/books.xml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/openai/inputs/example.json
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/openai/inputs/plain_html_example.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/openai/inputs/username.csv
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/single_node/fetch_node.py
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/single_node/image2text_node.py
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/single_node/kg_node.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/single_node/robot_node.py
+-rwxr-xr-x   0        0        0      986 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/manual deployment/commit_and_push.sh
+-rwxr-xr-x   0        0        0      611 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/manual deployment/commit_and_push_with_tests.sh
+-rwxr-xr-x   0        0        0      169 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/manual deployment/deploy_on_pip.sh
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/manual deployment/installation.sh
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/__init__.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/builders/__init__.py
+-rw-r--r--   0        0        0     6653 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/builders/graph_builder.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/docloaders/__init__.py
+-rw-r--r--   0        0        0     4649 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/docloaders/chromium.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/graphs/__init__.py
+-rw-r--r--   0        0        0    14947 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/graphs/abstract_graph.py
+-rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/graphs/base_graph.py
+-rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/graphs/csv_scraper_graph.py
+-rw-r--r--   0        0        0     5748 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/graphs/deep_scraper_graph.py
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/graphs/json_scraper_graph.py
+-rw-r--r--   0        0        0     4501 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/graphs/omni_scraper_graph.py
+-rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/graphs/omni_search_graph.py
+-rw-r--r--   0        0        0     3397 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/graphs/pdf_scraper_graph.py
+-rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/graphs/script_creator_graph.py
+-rw-r--r--   0        0        0     3954 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/graphs/search_graph.py
+-rw-r--r--   0        0        0     3868 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/graphs/smart_scraper_graph.py
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/graphs/smart_scraper_multi_graph.py
+-rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/graphs/speech_graph.py
+-rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/graphs/xml_scraper_graph.py
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/helpers/__init__.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/helpers/generate_answer_node_csv_prompts.py
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/helpers/generate_answer_node_omni_prompts.py
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/helpers/generate_answer_node_pdf_prompts.py
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/helpers/generate_answer_node_prompts.py
+-rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/helpers/models_tokens.py
+-rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/helpers/nodes_metadata.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/helpers/robots.py
+-rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/helpers/schemas.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/models/__init__.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/models/anthropic.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/models/azure_openai.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/models/bedrock.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/models/deepseek.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/models/gemini.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/models/groq.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/models/hugging_face.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/models/ollama.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/models/openai.py
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/models/openai_itt.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/models/openai_tts.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/nodes/__init__.py
+-rw-r--r--   0        0        0     8903 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/nodes/base_node.py
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/nodes/conditional_node.py
+-rw-r--r--   0        0        0     6553 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/nodes/fetch_node.py
+-rw-r--r--   0        0        0     5779 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/nodes/generate_answer_csv_node.py
+-rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/nodes/generate_answer_node.py
+-rw-r--r--   0        0        0     5301 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/nodes/generate_answer_omni_node.py
+-rw-r--r--   0        0        0     5757 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/nodes/generate_answer_pdf_node.py
+-rw-r--r--   0        0        0     4424 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/nodes/generate_scraper_node.py
+-rw-r--r--   0        0        0     3757 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/nodes/get_probable_tags_node.py
+-rw-r--r--   0        0        0     4603 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/nodes/graph_iterator_node.py
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/nodes/image_to_text_node.py
+-rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/nodes/merge_answers_node.py
+-rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/nodes/parse_node.py
+-rw-r--r--   0        0        0     4565 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/nodes/rag_node.py
+-rw-r--r--   0        0        0     6342 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/nodes/robots_node.py
+-rw-r--r--   0        0        0     4218 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/nodes/search_internet_node.py
+-rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/nodes/search_link_node.py
+-rw-r--r--   0        0        0     4992 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/nodes/search_node_with_context.py
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/nodes/text_to_speech_node.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/utils/__init__.py
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/utils/cleanup_html.py
+-rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/utils/convert_to_csv.py
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/utils/convert_to_json.py
+-rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/utils/logging.py
+-rw-r--r--   0        0        0     4638 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/utils/parse_state_keys.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/utils/prettify_exec_info.py
+-rw-r--r--   0        0        0     6404 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/utils/proxy_rotation.py
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/utils/research_web.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/utils/save_audio_from_bytes.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/utils/sys_dynamic_import.py
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/utils/token_calculator.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/tests/Readme.md
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/tests/graphs/scrape_json_ollama.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/tests/graphs/scrape_plain_text_llama3_test.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/tests/graphs/scrape_plain_text_mistral_test.py
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/tests/graphs/scrape_xml_ollama_test.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/tests/graphs/script_generator_test.py
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/tests/graphs/smart_scraper_ollama_test.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/tests/graphs/inputs/books.xml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/tests/graphs/inputs/example.json
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/tests/graphs/inputs/plain_html_example.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/tests/graphs/inputs/username.csv
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/tests/nodes/fetch_node_test.py
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/tests/nodes/robot_node_test.py
+-rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/tests/nodes/search_link_node_test.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/tests/nodes/inputs/books.xml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/tests/nodes/inputs/example.json
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/tests/nodes/inputs/plain_html_example.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/tests/nodes/inputs/username.csv
+-rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/tests/utils/test_proxy_rotation.py
+-rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/tests/utils/test_sys_dynamic_import.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/LICENSE
+-rw-r--r--   0        0        0     9182 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/README.md
+-rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/pyproject.toml
+-rw-r--r--   0        0        0    10804 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/PKG-INFO
```

### Comparing `scrapegraphai-1.5.0b2/.releaserc.yml` & `scrapegraphai-1.5.0b3/.releaserc.yml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/CHANGELOG.md` & `scrapegraphai-1.5.0b3/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+## [1.5.0-beta.3](https://github.com/VinciGit00/Scrapegraph-ai/compare/v1.5.0-beta.2...v1.5.0-beta.3) (2024-05-24)
+
+
+### Bug Fixes
+
+* **kg:** removed unused nodes and utils ([5684578](https://github.com/VinciGit00/Scrapegraph-ai/commit/5684578fab635e862de58f7847ad736c6a57f766))
+
 ## [1.5.0-beta.2](https://github.com/VinciGit00/Scrapegraph-ai/compare/v1.5.0-beta.1...v1.5.0-beta.2) (2024-05-24)
 
 
 ### Bug Fixes
 
 * **pdf_scraper:** fix the pdf scraper gaph ([d00cde6](https://github.com/VinciGit00/Scrapegraph-ai/commit/d00cde60309935e283ba9116cf0b114e53cb9640))
 * **local_file:** fixed textual input pdf, csv, json and xml graph ([8d5eb0b](https://github.com/VinciGit00/Scrapegraph-ai/commit/8d5eb0bb0d5d008a63a96df94ce3842320376b8e))
```

### Comparing `scrapegraphai-1.5.0b2/CODE_OF_CONDUCT.md` & `scrapegraphai-1.5.0b3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/CONTRIBUTING.md` & `scrapegraphai-1.5.0b3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/readthedocs.yml` & `scrapegraphai-1.5.0b3/readthedocs.yml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/requirements-dev.lock` & `scrapegraphai-1.5.0b3/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/requirements.lock` & `scrapegraphai-1.5.0b3/requirements.lock`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/.github/ISSUE_TEMPLATE/bug_report.md` & `scrapegraphai-1.5.0b3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/.github/ISSUE_TEMPLATE/feature_request.md` & `scrapegraphai-1.5.0b3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/.github/workflows/codeql.yml` & `scrapegraphai-1.5.0b3/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/.github/workflows/dependency-review.yml` & `scrapegraphai-1.5.0b3/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/.github/workflows/pylint.yml` & `scrapegraphai-1.5.0b3/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/.github/workflows/python-publish.yml` & `scrapegraphai-1.5.0b3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/.github/workflows/release.yml` & `scrapegraphai-1.5.0b3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/docs/Makefile` & `scrapegraphai-1.5.0b3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/docs/README.md` & `scrapegraphai-1.5.0b3/docs/README.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/docs/make.bat` & `scrapegraphai-1.5.0b3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/docs/assets/apikey_1.png` & `scrapegraphai-1.5.0b3/docs/assets/apikey_1.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/docs/assets/apikey_2.png` & `scrapegraphai-1.5.0b3/docs/assets/apikey_2.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/docs/assets/apikey_3.png` & `scrapegraphai-1.5.0b3/docs/assets/apikey_3.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/docs/assets/apikey_4.png` & `scrapegraphai-1.5.0b3/docs/assets/apikey_4.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/docs/assets/codespaces-badge.png` & `scrapegraphai-1.5.0b3/docs/assets/codespaces-badge.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/docs/assets/logo_authors.png` & `scrapegraphai-1.5.0b3/docs/assets/logo_authors.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/docs/assets/omniscrapergraph.png` & `scrapegraphai-1.5.0b3/docs/assets/omniscrapergraph.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/docs/assets/omnisearchgraph.png` & `scrapegraphai-1.5.0b3/docs/assets/omnisearchgraph.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/docs/assets/project_overview_diagram.fig` & `scrapegraphai-1.5.0b3/docs/assets/project_overview_diagram.fig`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/docs/assets/project_overview_diagram.png` & `scrapegraphai-1.5.0b3/docs/assets/project_overview_diagram.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/docs/assets/scrapegraphai_logo.png` & `scrapegraphai-1.5.0b3/docs/assets/scrapegraphai_logo.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/docs/assets/searchgraph.png` & `scrapegraphai-1.5.0b3/docs/assets/searchgraph.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/docs/assets/serp_api_logo.png` & `scrapegraphai-1.5.0b3/docs/assets/serp_api_logo.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/docs/assets/smartscrapergraph.png` & `scrapegraphai-1.5.0b3/docs/assets/smartscrapergraph.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/docs/assets/speechgraph.png` & `scrapegraphai-1.5.0b3/docs/assets/speechgraph.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/docs/assets/transparent_stat.png` & `scrapegraphai-1.5.0b3/docs/assets/transparent_stat.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/docs/source/conf.py` & `scrapegraphai-1.5.0b3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/docs/source/index.rst` & `scrapegraphai-1.5.0b3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/docs/source/getting_started/examples.rst` & `scrapegraphai-1.5.0b3/docs/source/getting_started/examples.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/docs/source/getting_started/installation.rst` & `scrapegraphai-1.5.0b3/docs/source/getting_started/installation.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/docs/source/introduction/contributing.rst` & `scrapegraphai-1.5.0b3/docs/source/introduction/contributing.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/docs/source/introduction/overview.rst` & `scrapegraphai-1.5.0b3/docs/source/introduction/overview.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/docs/source/modules/scrapegraphai.graphs.rst` & `scrapegraphai-1.5.0b3/docs/source/modules/scrapegraphai.graphs.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/docs/source/modules/scrapegraphai.nodes.rst` & `scrapegraphai-1.5.0b3/docs/source/modules/scrapegraphai.nodes.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/docs/source/modules/scrapegraphai.rst` & `scrapegraphai-1.5.0b3/docs/source/modules/scrapegraphai.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/docs/source/scrapers/benchmarks.rst` & `scrapegraphai-1.5.0b3/docs/source/scrapers/benchmarks.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/docs/source/scrapers/graph_config.rst` & `scrapegraphai-1.5.0b3/docs/source/scrapers/graph_config.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/docs/source/scrapers/graphs.rst` & `scrapegraphai-1.5.0b3/docs/source/scrapers/graphs.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/docs/source/scrapers/llm.rst` & `scrapegraphai-1.5.0b3/docs/source/scrapers/llm.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/readme.md` & `scrapegraphai-1.5.0b3/examples/readme.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/anthropic/smart_scraper_haiku.py` & `scrapegraphai-1.5.0b3/examples/anthropic/smart_scraper_haiku.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/azure/json_scraper_azure.py` & `scrapegraphai-1.5.0b3/examples/azure/json_scraper_azure.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/azure/search_graph_azure.py` & `scrapegraphai-1.5.0b3/examples/azure/search_graph_azure.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/azure/smart_scraper_azure_openai.py` & `scrapegraphai-1.5.0b3/examples/azure/smart_scraper_azure_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/azure/xml_scraper_azure.py` & `scrapegraphai-1.5.0b3/examples/azure/xml_scraper_azure.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/azure/inputs/books.xml` & `scrapegraphai-1.5.0b3/examples/azure/inputs/books.xml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/azure/inputs/example.json` & `scrapegraphai-1.5.0b3/examples/azure/inputs/example.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/bedrock/csv_scraper_bedrock.py` & `scrapegraphai-1.5.0b3/examples/bedrock/csv_scraper_bedrock.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/bedrock/custom_graph_bedrock.py` & `scrapegraphai-1.5.0b3/examples/bedrock/custom_graph_bedrock.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/bedrock/json_scraper_bedrock.py` & `scrapegraphai-1.5.0b3/examples/bedrock/json_scraper_bedrock.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/bedrock/scrape_plain_text_bedrock.py` & `scrapegraphai-1.5.0b3/examples/bedrock/scrape_plain_text_bedrock.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/bedrock/scrapegraphai_bedrock.png` & `scrapegraphai-1.5.0b3/examples/bedrock/scrapegraphai_bedrock.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/bedrock/script_generator_bedrock.py` & `scrapegraphai-1.5.0b3/examples/bedrock/script_generator_bedrock.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/bedrock/search_graph_bedrock.py` & `scrapegraphai-1.5.0b3/examples/bedrock/search_graph_bedrock.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/bedrock/smart_scraper_bedrock.py` & `scrapegraphai-1.5.0b3/examples/bedrock/smart_scraper_bedrock.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/bedrock/xml_scraper_bedrock.py` & `scrapegraphai-1.5.0b3/examples/bedrock/xml_scraper_bedrock.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/bedrock/inputs/books.xml` & `scrapegraphai-1.5.0b3/examples/bedrock/inputs/books.xml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/bedrock/inputs/example.json` & `scrapegraphai-1.5.0b3/examples/bedrock/inputs/example.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/bedrock/inputs/plain_html_example.txt` & `scrapegraphai-1.5.0b3/examples/bedrock/inputs/plain_html_example.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/benchmarks/GenerateScraper/Readme.md` & `scrapegraphai-1.5.0b3/examples/benchmarks/GenerateScraper/Readme.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/benchmarks/GenerateScraper/benchmark_groq.py` & `scrapegraphai-1.5.0b3/examples/benchmarks/GenerateScraper/benchmark_groq.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/benchmarks/GenerateScraper/benchmark_llama3.py` & `scrapegraphai-1.5.0b3/examples/benchmarks/GenerateScraper/benchmark_llama3.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/benchmarks/GenerateScraper/benchmark_mistral.py` & `scrapegraphai-1.5.0b3/examples/benchmarks/GenerateScraper/benchmark_mistral.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/benchmarks/GenerateScraper/benchmark_openai_gpt35.py` & `scrapegraphai-1.5.0b3/examples/benchmarks/GenerateScraper/benchmark_openai_gpt35.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/benchmarks/GenerateScraper/benchmark_openai_gpt4.py` & `scrapegraphai-1.5.0b3/examples/benchmarks/GenerateScraper/benchmark_openai_gpt4.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/benchmarks/GenerateScraper/inputs/example_1.txt` & `scrapegraphai-1.5.0b3/examples/benchmarks/GenerateScraper/inputs/example_1.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/benchmarks/GenerateScraper/inputs/example_2.txt` & `scrapegraphai-1.5.0b3/examples/benchmarks/GenerateScraper/inputs/example_2.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/benchmarks/SmartScraper/Readme.md` & `scrapegraphai-1.5.0b3/examples/benchmarks/SmartScraper/Readme.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/benchmarks/SmartScraper/benchmark_docker.py` & `scrapegraphai-1.5.0b3/examples/benchmarks/SmartScraper/benchmark_docker.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/benchmarks/SmartScraper/benchmark_groq.py` & `scrapegraphai-1.5.0b3/examples/benchmarks/SmartScraper/benchmark_groq.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/benchmarks/SmartScraper/benchmark_llama3.py` & `scrapegraphai-1.5.0b3/examples/benchmarks/SmartScraper/benchmark_llama3.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/benchmarks/SmartScraper/benchmark_mistral.py` & `scrapegraphai-1.5.0b3/examples/benchmarks/SmartScraper/benchmark_mistral.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/benchmarks/SmartScraper/benchmark_openai_gpt35.py` & `scrapegraphai-1.5.0b3/examples/benchmarks/SmartScraper/benchmark_openai_gpt35.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/benchmarks/SmartScraper/benchmark_openai_gpt4.py` & `scrapegraphai-1.5.0b3/examples/benchmarks/SmartScraper/benchmark_openai_gpt4.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/benchmarks/SmartScraper/inputs/example_1.txt` & `scrapegraphai-1.5.0b3/examples/benchmarks/SmartScraper/inputs/example_1.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/benchmarks/SmartScraper/inputs/example_2.txt` & `scrapegraphai-1.5.0b3/examples/benchmarks/SmartScraper/inputs/example_2.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/deepseek/csv_scraper_deepseek.py` & `scrapegraphai-1.5.0b3/examples/deepseek/csv_scraper_deepseek.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/deepseek/json_scraper_deepseek.py` & `scrapegraphai-1.5.0b3/examples/deepseek/json_scraper_deepseek.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/deepseek/script_generator_deepseek.py` & `scrapegraphai-1.5.0b3/examples/deepseek/script_generator_deepseek.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/deepseek/search_graph_deepseek.py` & `scrapegraphai-1.5.0b3/examples/deepseek/search_graph_deepseek.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/deepseek/smart_scarper_deepseek.py` & `scrapegraphai-1.5.0b3/examples/deepseek/smart_scarper_deepseek.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/deepseek/xml_scraper_deepseek.py` & `scrapegraphai-1.5.0b3/examples/deepseek/xml_scraper_deepseek.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/deepseek/inputs/books.xml` & `scrapegraphai-1.5.0b3/examples/deepseek/inputs/books.xml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/deepseek/inputs/example.json` & `scrapegraphai-1.5.0b3/examples/deepseek/inputs/example.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/gemini/csv_scraper_gemini.py` & `scrapegraphai-1.5.0b3/examples/gemini/csv_scraper_gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/gemini/custom_graph_gemini.py` & `scrapegraphai-1.5.0b3/examples/gemini/custom_graph_gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/gemini/json_scraper_gemini.py` & `scrapegraphai-1.5.0b3/examples/gemini/json_scraper_gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/gemini/scrape_plain_text_gemini.py` & `scrapegraphai-1.5.0b3/examples/gemini/scrape_plain_text_gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/gemini/scrape_xml_gemini.py` & `scrapegraphai-1.5.0b3/examples/gemini/scrape_xml_gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/gemini/script_generator_gemini.py` & `scrapegraphai-1.5.0b3/examples/gemini/script_generator_gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/gemini/search_graph_gemini.py` & `scrapegraphai-1.5.0b3/examples/gemini/search_graph_gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/gemini/smart_scraper_gemini.py` & `scrapegraphai-1.5.0b3/examples/gemini/smart_scraper_gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/gemini/xml_scraper_openai.py` & `scrapegraphai-1.5.0b3/examples/gemini/xml_scraper_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/gemini/inputs/books.xml` & `scrapegraphai-1.5.0b3/examples/gemini/inputs/books.xml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/gemini/inputs/example.json` & `scrapegraphai-1.5.0b3/examples/gemini/inputs/example.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/gemini/inputs/plain_html_example.txt` & `scrapegraphai-1.5.0b3/examples/gemini/inputs/plain_html_example.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/groq/search_graph_groq_openai.py` & `scrapegraphai-1.5.0b3/examples/groq/search_graph_groq_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/groq/smart_scraper_groq_ollama.py` & `scrapegraphai-1.5.0b3/examples/groq/smart_scraper_groq_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/groq/smart_scraper_groq_openai.py` & `scrapegraphai-1.5.0b3/examples/groq/smart_scraper_groq_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/huggingfacehub/smart_scraper_huggingfacehub.py` & `scrapegraphai-1.5.0b3/examples/huggingfacehub/smart_scraper_huggingfacehub.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/local_models/csv_scraper_ollama.py` & `scrapegraphai-1.5.0b3/examples/local_models/csv_scraper_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/local_models/json_scraper_ollama.py` & `scrapegraphai-1.5.0b3/examples/local_models/json_scraper_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/local_models/scrape_plain_text_ollama.py` & `scrapegraphai-1.5.0b3/examples/local_models/scrape_plain_text_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/local_models/scrape_xml_ollama.py` & `scrapegraphai-1.5.0b3/examples/local_models/scrape_xml_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/local_models/script_generator_ollama.py` & `scrapegraphai-1.5.0b3/examples/local_models/script_generator_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/local_models/search_graph_ollama.py` & `scrapegraphai-1.5.0b3/examples/local_models/search_graph_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/local_models/smart_scraper_ollama.py` & `scrapegraphai-1.5.0b3/examples/local_models/smart_scraper_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/local_models/xml_scraper_ollama.py` & `scrapegraphai-1.5.0b3/examples/local_models/xml_scraper_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/local_models/inputs/books.xml` & `scrapegraphai-1.5.0b3/examples/local_models/inputs/books.xml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/local_models/inputs/example.json` & `scrapegraphai-1.5.0b3/examples/local_models/inputs/example.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/local_models/inputs/plain_html_example.txt` & `scrapegraphai-1.5.0b3/examples/local_models/inputs/plain_html_example.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/mixed_models/search_graph_groq_ollama.py` & `scrapegraphai-1.5.0b3/examples/mixed_models/search_graph_groq_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/mixed_models/smart_scraper_mixed.py` & `scrapegraphai-1.5.0b3/examples/mixed_models/smart_scraper_mixed.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/mixed_models/inputs/books.xml` & `scrapegraphai-1.5.0b3/examples/mixed_models/inputs/books.xml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/mixed_models/inputs/example.json` & `scrapegraphai-1.5.0b3/examples/mixed_models/inputs/example.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/mixed_models/inputs/plain_html_example.txt` & `scrapegraphai-1.5.0b3/examples/mixed_models/inputs/plain_html_example.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/openai/csv_scraper_openai.py` & `scrapegraphai-1.5.0b3/examples/openai/csv_scraper_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/openai/custom_graph_openai.py` & `scrapegraphai-1.5.0b3/examples/openai/custom_graph_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/openai/deep_scraper_openai.py` & `scrapegraphai-1.5.0b3/examples/openai/deep_scraper_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/openai/json_scraper_openai.py` & `scrapegraphai-1.5.0b3/examples/openai/json_scraper_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/openai/omni_scraper_openai.py` & `scrapegraphai-1.5.0b3/examples/openai/omni_scraper_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/openai/omni_search_graph_openai.py` & `scrapegraphai-1.5.0b3/examples/openai/omni_search_graph_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/openai/pdf_scraper_openai.py` & `scrapegraphai-1.5.0b3/examples/openai/pdf_scraper_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/openai/scrape_plain_text_openai.py` & `scrapegraphai-1.5.0b3/examples/openai/scrape_plain_text_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/openai/script_generator_openai.py` & `scrapegraphai-1.5.0b3/examples/openai/script_generator_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/openai/search_graph_openai.py` & `scrapegraphai-1.5.0b3/examples/openai/search_graph_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/openai/smart_scraper_multi_openai.py` & `scrapegraphai-1.5.0b3/examples/openai/smart_scraper_multi_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/openai/smart_scraper_openai.py` & `scrapegraphai-1.5.0b3/examples/openai/smart_scraper_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/openai/smart_scraper_schema_openai.py` & `scrapegraphai-1.5.0b3/examples/openai/smart_scraper_schema_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/openai/speech_graph_openai.py` & `scrapegraphai-1.5.0b3/examples/openai/speech_graph_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/openai/xml_scraper_openai.py` & `scrapegraphai-1.5.0b3/examples/openai/xml_scraper_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/openai/inputs/books.xml` & `scrapegraphai-1.5.0b3/examples/openai/inputs/books.xml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/openai/inputs/example.json` & `scrapegraphai-1.5.0b3/examples/openai/inputs/example.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/openai/inputs/plain_html_example.txt` & `scrapegraphai-1.5.0b3/examples/openai/inputs/plain_html_example.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/single_node/fetch_node.py` & `scrapegraphai-1.5.0b3/examples/single_node/fetch_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/single_node/image2text_node.py` & `scrapegraphai-1.5.0b3/examples/single_node/image2text_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/single_node/kg_node.py` & `scrapegraphai-1.5.0b3/examples/single_node/kg_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/examples/single_node/robot_node.py` & `scrapegraphai-1.5.0b3/examples/single_node/robot_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/manual deployment/commit_and_push.sh` & `scrapegraphai-1.5.0b3/manual deployment/commit_and_push.sh`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/manual deployment/commit_and_push_with_tests.sh` & `scrapegraphai-1.5.0b3/manual deployment/commit_and_push_with_tests.sh`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/builders/graph_builder.py` & `scrapegraphai-1.5.0b3/scrapegraphai/builders/graph_builder.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/docloaders/chromium.py` & `scrapegraphai-1.5.0b3/scrapegraphai/docloaders/chromium.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/graphs/__init__.py` & `scrapegraphai-1.5.0b3/scrapegraphai/graphs/__init__.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/graphs/abstract_graph.py` & `scrapegraphai-1.5.0b3/scrapegraphai/graphs/abstract_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/graphs/base_graph.py` & `scrapegraphai-1.5.0b3/scrapegraphai/graphs/base_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/graphs/csv_scraper_graph.py` & `scrapegraphai-1.5.0b3/scrapegraphai/graphs/csv_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/graphs/deep_scraper_graph.py` & `scrapegraphai-1.5.0b3/scrapegraphai/graphs/deep_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/graphs/json_scraper_graph.py` & `scrapegraphai-1.5.0b3/scrapegraphai/graphs/json_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/graphs/omni_scraper_graph.py` & `scrapegraphai-1.5.0b3/scrapegraphai/graphs/omni_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/graphs/omni_search_graph.py` & `scrapegraphai-1.5.0b3/scrapegraphai/graphs/omni_search_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/graphs/pdf_scraper_graph.py` & `scrapegraphai-1.5.0b3/scrapegraphai/graphs/pdf_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/graphs/script_creator_graph.py` & `scrapegraphai-1.5.0b3/scrapegraphai/graphs/script_creator_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/graphs/search_graph.py` & `scrapegraphai-1.5.0b3/scrapegraphai/graphs/search_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/graphs/smart_scraper_graph.py` & `scrapegraphai-1.5.0b3/scrapegraphai/graphs/smart_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/graphs/smart_scraper_multi_graph.py` & `scrapegraphai-1.5.0b3/scrapegraphai/graphs/smart_scraper_multi_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 
 from .base_graph import BaseGraph
 from .abstract_graph import AbstractGraph
 from .smart_scraper_graph import SmartScraperGraph
 
 from ..nodes import (
     GraphIteratorNode,
-    MergeAnswersNode,
-    KnowledgeGraphNode
+    MergeAnswersNode
 )
 
 
 class SmartScraperMultiGraph(AbstractGraph):
     """ 
     SmartScraperMultiGraph is a scraping pipeline that scrapes a list of URLs and generates answers to a given prompt.
     It only requires a user prompt and a list of URLs.
```

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/graphs/speech_graph.py` & `scrapegraphai-1.5.0b3/scrapegraphai/graphs/speech_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/graphs/xml_scraper_graph.py` & `scrapegraphai-1.5.0b3/scrapegraphai/graphs/xml_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/helpers/__init__.py` & `scrapegraphai-1.5.0b3/scrapegraphai/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/helpers/generate_answer_node_csv_prompts.py` & `scrapegraphai-1.5.0b3/scrapegraphai/helpers/generate_answer_node_csv_prompts.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/helpers/generate_answer_node_omni_prompts.py` & `scrapegraphai-1.5.0b3/scrapegraphai/helpers/generate_answer_node_omni_prompts.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/helpers/generate_answer_node_pdf_prompts.py` & `scrapegraphai-1.5.0b3/scrapegraphai/helpers/generate_answer_node_pdf_prompts.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/helpers/generate_answer_node_prompts.py` & `scrapegraphai-1.5.0b3/scrapegraphai/helpers/generate_answer_node_prompts.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/helpers/models_tokens.py` & `scrapegraphai-1.5.0b3/scrapegraphai/helpers/models_tokens.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/helpers/nodes_metadata.py` & `scrapegraphai-1.5.0b3/scrapegraphai/helpers/nodes_metadata.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/helpers/schemas.py` & `scrapegraphai-1.5.0b3/scrapegraphai/helpers/schemas.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/models/bedrock.py` & `scrapegraphai-1.5.0b3/scrapegraphai/models/bedrock.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/models/gemini.py` & `scrapegraphai-1.5.0b3/scrapegraphai/models/gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/models/openai_itt.py` & `scrapegraphai-1.5.0b3/scrapegraphai/models/openai_itt.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/models/openai_tts.py` & `scrapegraphai-1.5.0b3/scrapegraphai/models/openai_tts.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/nodes/__init__.py` & `scrapegraphai-1.5.0b3/scrapegraphai/nodes/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,9 +15,8 @@
 from .generate_scraper_node import GenerateScraperNode
 from .search_link_node import SearchLinkNode
 from .robots_node import RobotsNode
 from .generate_answer_csv_node import GenerateAnswerCSVNode
 from .generate_answer_pdf_node import GenerateAnswerPDFNode
 from .graph_iterator_node import GraphIteratorNode
 from .merge_answers_node import MergeAnswersNode
-from .generate_answer_omni_node import GenerateAnswerOmniNode
-from .knowledge_graph_node import KnowledgeGraphNode
+from .generate_answer_omni_node import GenerateAnswerOmniNode
```

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/nodes/base_node.py` & `scrapegraphai-1.5.0b3/scrapegraphai/nodes/base_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/nodes/blocks_identifier.py` & `scrapegraphai-1.5.0b3/scrapegraphai/nodes/parse_node.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,67 +1,86 @@
-""" 
-BlocksIndentifier Module
+"""
+ParseNode Module
 """
 
 from typing import List, Optional
 
-from langchain_community.document_loaders import AsyncChromiumLoader
-from langchain_core.documents import Document
-
+from langchain.text_splitter import RecursiveCharacterTextSplitter
+from langchain_community.document_transformers import Html2TextTransformer
+from ..utils.logging import get_logger
 from .base_node import BaseNode
 
 
-class BlocksIndentifier(BaseNode):
+class ParseNode(BaseNode):
     """
-    A node responsible to identify the blocks in the HTML content of a specified HTML content
-    e.g products in a E-commerce, flights in a travel website etc.
+    A node responsible for parsing HTML content from a document.
+    The parsed content is split into chunks for further processing.
+
+    This node enhances the scraping workflow by allowing for targeted extraction of
+    content, thereby optimizing the processing of large HTML documents.
 
     Attributes:
-        headless (bool): A flag indicating whether the browser should run in headless mode.
-        verbose (bool): A flag indicating whether to print verbose output during execution.
+        verbose (bool): A flag indicating whether to show print statements during execution.
 
     Args:
         input (str): Boolean expression defining the input keys needed from the state.
         output (List[str]): List of output keys to be updated in the state.
-        node_config (Optional[dict]): Additional configuration for the node.
-        node_name (str): The unique identifier name for the node, defaulting to "BlocksIndentifier".
+        node_config (dict): Additional configuration for the node.
+        node_name (str): The unique identifier name for the node, defaulting to "Parse".
     """
 
     def __init__(
         self,
         input: str,
         output: List[str],
-        node_config: Optional[dict],
-        node_name: str = "BlocksIndentifier",
+        node_config: Optional[dict] = None,
+        node_name: str = "Parse",
     ):
-        super().__init__(node_name, "node", input, output, 1)
+        super().__init__(node_name, "node", input, output, 1, node_config)
 
-        self.headless = (
-            True if node_config is None else node_config.get("headless", True)
-        )
         self.verbose = (
-            True if node_config is None else node_config.get("verbose", False)
+            False if node_config is None else node_config.get("verbose", False)
+        )
+        self.parse_html = (
+            True if node_config is None else node_config.get("parse_html", True)
         )
 
-    def execute(self, state):
+    def execute(self, state: dict) -> dict:
         """
-        Executes the node's logic, caracterized by a pre-processing of the HTML content and
-        subsequent identification of the blocks in the HTML content.
+        Executes the node's logic to parse the HTML document content and split it into chunks.
 
         Args:
-            state (dict): The current state of the graph. The input keys will be used
-                            to fetch the correct data types from the state.
+            state (dict): The current state of the graph. The input keys will be used to fetch the
+                            correct data from the state.
 
         Returns:
-            dict: The updated state with a new output key containing the fetched HTML content.
+            dict: The updated state with the output key containing the parsed content chunks.
 
         Raises:
-            KeyError: If the input key is not found in the state, indicating that the
-                    necessary information to perform the operation is missing.
+            KeyError: If the input keys are not found in the state, indicating that the
+                        necessary information for parsing the content is missing.
         """
+
         self.logger.info(f"--- Executing {self.node_name} Node ---")
 
         # Interpret input keys based on the provided input expression
         input_keys = self.get_input_keys(state)
 
         # Fetching data from the state based on the input keys
         input_data = [state[key] for key in input_keys]
+
+        text_splitter = RecursiveCharacterTextSplitter.from_tiktoken_encoder(
+            chunk_size=self.node_config.get("chunk_size", 4096),
+            chunk_overlap=0,
+        )
+
+        # Parse the document
+        docs_transformed = input_data[0]
+        if self.parse_html:
+            docs_transformed = Html2TextTransformer().transform_documents(input_data[0])
+        docs_transformed = docs_transformed[0]
+
+        chunks = text_splitter.split_text(docs_transformed.page_content)
+
+        state.update({self.output[0]: chunks})
+
+        return state
```

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/nodes/conditional_node.py` & `scrapegraphai-1.5.0b3/scrapegraphai/nodes/conditional_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/nodes/fetch_node.py` & `scrapegraphai-1.5.0b3/scrapegraphai/nodes/fetch_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/nodes/generate_answer_csv_node.py` & `scrapegraphai-1.5.0b3/scrapegraphai/nodes/generate_answer_csv_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/nodes/generate_answer_node.py` & `scrapegraphai-1.5.0b3/scrapegraphai/nodes/generate_answer_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/nodes/generate_answer_omni_node.py` & `scrapegraphai-1.5.0b3/scrapegraphai/nodes/generate_answer_omni_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/nodes/generate_answer_pdf_node.py` & `scrapegraphai-1.5.0b3/scrapegraphai/nodes/generate_answer_pdf_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/nodes/generate_scraper_node.py` & `scrapegraphai-1.5.0b3/scrapegraphai/nodes/generate_scraper_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/nodes/get_probable_tags_node.py` & `scrapegraphai-1.5.0b3/scrapegraphai/nodes/get_probable_tags_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/nodes/graph_iterator_node.py` & `scrapegraphai-1.5.0b3/scrapegraphai/nodes/graph_iterator_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/nodes/image_to_text_node.py` & `scrapegraphai-1.5.0b3/scrapegraphai/nodes/image_to_text_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/nodes/knowledge_graph_node.py` & `scrapegraphai-1.5.0b3/scrapegraphai/nodes/search_link_node.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,101 +1,120 @@
 """
-KnowledgeGraphNode Module
+SearchLinkNode Module
 """
 
 # Imports from standard library
 from typing import List, Optional
 from tqdm import tqdm
 
 # Imports from Langchain
 from langchain.prompts import PromptTemplate
 from langchain_core.output_parsers import JsonOutputParser
+from langchain_core.runnables import RunnableParallel
+
+from ..utils.logging import get_logger
 
 # Imports from the library
 from .base_node import BaseNode
-from ..utils import create_graph, create_interactive_graph
 
 
-class KnowledgeGraphNode(BaseNode):
+class SearchLinkNode(BaseNode):
     """
-    A node responsible for generating a knowledge graph from a dictionary.
+    A node that can filter out the relevant links in the webpage content for the user prompt.
+    Node expects the aleready scrapped links on the webpage and hence it is expected
+    that this node be used after the FetchNode.
 
     Attributes:
-        llm_model: An instance of a language model client, configured for generating answers.
+        llm_model: An instance of the language model client used for generating answers.
         verbose (bool): A flag indicating whether to show print statements during execution.
 
     Args:
         input (str): Boolean expression defining the input keys needed from the state.
         output (List[str]): List of output keys to be updated in the state.
         node_config (dict): Additional configuration for the node.
         node_name (str): The unique identifier name for the node, defaulting to "GenerateAnswer".
     """
 
-    def __init__(self, input: str, output: List[str], node_config: Optional[dict] = None,
-                 node_name: str = "KnowledgeGraph"):
-        super().__init__(node_name, "node", input, output, 2, node_config)
+    def __init__(
+        self,
+        input: str,
+        output: List[str],
+        node_config: Optional[dict] = None,
+        node_name: str = "GenerateLinks",
+    ):
+        super().__init__(node_name, "node", input, output, 1, node_config)
 
         self.llm_model = node_config["llm_model"]
-        self.verbose = False if node_config is None else node_config.get(
-            "verbose", False)
+        self.verbose = (
+            False if node_config is None else node_config.get("verbose", False)
+        )
 
     def execute(self, state: dict) -> dict:
         """
-        Executes the node's logic to create a knowledge graph from a dictionary.
+        Filter out relevant links from the webpage that are relavant to prompt. Out of the filtered links, also
+        ensure that all links are navigable.
 
         Args:
-            state (dict): The current state of the graph. The input keys will be used
-                            to fetch the correct data from the state.
+            state (dict): The current state of the graph. The input keys will be used to fetch the
+                            correct data types from the state.
 
         Returns:
-            dict: The updated state with the output key containing the generated answer.
+            dict: The updated state with the output key containing the list of links.
 
         Raises:
-            KeyError: If the input keys are not found in the state, indicating
-                      that the necessary information for generating an answer is missing.
+            KeyError: If the input keys are not found in the state, indicating that the
+                        necessary information for generating the answer is missing.
         """
 
-        if self.verbose:
-            print(f"--- Executing {self.node_name} Node ---")
+        self.logger.info(f"--- Executing {self.node_name} Node ---")
 
         # Interpret input keys based on the provided input expression
         input_keys = self.get_input_keys(state)
 
-        # Fetching data from the state based on the input keys
-        input_data = [state[key] for key in input_keys]
-
-        user_prompt = input_data[0]
-        answer_dict = input_data[1]
-
-        # Build the graph
-        graph = create_graph(answer_dict)
-        # Create the interactive graph
-        create_interactive_graph(graph, output_file='knowledge_graph.html')
-
-        # output_parser = JsonOutputParser()
-        # format_instructions = output_parser.get_format_instructions()
-
-        # template_merge = """
-        # You are a website scraper and you have just scraped some content from multiple websites.\n
-        # You are now asked to provide an answer to a USER PROMPT based on the content you have scraped.\n
-        # You need to merge the content from the different websites into a single answer without repetitions (if there are any). \n
-        # The scraped contents are in a JSON format and you need to merge them based on the context and providing a correct JSON structure.\n
-        # OUTPUT INSTRUCTIONS: {format_instructions}\n
-        # USER PROMPT: {user_prompt}\n
-        # WEBSITE CONTENT: {website_content}
-        # """
-
-        # prompt_template = PromptTemplate(
-        #     template=template_merge,
-        #     input_variables=["user_prompt"],
-        #     partial_variables={
-        #         "format_instructions": format_instructions,
-        #         "website_content": answers_str,
-        #     },
-        # )
-
-        # merge_chain = prompt_template | self.llm_model | output_parser
-        # answer = merge_chain.invoke({"user_prompt": user_prompt})
-
-        # Update the state with the generated answer
-        state.update({self.output[0]: graph})
+        user_prompt = state[input_keys[0]]
+        parsed_content_chunks = state[input_keys[1]]
+        output_parser = JsonOutputParser()
+
+        prompt_relevant_links = """
+            You are a website scraper and you have just scraped the following content from a website.
+            Content: {content}
+            
+            You are now tasked with identifying all hyper links within the content that are potentially
+            relevant to the user task: {user_prompt}
+            
+            Assume relevance broadly, including any links that might be related or potentially useful 
+            in relation to the task.
+            
+            Please list only valid URLs and make sure to err on the side of inclusion if it's uncertain 
+            whether the content at the link is directly relevant.
+
+            Output only a list of relevant links in the format:
+            [
+                "link1",
+                "link2",
+                "link3",
+                .
+                .
+                .
+            ]
+            """
+        relevant_links = []
+
+        for i, chunk in enumerate(
+            tqdm(
+                parsed_content_chunks,
+                desc="Processing chunks",
+                disable=not self.verbose,
+            )
+        ):
+            merge_prompt = PromptTemplate(
+                template=prompt_relevant_links,
+                input_variables=["content", "user_prompt"],
+            )
+            merge_chain = merge_prompt | self.llm_model | output_parser
+            # merge_chain = merge_prompt | self.llm_model
+            answer = merge_chain.invoke(
+                {"content": chunk.page_content, "user_prompt": user_prompt}
+            )
+            relevant_links += answer
+        state.update({self.output[0]: relevant_links})
         return state
```

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/nodes/merge_answers_node.py` & `scrapegraphai-1.5.0b3/scrapegraphai/nodes/merge_answers_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/nodes/rag_node.py` & `scrapegraphai-1.5.0b3/scrapegraphai/nodes/rag_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/nodes/robots_node.py` & `scrapegraphai-1.5.0b3/scrapegraphai/nodes/robots_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/nodes/search_internet_node.py` & `scrapegraphai-1.5.0b3/scrapegraphai/nodes/search_internet_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/nodes/search_node_with_context.py` & `scrapegraphai-1.5.0b3/scrapegraphai/nodes/search_node_with_context.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/nodes/text_to_speech_node.py` & `scrapegraphai-1.5.0b3/scrapegraphai/nodes/text_to_speech_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/utils/cleanup_html.py` & `scrapegraphai-1.5.0b3/scrapegraphai/utils/cleanup_html.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/utils/convert_to_csv.py` & `scrapegraphai-1.5.0b3/scrapegraphai/utils/convert_to_csv.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/utils/convert_to_json.py` & `scrapegraphai-1.5.0b3/scrapegraphai/utils/convert_to_json.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/utils/logging.py` & `scrapegraphai-1.5.0b3/scrapegraphai/utils/logging.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/utils/parse_state_keys.py` & `scrapegraphai-1.5.0b3/scrapegraphai/utils/parse_state_keys.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/utils/prettify_exec_info.py` & `scrapegraphai-1.5.0b3/scrapegraphai/utils/prettify_exec_info.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/utils/proxy_rotation.py` & `scrapegraphai-1.5.0b3/scrapegraphai/utils/proxy_rotation.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/utils/research_web.py` & `scrapegraphai-1.5.0b3/scrapegraphai/utils/research_web.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/utils/save_audio_from_bytes.py` & `scrapegraphai-1.5.0b3/scrapegraphai/utils/save_audio_from_bytes.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/utils/sys_dynamic_import.py` & `scrapegraphai-1.5.0b3/scrapegraphai/utils/sys_dynamic_import.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/scrapegraphai/utils/token_calculator.py` & `scrapegraphai-1.5.0b3/scrapegraphai/utils/token_calculator.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/tests/graphs/scrape_json_ollama.py` & `scrapegraphai-1.5.0b3/tests/graphs/scrape_json_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/tests/graphs/scrape_plain_text_llama3_test.py` & `scrapegraphai-1.5.0b3/tests/graphs/scrape_plain_text_llama3_test.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/tests/graphs/scrape_plain_text_mistral_test.py` & `scrapegraphai-1.5.0b3/tests/graphs/scrape_plain_text_mistral_test.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/tests/graphs/scrape_xml_ollama_test.py` & `scrapegraphai-1.5.0b3/tests/graphs/scrape_xml_ollama_test.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/tests/graphs/script_generator_test.py` & `scrapegraphai-1.5.0b3/tests/graphs/script_generator_test.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/tests/graphs/smart_scraper_ollama_test.py` & `scrapegraphai-1.5.0b3/tests/graphs/smart_scraper_ollama_test.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/tests/graphs/inputs/books.xml` & `scrapegraphai-1.5.0b3/tests/graphs/inputs/books.xml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/tests/graphs/inputs/example.json` & `scrapegraphai-1.5.0b3/tests/graphs/inputs/example.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/tests/graphs/inputs/plain_html_example.txt` & `scrapegraphai-1.5.0b3/tests/graphs/inputs/plain_html_example.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/tests/nodes/fetch_node_test.py` & `scrapegraphai-1.5.0b3/tests/nodes/fetch_node_test.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/tests/nodes/robot_node_test.py` & `scrapegraphai-1.5.0b3/tests/nodes/robot_node_test.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/tests/nodes/search_link_node_test.py` & `scrapegraphai-1.5.0b3/tests/nodes/search_link_node_test.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/tests/nodes/inputs/books.xml` & `scrapegraphai-1.5.0b3/tests/nodes/inputs/books.xml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/tests/nodes/inputs/example.json` & `scrapegraphai-1.5.0b3/tests/nodes/inputs/example.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/tests/nodes/inputs/plain_html_example.txt` & `scrapegraphai-1.5.0b3/tests/nodes/inputs/plain_html_example.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/tests/utils/test_proxy_rotation.py` & `scrapegraphai-1.5.0b3/tests/utils/test_proxy_rotation.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/tests/utils/test_sys_dynamic_import.py` & `scrapegraphai-1.5.0b3/tests/utils/test_sys_dynamic_import.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/LICENSE` & `scrapegraphai-1.5.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/README.md` & `scrapegraphai-1.5.0b3/README.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b2/pyproject.toml` & `scrapegraphai-1.5.0b3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "scrapegraphai"
 
 
-version = "1.5.0b2"
+version = "1.5.0b3"
 
 
 description = "A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines."
 authors = [
     { name = "Marco Vinciguerra", email = "mvincig11@gmail.com" },
     { name = "Marco Perini", email = "perinim.98@gmail.com" },
     { name = "Lorenzo Padoan", email = "lorenzo.padoan977@gmail.com" }
```

### Comparing `scrapegraphai-1.5.0b2/PKG-INFO` & `scrapegraphai-1.5.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: scrapegraphai
-Version: 1.5.0b2
+Version: 1.5.0b3
 Summary: A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines.
 Author-email: Marco Vinciguerra <mvincig11@gmail.com>, Marco Perini <perinim.98@gmail.com>, Lorenzo Padoan <lorenzo.padoan977@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: ai,artificial intelligence,gpt,graph,langchain,machine learning,natural language processing,nlp,openai,rag,scrapegraph,scrapegraphai,scraping,web scraping,web scraping library,web scraping tool,webscraping
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

