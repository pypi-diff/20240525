# Comparing `tmp/scrapegraphai-1.5.0b1.tar.gz` & `tmp/scrapegraphai-1.5.0b2.tar.gz`

## Comparing `scrapegraphai-1.5.0b1.tar` & `scrapegraphai-1.5.0b2.tar`

### file list

```diff
@@ -1,284 +1,285 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/.gitattributes
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/.releaserc.yml
--rw-r--r--   0        0        0    46284 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/CHANGELOG.md
--rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/CONTRIBUTING.md
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/Dockerfile
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/SECURITY.md
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/citation.cff
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/docker-compose.yml
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/readthedocs.yml
--rw-r--r--   0        0        0     7557 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/requirements-dev.lock
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/requirements-dev.txt
--rw-r--r--   0        0        0     7372 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/requirements.lock
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/requirements.txt
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/.github/ISSUE_TEMPLATE/custom.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/.github/workflows/codeql.yml
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/.github/workflows/dependency-review.yml
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/.github/workflows/pylint.yml
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/.github/workflows/release.yml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/docs/Makefile
--rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/docs/README.md
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/docs/make.bat
--rw-r--r--   0        0        0    60520 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/docs/assets/apikey_1.png
--rw-r--r--   0        0        0   123826 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/docs/assets/apikey_2.png
--rw-r--r--   0        0        0    60775 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/docs/assets/apikey_3.png
--rw-r--r--   0        0        0    86914 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/docs/assets/apikey_4.png
--rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/docs/assets/codespaces-badge.png
--rw-r--r--   0        0        0  1178826 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/docs/assets/logo_authors.png
--rw-r--r--   0        0        0    73949 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/docs/assets/omniscrapergraph.png
--rw-r--r--   0        0        0    58062 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/docs/assets/omnisearchgraph.png
--rw-r--r--   0        0        0    53007 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/docs/assets/project_overview_diagram.fig
--rw-r--r--   0        0        0    83949 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/docs/assets/project_overview_diagram.png
--rw-r--r--   0        0        0    33264 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/docs/assets/scrapegraphai_logo.png
--rw-r--r--   0        0        0    54611 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/docs/assets/searchgraph.png
--rw-r--r--   0        0        0    15508 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/docs/assets/serp_api_logo.png
--rw-r--r--   0        0        0    61095 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/docs/assets/smartscrapergraph.png
--rw-r--r--   0        0        0    49312 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/docs/assets/speechgraph.png
--rw-r--r--   0        0        0   221972 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/docs/assets/transparent_stat.png
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/docs/source/conf.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/docs/source/index.rst
--rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/docs/source/getting_started/examples.rst
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/docs/source/getting_started/installation.rst
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/docs/source/introduction/contributing.rst
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/docs/source/introduction/overview.rst
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/docs/source/modules/modules.rst
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/docs/source/modules/scrapegraphai.graphs.rst
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/docs/source/modules/scrapegraphai.nodes.rst
--rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/docs/source/modules/scrapegraphai.rst
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/docs/source/scrapers/benchmarks.rst
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/docs/source/scrapers/graph_config.rst
--rw-r--r--   0        0        0     5646 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/docs/source/scrapers/graphs.rst
--rw-r--r--   0        0        0     5568 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/docs/source/scrapers/llm.rst
--rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/readme.md
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/anthropic/smart_scraper_haiku.py
--rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/azure/json_scraper_azure.py
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/azure/search_graph_azure.py
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/azure/smart_scraper_azure_openai.py
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/azure/xml_scraper_azure.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/azure/inputs/books.xml
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/azure/inputs/example.json
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/azure/inputs/username.csv
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/bedrock/.env.example
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/bedrock/README.md
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/bedrock/csv_scraper_bedrock.py
--rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/bedrock/custom_graph_bedrock.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/bedrock/json_scraper_bedrock.py
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/bedrock/scrape_plain_text_bedrock.py
--rw-r--r--   0        0        0    82480 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/bedrock/scrapegraphai_bedrock.png
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/bedrock/script_generator_bedrock.py
--rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/bedrock/search_graph_bedrock.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/bedrock/smart_scraper_bedrock.py
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/bedrock/xml_scraper_bedrock.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/bedrock/inputs/books.xml
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/bedrock/inputs/example.json
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/bedrock/inputs/plain_html_example.txt
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/bedrock/inputs/username.csv
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/benchmarks/readme.md
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/benchmarks/GenerateScraper/.env.example
--rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/benchmarks/GenerateScraper/Readme.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/benchmarks/GenerateScraper/benchmark_docker.py
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/benchmarks/GenerateScraper/benchmark_groq.py
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/benchmarks/GenerateScraper/benchmark_llama3.py
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/benchmarks/GenerateScraper/benchmark_mistral.py
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/benchmarks/GenerateScraper/benchmark_openai_gpt35.py
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/benchmarks/GenerateScraper/benchmark_openai_gpt4.py
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/benchmarks/GenerateScraper/inputs/example_1.txt
--rw-r--r--   0        0        0  2590773 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/benchmarks/GenerateScraper/inputs/example_2.txt
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/benchmarks/SmartScraper/.env.example
--rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/benchmarks/SmartScraper/Readme.md
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/benchmarks/SmartScraper/benchmark_docker.py
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/benchmarks/SmartScraper/benchmark_groq.py
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/benchmarks/SmartScraper/benchmark_llama3.py
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/benchmarks/SmartScraper/benchmark_mistral.py
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/benchmarks/SmartScraper/benchmark_openai_gpt35.py
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/benchmarks/SmartScraper/benchmark_openai_gpt4.py
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/benchmarks/SmartScraper/inputs/example_1.txt
--rw-r--r--   0        0        0  2590773 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/benchmarks/SmartScraper/inputs/example_2.txt
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/deepseek/.env.example
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/deepseek/csv_scraper_deepseek.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/deepseek/json_scraper_deepseek.py
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/deepseek/script_generator_deepseek.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/deepseek/search_graph_deepseek.py
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/deepseek/smart_scarper_deepseek.py
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/deepseek/xml_scraper_deepseek.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/deepseek/inputs/books.xml
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/deepseek/inputs/example.json
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/deepseek/inputs/username.csv
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/gemini/.env.example
--rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/gemini/csv_scraper_gemini.py
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/gemini/custom_graph_gemini.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/gemini/json_scraper_gemini.py
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/gemini/readme.md
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/gemini/scrape_plain_text_gemini.py
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/gemini/scrape_xml_gemini.py
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/gemini/script_generator_gemini.py
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/gemini/search_graph_gemini.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/gemini/smart_scraper_gemini.py
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/gemini/xml_scraper_openai.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/gemini/inputs/books.xml
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/gemini/inputs/example.json
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/gemini/inputs/plain_html_example.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/gemini/inputs/username.csv
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/groq/.env.example
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/groq/search_graph_groq_openai.py
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/groq/smart_scraper_groq_ollama.py
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/groq/smart_scraper_groq_openai.py
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/huggingfacehub/smart_scraper_huggingfacehub.py
--rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/knowledge_graph/kg_custom_graph.py
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/knowledge_graph/load_vector.py
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/knowledge_graph/save_vector.py
--rw-r--r--   0        0        0    20332 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/knowledge_graph/input/job_postings.json
--rw-r--r--   0        0        0   399405 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/knowledge_graph/output/faiss_index/index.faiss
--rw-r--r--   0        0        0    14447 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/knowledge_graph/output/faiss_index/index.pkl
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/local_models/csv_scraper_ollama.py
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/local_models/json_scraper_ollama.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/local_models/scrape_plain_text_ollama.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/local_models/scrape_xml_ollama.py
--rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/local_models/script_generator_ollama.py
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/local_models/search_graph_ollama.py
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/local_models/smart_scraper_ollama.py
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/local_models/xml_scraper_ollama.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/local_models/inputs/books.xml
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/local_models/inputs/example.json
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/local_models/inputs/plain_html_example.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/local_models/inputs/username.csv
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/mixed_models/.env.example
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/mixed_models/readme.md
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/mixed_models/search_graph_groq_ollama.py
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/mixed_models/smart_scraper_mixed.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/mixed_models/inputs/books.xml
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/mixed_models/inputs/example.json
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/mixed_models/inputs/plain_html_example.txt
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/openai/.env.example
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/openai/csv_scraper_openai.py
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/openai/custom_graph_openai.py
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/openai/deep_scraper_openai.py
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/openai/json_scraper_openai.py
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/openai/omni_scraper_openai.py
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/openai/omni_search_graph_openai.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/openai/readme.md
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/openai/scrape_plain_text_openai.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/openai/script_generator_openai.py
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/openai/search_graph_openai.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/openai/smart_scraper_multi_openai.py
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/openai/smart_scraper_openai.py
--rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/openai/smart_scraper_schema_openai.py
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/openai/speech_graph_openai.py
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/openai/xml_scraper_openai.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/openai/inputs/books.xml
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/openai/inputs/example.json
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/openai/inputs/plain_html_example.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/openai/inputs/username.csv
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/single_node/fetch_node.py
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/single_node/image2text_node.py
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/single_node/kg_node.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/examples/single_node/robot_node.py
--rwxr-xr-x   0        0        0      986 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/manual deployment/commit_and_push.sh
--rwxr-xr-x   0        0        0      611 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/manual deployment/commit_and_push_with_tests.sh
--rwxr-xr-x   0        0        0      169 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/manual deployment/deploy_on_pip.sh
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/manual deployment/installation.sh
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/__init__.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/builders/__init__.py
--rw-r--r--   0        0        0     6653 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/builders/graph_builder.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/docloaders/__init__.py
--rw-r--r--   0        0        0     4649 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/docloaders/chromium.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/graphs/__init__.py
--rw-r--r--   0        0        0    14525 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/graphs/abstract_graph.py
--rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/graphs/base_graph.py
--rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/graphs/csv_scraper_graph.py
--rw-r--r--   0        0        0     5748 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/graphs/deep_scraper_graph.py
--rw-r--r--   0        0        0     3609 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/graphs/json_scraper_graph.py
--rw-r--r--   0        0        0     4501 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/graphs/omni_scraper_graph.py
--rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/graphs/omni_search_graph.py
--rw-r--r--   0        0        0     3754 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/graphs/pdf_scraper_graph.py
--rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/graphs/script_creator_graph.py
--rw-r--r--   0        0        0     3954 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/graphs/search_graph.py
--rw-r--r--   0        0        0     3868 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/graphs/smart_scraper_graph.py
--rw-r--r--   0        0        0     3733 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/graphs/smart_scraper_multi_graph.py
--rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/graphs/speech_graph.py
--rw-r--r--   0        0        0     3751 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/graphs/xml_scraper_graph.py
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/helpers/__init__.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/helpers/generate_answer_node_csv_prompts.py
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/helpers/generate_answer_node_omni_prompts.py
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/helpers/generate_answer_node_pdf_prompts.py
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/helpers/generate_answer_node_prompts.py
--rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/helpers/models_tokens.py
--rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/helpers/nodes_metadata.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/helpers/robots.py
--rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/helpers/schemas.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/models/__init__.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/models/anthropic.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/models/azure_openai.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/models/bedrock.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/models/deepseek.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/models/gemini.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/models/groq.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/models/hugging_face.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/models/ollama.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/models/openai.py
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/models/openai_itt.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/models/openai_tts.py
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/nodes/__init__.py
--rw-r--r--   0        0        0     8903 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/nodes/base_node.py
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/nodes/blocks_identifier.py
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/nodes/conditional_node.py
--rw-r--r--   0        0        0     6597 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/nodes/fetch_node.py
--rw-r--r--   0        0        0     5779 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/nodes/generate_answer_csv_node.py
--rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/nodes/generate_answer_node.py
--rw-r--r--   0        0        0     5301 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/nodes/generate_answer_omni_node.py
--rw-r--r--   0        0        0     5757 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/nodes/generate_answer_pdf_node.py
--rw-r--r--   0        0        0     4424 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/nodes/generate_scraper_node.py
--rw-r--r--   0        0        0     3757 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/nodes/get_probable_tags_node.py
--rw-r--r--   0        0        0     4603 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/nodes/graph_iterator_node.py
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/nodes/image_to_text_node.py
--rw-r--r--   0        0        0     3970 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/nodes/knowledge_graph_node.py
--rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/nodes/merge_answers_node.py
--rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/nodes/parse_node.py
--rw-r--r--   0        0        0     4565 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/nodes/rag_node.py
--rw-r--r--   0        0        0     6342 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/nodes/robots_node.py
--rw-r--r--   0        0        0     4218 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/nodes/search_internet_node.py
--rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/nodes/search_link_node.py
--rw-r--r--   0        0        0     4992 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/nodes/search_node_with_context.py
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/nodes/text_to_speech_node.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/utils/__init__.py
--rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/utils/cleanup_html.py
--rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/utils/convert_to_csv.py
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/utils/convert_to_json.py
--rw-r--r--   0        0        0     6364 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/utils/knowledge_graph.py
--rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/utils/logging.py
--rw-r--r--   0        0        0     4638 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/utils/parse_state_keys.py
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/utils/prettify_exec_info.py
--rw-r--r--   0        0        0     6404 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/utils/proxy_rotation.py
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/utils/research_web.py
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/utils/save_audio_from_bytes.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/utils/sys_dynamic_import.py
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/scrapegraphai/utils/token_calculator.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/tests/Readme.md
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/tests/graphs/scrape_json_ollama.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/tests/graphs/scrape_plain_text_llama3_test.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/tests/graphs/scrape_plain_text_mistral_test.py
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/tests/graphs/scrape_xml_ollama_test.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/tests/graphs/script_generator_test.py
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/tests/graphs/smart_scraper_ollama_test.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/tests/graphs/inputs/books.xml
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/tests/graphs/inputs/example.json
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/tests/graphs/inputs/plain_html_example.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/tests/graphs/inputs/username.csv
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/tests/nodes/fetch_node_test.py
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/tests/nodes/robot_node_test.py
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/tests/nodes/search_link_node_test.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/tests/nodes/inputs/books.xml
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/tests/nodes/inputs/example.json
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/tests/nodes/inputs/plain_html_example.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/tests/nodes/inputs/username.csv
--rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/tests/utils/test_proxy_rotation.py
--rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/tests/utils/test_sys_dynamic_import.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/LICENSE
--rw-r--r--   0        0        0     9182 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/README.md
--rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/pyproject.toml
--rw-r--r--   0        0        0    10804 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b1/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/.gitattributes
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/.releaserc.yml
+-rw-r--r--   0        0        0    46740 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/CHANGELOG.md
+-rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/CONTRIBUTING.md
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/Dockerfile
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/SECURITY.md
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/citation.cff
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docker-compose.yml
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/readthedocs.yml
+-rw-r--r--   0        0        0     7557 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/requirements-dev.lock
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/requirements-dev.txt
+-rw-r--r--   0        0        0     7372 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/requirements.lock
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/requirements.txt
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/.github/ISSUE_TEMPLATE/custom.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/.github/workflows/dependency-review.yml
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/.github/workflows/release.yml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/Makefile
+-rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/README.md
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/make.bat
+-rw-r--r--   0        0        0    60520 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/assets/apikey_1.png
+-rw-r--r--   0        0        0   123826 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/assets/apikey_2.png
+-rw-r--r--   0        0        0    60775 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/assets/apikey_3.png
+-rw-r--r--   0        0        0    86914 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/assets/apikey_4.png
+-rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/assets/codespaces-badge.png
+-rw-r--r--   0        0        0  1178826 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/assets/logo_authors.png
+-rw-r--r--   0        0        0    73949 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/assets/omniscrapergraph.png
+-rw-r--r--   0        0        0    58062 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/assets/omnisearchgraph.png
+-rw-r--r--   0        0        0    53007 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/assets/project_overview_diagram.fig
+-rw-r--r--   0        0        0    83949 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/assets/project_overview_diagram.png
+-rw-r--r--   0        0        0    33264 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/assets/scrapegraphai_logo.png
+-rw-r--r--   0        0        0    54611 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/assets/searchgraph.png
+-rw-r--r--   0        0        0    15508 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/assets/serp_api_logo.png
+-rw-r--r--   0        0        0    61095 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/assets/smartscrapergraph.png
+-rw-r--r--   0        0        0    49312 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/assets/speechgraph.png
+-rw-r--r--   0        0        0   221972 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/assets/transparent_stat.png
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/source/conf.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/source/index.rst
+-rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/source/getting_started/examples.rst
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/source/getting_started/installation.rst
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/source/introduction/contributing.rst
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/source/introduction/overview.rst
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/source/modules/modules.rst
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/source/modules/scrapegraphai.graphs.rst
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/source/modules/scrapegraphai.nodes.rst
+-rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/source/modules/scrapegraphai.rst
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/source/scrapers/benchmarks.rst
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/source/scrapers/graph_config.rst
+-rw-r--r--   0        0        0     5646 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/source/scrapers/graphs.rst
+-rw-r--r--   0        0        0     5568 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/docs/source/scrapers/llm.rst
+-rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/readme.md
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/anthropic/smart_scraper_haiku.py
+-rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/azure/json_scraper_azure.py
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/azure/search_graph_azure.py
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/azure/smart_scraper_azure_openai.py
+-rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/azure/xml_scraper_azure.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/azure/inputs/books.xml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/azure/inputs/example.json
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/azure/inputs/username.csv
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/bedrock/.env.example
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/bedrock/README.md
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/bedrock/csv_scraper_bedrock.py
+-rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/bedrock/custom_graph_bedrock.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/bedrock/json_scraper_bedrock.py
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/bedrock/scrape_plain_text_bedrock.py
+-rw-r--r--   0        0        0    82480 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/bedrock/scrapegraphai_bedrock.png
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/bedrock/script_generator_bedrock.py
+-rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/bedrock/search_graph_bedrock.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/bedrock/smart_scraper_bedrock.py
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/bedrock/xml_scraper_bedrock.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/bedrock/inputs/books.xml
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/bedrock/inputs/example.json
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/bedrock/inputs/plain_html_example.txt
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/bedrock/inputs/username.csv
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/benchmarks/readme.md
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/benchmarks/GenerateScraper/.env.example
+-rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/benchmarks/GenerateScraper/Readme.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/benchmarks/GenerateScraper/benchmark_docker.py
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/benchmarks/GenerateScraper/benchmark_groq.py
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/benchmarks/GenerateScraper/benchmark_llama3.py
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/benchmarks/GenerateScraper/benchmark_mistral.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/benchmarks/GenerateScraper/benchmark_openai_gpt35.py
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/benchmarks/GenerateScraper/benchmark_openai_gpt4.py
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/benchmarks/GenerateScraper/inputs/example_1.txt
+-rw-r--r--   0        0        0  2590773 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/benchmarks/GenerateScraper/inputs/example_2.txt
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/benchmarks/SmartScraper/.env.example
+-rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/benchmarks/SmartScraper/Readme.md
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/benchmarks/SmartScraper/benchmark_docker.py
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/benchmarks/SmartScraper/benchmark_groq.py
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/benchmarks/SmartScraper/benchmark_llama3.py
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/benchmarks/SmartScraper/benchmark_mistral.py
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/benchmarks/SmartScraper/benchmark_openai_gpt35.py
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/benchmarks/SmartScraper/benchmark_openai_gpt4.py
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/benchmarks/SmartScraper/inputs/example_1.txt
+-rw-r--r--   0        0        0  2590773 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/benchmarks/SmartScraper/inputs/example_2.txt
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/deepseek/.env.example
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/deepseek/csv_scraper_deepseek.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/deepseek/json_scraper_deepseek.py
+-rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/deepseek/script_generator_deepseek.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/deepseek/search_graph_deepseek.py
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/deepseek/smart_scarper_deepseek.py
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/deepseek/xml_scraper_deepseek.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/deepseek/inputs/books.xml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/deepseek/inputs/example.json
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/deepseek/inputs/username.csv
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/gemini/.env.example
+-rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/gemini/csv_scraper_gemini.py
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/gemini/custom_graph_gemini.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/gemini/json_scraper_gemini.py
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/gemini/readme.md
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/gemini/scrape_plain_text_gemini.py
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/gemini/scrape_xml_gemini.py
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/gemini/script_generator_gemini.py
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/gemini/search_graph_gemini.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/gemini/smart_scraper_gemini.py
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/gemini/xml_scraper_openai.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/gemini/inputs/books.xml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/gemini/inputs/example.json
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/gemini/inputs/plain_html_example.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/gemini/inputs/username.csv
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/groq/.env.example
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/groq/search_graph_groq_openai.py
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/groq/smart_scraper_groq_ollama.py
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/groq/smart_scraper_groq_openai.py
+-rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/huggingfacehub/smart_scraper_huggingfacehub.py
+-rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/knowledge_graph/kg_custom_graph.py
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/knowledge_graph/load_vector.py
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/knowledge_graph/save_vector.py
+-rw-r--r--   0        0        0    20332 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/knowledge_graph/input/job_postings.json
+-rw-r--r--   0        0        0   399405 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/knowledge_graph/output/faiss_index/index.faiss
+-rw-r--r--   0        0        0    14447 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/knowledge_graph/output/faiss_index/index.pkl
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/local_models/csv_scraper_ollama.py
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/local_models/json_scraper_ollama.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/local_models/scrape_plain_text_ollama.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/local_models/scrape_xml_ollama.py
+-rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/local_models/script_generator_ollama.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/local_models/search_graph_ollama.py
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/local_models/smart_scraper_ollama.py
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/local_models/xml_scraper_ollama.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/local_models/inputs/books.xml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/local_models/inputs/example.json
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/local_models/inputs/plain_html_example.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/local_models/inputs/username.csv
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/mixed_models/.env.example
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/mixed_models/readme.md
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/mixed_models/search_graph_groq_ollama.py
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/mixed_models/smart_scraper_mixed.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/mixed_models/inputs/books.xml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/mixed_models/inputs/example.json
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/mixed_models/inputs/plain_html_example.txt
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/openai/.env.example
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/openai/csv_scraper_openai.py
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/openai/custom_graph_openai.py
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/openai/deep_scraper_openai.py
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/openai/json_scraper_openai.py
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/openai/omni_scraper_openai.py
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/openai/omni_search_graph_openai.py
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/openai/pdf_scraper_openai.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/openai/readme.md
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/openai/scrape_plain_text_openai.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/openai/script_generator_openai.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/openai/search_graph_openai.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/openai/smart_scraper_multi_openai.py
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/openai/smart_scraper_openai.py
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/openai/smart_scraper_schema_openai.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/openai/speech_graph_openai.py
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/openai/xml_scraper_openai.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/openai/inputs/books.xml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/openai/inputs/example.json
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/openai/inputs/plain_html_example.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/openai/inputs/username.csv
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/single_node/fetch_node.py
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/single_node/image2text_node.py
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/single_node/kg_node.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/examples/single_node/robot_node.py
+-rwxr-xr-x   0        0        0      986 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/manual deployment/commit_and_push.sh
+-rwxr-xr-x   0        0        0      611 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/manual deployment/commit_and_push_with_tests.sh
+-rwxr-xr-x   0        0        0      169 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/manual deployment/deploy_on_pip.sh
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/manual deployment/installation.sh
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/__init__.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/builders/__init__.py
+-rw-r--r--   0        0        0     6653 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/builders/graph_builder.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/docloaders/__init__.py
+-rw-r--r--   0        0        0     4649 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/docloaders/chromium.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/graphs/__init__.py
+-rw-r--r--   0        0        0    14947 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/graphs/abstract_graph.py
+-rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/graphs/base_graph.py
+-rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/graphs/csv_scraper_graph.py
+-rw-r--r--   0        0        0     5748 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/graphs/deep_scraper_graph.py
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/graphs/json_scraper_graph.py
+-rw-r--r--   0        0        0     4501 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/graphs/omni_scraper_graph.py
+-rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/graphs/omni_search_graph.py
+-rw-r--r--   0        0        0     3397 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/graphs/pdf_scraper_graph.py
+-rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/graphs/script_creator_graph.py
+-rw-r--r--   0        0        0     3954 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/graphs/search_graph.py
+-rw-r--r--   0        0        0     3868 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/graphs/smart_scraper_graph.py
+-rw-r--r--   0        0        0     3733 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/graphs/smart_scraper_multi_graph.py
+-rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/graphs/speech_graph.py
+-rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/graphs/xml_scraper_graph.py
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/helpers/__init__.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/helpers/generate_answer_node_csv_prompts.py
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/helpers/generate_answer_node_omni_prompts.py
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/helpers/generate_answer_node_pdf_prompts.py
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/helpers/generate_answer_node_prompts.py
+-rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/helpers/models_tokens.py
+-rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/helpers/nodes_metadata.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/helpers/robots.py
+-rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/helpers/schemas.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/models/__init__.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/models/anthropic.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/models/azure_openai.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/models/bedrock.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/models/deepseek.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/models/gemini.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/models/groq.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/models/hugging_face.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/models/ollama.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/models/openai.py
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/models/openai_itt.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/models/openai_tts.py
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/nodes/__init__.py
+-rw-r--r--   0        0        0     8903 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/nodes/base_node.py
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/nodes/blocks_identifier.py
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/nodes/conditional_node.py
+-rw-r--r--   0        0        0     6553 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/nodes/fetch_node.py
+-rw-r--r--   0        0        0     5779 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/nodes/generate_answer_csv_node.py
+-rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/nodes/generate_answer_node.py
+-rw-r--r--   0        0        0     5301 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/nodes/generate_answer_omni_node.py
+-rw-r--r--   0        0        0     5757 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/nodes/generate_answer_pdf_node.py
+-rw-r--r--   0        0        0     4424 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/nodes/generate_scraper_node.py
+-rw-r--r--   0        0        0     3757 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/nodes/get_probable_tags_node.py
+-rw-r--r--   0        0        0     4603 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/nodes/graph_iterator_node.py
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/nodes/image_to_text_node.py
+-rw-r--r--   0        0        0     3970 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/nodes/knowledge_graph_node.py
+-rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/nodes/merge_answers_node.py
+-rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/nodes/parse_node.py
+-rw-r--r--   0        0        0     4565 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/nodes/rag_node.py
+-rw-r--r--   0        0        0     6342 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/nodes/robots_node.py
+-rw-r--r--   0        0        0     4218 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/nodes/search_internet_node.py
+-rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/nodes/search_link_node.py
+-rw-r--r--   0        0        0     4992 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/nodes/search_node_with_context.py
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/nodes/text_to_speech_node.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/utils/__init__.py
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/utils/cleanup_html.py
+-rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/utils/convert_to_csv.py
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/utils/convert_to_json.py
+-rw-r--r--   0        0        0     6364 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/utils/knowledge_graph.py
+-rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/utils/logging.py
+-rw-r--r--   0        0        0     4638 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/utils/parse_state_keys.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/utils/prettify_exec_info.py
+-rw-r--r--   0        0        0     6404 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/utils/proxy_rotation.py
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/utils/research_web.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/utils/save_audio_from_bytes.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/utils/sys_dynamic_import.py
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/scrapegraphai/utils/token_calculator.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/tests/Readme.md
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/tests/graphs/scrape_json_ollama.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/tests/graphs/scrape_plain_text_llama3_test.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/tests/graphs/scrape_plain_text_mistral_test.py
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/tests/graphs/scrape_xml_ollama_test.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/tests/graphs/script_generator_test.py
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/tests/graphs/smart_scraper_ollama_test.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/tests/graphs/inputs/books.xml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/tests/graphs/inputs/example.json
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/tests/graphs/inputs/plain_html_example.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/tests/graphs/inputs/username.csv
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/tests/nodes/fetch_node_test.py
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/tests/nodes/robot_node_test.py
+-rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/tests/nodes/search_link_node_test.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/tests/nodes/inputs/books.xml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/tests/nodes/inputs/example.json
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/tests/nodes/inputs/plain_html_example.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/tests/nodes/inputs/username.csv
+-rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/tests/utils/test_proxy_rotation.py
+-rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/tests/utils/test_sys_dynamic_import.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/LICENSE
+-rw-r--r--   0        0        0     9182 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/README.md
+-rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/pyproject.toml
+-rw-r--r--   0        0        0    10804 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b2/PKG-INFO
```

### Comparing `scrapegraphai-1.5.0b1/.releaserc.yml` & `scrapegraphai-1.5.0b2/.releaserc.yml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/CHANGELOG.md` & `scrapegraphai-1.5.0b2/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+## [1.5.0-beta.2](https://github.com/VinciGit00/Scrapegraph-ai/compare/v1.5.0-beta.1...v1.5.0-beta.2) (2024-05-24)
+
+
+### Bug Fixes
+
+* **pdf_scraper:** fix the pdf scraper gaph ([d00cde6](https://github.com/VinciGit00/Scrapegraph-ai/commit/d00cde60309935e283ba9116cf0b114e53cb9640))
+* **local_file:** fixed textual input pdf, csv, json and xml graph ([8d5eb0b](https://github.com/VinciGit00/Scrapegraph-ai/commit/8d5eb0bb0d5d008a63a96df94ce3842320376b8e))
+
 ## [1.5.0-beta.1](https://github.com/VinciGit00/Scrapegraph-ai/compare/v1.4.0...v1.5.0-beta.1) (2024-05-24)
 
 
 ### Features
 
 * **knowledgegraph:** add knowledge graph node ([0196423](https://github.com/VinciGit00/Scrapegraph-ai/commit/0196423bdeea6568086aae6db8fc0f5652fc4e87))
 * add logger integration ([e53766b](https://github.com/VinciGit00/Scrapegraph-ai/commit/e53766b16e89254f945f9b54b38445a24f8b81f2))
```

### Comparing `scrapegraphai-1.5.0b1/CODE_OF_CONDUCT.md` & `scrapegraphai-1.5.0b2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/CONTRIBUTING.md` & `scrapegraphai-1.5.0b2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/readthedocs.yml` & `scrapegraphai-1.5.0b2/readthedocs.yml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/requirements-dev.lock` & `scrapegraphai-1.5.0b2/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/requirements.lock` & `scrapegraphai-1.5.0b2/requirements.lock`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/.github/ISSUE_TEMPLATE/bug_report.md` & `scrapegraphai-1.5.0b2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/.github/ISSUE_TEMPLATE/feature_request.md` & `scrapegraphai-1.5.0b2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/.github/workflows/codeql.yml` & `scrapegraphai-1.5.0b2/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/.github/workflows/dependency-review.yml` & `scrapegraphai-1.5.0b2/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/.github/workflows/pylint.yml` & `scrapegraphai-1.5.0b2/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/.github/workflows/python-publish.yml` & `scrapegraphai-1.5.0b2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/.github/workflows/release.yml` & `scrapegraphai-1.5.0b2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/docs/Makefile` & `scrapegraphai-1.5.0b2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/docs/README.md` & `scrapegraphai-1.5.0b2/docs/README.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/docs/make.bat` & `scrapegraphai-1.5.0b2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/docs/assets/apikey_1.png` & `scrapegraphai-1.5.0b2/docs/assets/apikey_1.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/docs/assets/apikey_2.png` & `scrapegraphai-1.5.0b2/docs/assets/apikey_2.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/docs/assets/apikey_3.png` & `scrapegraphai-1.5.0b2/docs/assets/apikey_3.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/docs/assets/apikey_4.png` & `scrapegraphai-1.5.0b2/docs/assets/apikey_4.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/docs/assets/codespaces-badge.png` & `scrapegraphai-1.5.0b2/docs/assets/codespaces-badge.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/docs/assets/logo_authors.png` & `scrapegraphai-1.5.0b2/docs/assets/logo_authors.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/docs/assets/omniscrapergraph.png` & `scrapegraphai-1.5.0b2/docs/assets/omniscrapergraph.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/docs/assets/omnisearchgraph.png` & `scrapegraphai-1.5.0b2/docs/assets/omnisearchgraph.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/docs/assets/project_overview_diagram.fig` & `scrapegraphai-1.5.0b2/docs/assets/project_overview_diagram.fig`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/docs/assets/project_overview_diagram.png` & `scrapegraphai-1.5.0b2/docs/assets/project_overview_diagram.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/docs/assets/scrapegraphai_logo.png` & `scrapegraphai-1.5.0b2/docs/assets/scrapegraphai_logo.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/docs/assets/searchgraph.png` & `scrapegraphai-1.5.0b2/docs/assets/searchgraph.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/docs/assets/serp_api_logo.png` & `scrapegraphai-1.5.0b2/docs/assets/serp_api_logo.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/docs/assets/smartscrapergraph.png` & `scrapegraphai-1.5.0b2/docs/assets/smartscrapergraph.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/docs/assets/speechgraph.png` & `scrapegraphai-1.5.0b2/docs/assets/speechgraph.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/docs/assets/transparent_stat.png` & `scrapegraphai-1.5.0b2/docs/assets/transparent_stat.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/docs/source/conf.py` & `scrapegraphai-1.5.0b2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/docs/source/index.rst` & `scrapegraphai-1.5.0b2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/docs/source/getting_started/examples.rst` & `scrapegraphai-1.5.0b2/docs/source/getting_started/examples.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/docs/source/getting_started/installation.rst` & `scrapegraphai-1.5.0b2/docs/source/getting_started/installation.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/docs/source/introduction/contributing.rst` & `scrapegraphai-1.5.0b2/docs/source/introduction/contributing.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/docs/source/introduction/overview.rst` & `scrapegraphai-1.5.0b2/docs/source/introduction/overview.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/docs/source/modules/scrapegraphai.graphs.rst` & `scrapegraphai-1.5.0b2/docs/source/modules/scrapegraphai.graphs.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/docs/source/modules/scrapegraphai.nodes.rst` & `scrapegraphai-1.5.0b2/docs/source/modules/scrapegraphai.nodes.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/docs/source/modules/scrapegraphai.rst` & `scrapegraphai-1.5.0b2/docs/source/modules/scrapegraphai.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/docs/source/scrapers/benchmarks.rst` & `scrapegraphai-1.5.0b2/docs/source/scrapers/benchmarks.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/docs/source/scrapers/graph_config.rst` & `scrapegraphai-1.5.0b2/docs/source/scrapers/graph_config.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/docs/source/scrapers/graphs.rst` & `scrapegraphai-1.5.0b2/docs/source/scrapers/graphs.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/docs/source/scrapers/llm.rst` & `scrapegraphai-1.5.0b2/docs/source/scrapers/llm.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/readme.md` & `scrapegraphai-1.5.0b2/examples/readme.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/anthropic/smart_scraper_haiku.py` & `scrapegraphai-1.5.0b2/examples/anthropic/smart_scraper_haiku.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/azure/json_scraper_azure.py` & `scrapegraphai-1.5.0b2/examples/azure/json_scraper_azure.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/azure/search_graph_azure.py` & `scrapegraphai-1.5.0b2/examples/azure/search_graph_azure.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/azure/smart_scraper_azure_openai.py` & `scrapegraphai-1.5.0b2/examples/azure/smart_scraper_azure_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/azure/xml_scraper_azure.py` & `scrapegraphai-1.5.0b2/examples/azure/xml_scraper_azure.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/azure/inputs/books.xml` & `scrapegraphai-1.5.0b2/examples/azure/inputs/books.xml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/azure/inputs/example.json` & `scrapegraphai-1.5.0b2/examples/azure/inputs/example.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/bedrock/csv_scraper_bedrock.py` & `scrapegraphai-1.5.0b2/examples/bedrock/csv_scraper_bedrock.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/bedrock/custom_graph_bedrock.py` & `scrapegraphai-1.5.0b2/examples/bedrock/custom_graph_bedrock.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/bedrock/json_scraper_bedrock.py` & `scrapegraphai-1.5.0b2/examples/bedrock/json_scraper_bedrock.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/bedrock/scrape_plain_text_bedrock.py` & `scrapegraphai-1.5.0b2/examples/bedrock/scrape_plain_text_bedrock.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/bedrock/scrapegraphai_bedrock.png` & `scrapegraphai-1.5.0b2/examples/bedrock/scrapegraphai_bedrock.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/bedrock/script_generator_bedrock.py` & `scrapegraphai-1.5.0b2/examples/bedrock/script_generator_bedrock.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/bedrock/search_graph_bedrock.py` & `scrapegraphai-1.5.0b2/examples/bedrock/search_graph_bedrock.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/bedrock/smart_scraper_bedrock.py` & `scrapegraphai-1.5.0b2/examples/bedrock/smart_scraper_bedrock.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/bedrock/xml_scraper_bedrock.py` & `scrapegraphai-1.5.0b2/examples/bedrock/xml_scraper_bedrock.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/bedrock/inputs/books.xml` & `scrapegraphai-1.5.0b2/examples/bedrock/inputs/books.xml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/bedrock/inputs/example.json` & `scrapegraphai-1.5.0b2/examples/bedrock/inputs/example.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/bedrock/inputs/plain_html_example.txt` & `scrapegraphai-1.5.0b2/examples/bedrock/inputs/plain_html_example.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/benchmarks/GenerateScraper/Readme.md` & `scrapegraphai-1.5.0b2/examples/benchmarks/GenerateScraper/Readme.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/benchmarks/GenerateScraper/benchmark_groq.py` & `scrapegraphai-1.5.0b2/examples/benchmarks/GenerateScraper/benchmark_groq.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/benchmarks/GenerateScraper/benchmark_llama3.py` & `scrapegraphai-1.5.0b2/examples/benchmarks/GenerateScraper/benchmark_llama3.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/benchmarks/GenerateScraper/benchmark_mistral.py` & `scrapegraphai-1.5.0b2/examples/benchmarks/GenerateScraper/benchmark_mistral.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/benchmarks/GenerateScraper/benchmark_openai_gpt35.py` & `scrapegraphai-1.5.0b2/examples/benchmarks/GenerateScraper/benchmark_openai_gpt35.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/benchmarks/GenerateScraper/benchmark_openai_gpt4.py` & `scrapegraphai-1.5.0b2/examples/benchmarks/GenerateScraper/benchmark_openai_gpt4.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/benchmarks/GenerateScraper/inputs/example_1.txt` & `scrapegraphai-1.5.0b2/examples/benchmarks/GenerateScraper/inputs/example_1.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/benchmarks/GenerateScraper/inputs/example_2.txt` & `scrapegraphai-1.5.0b2/examples/benchmarks/GenerateScraper/inputs/example_2.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/benchmarks/SmartScraper/Readme.md` & `scrapegraphai-1.5.0b2/examples/benchmarks/SmartScraper/Readme.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/benchmarks/SmartScraper/benchmark_docker.py` & `scrapegraphai-1.5.0b2/examples/benchmarks/SmartScraper/benchmark_docker.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/benchmarks/SmartScraper/benchmark_groq.py` & `scrapegraphai-1.5.0b2/examples/benchmarks/SmartScraper/benchmark_groq.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/benchmarks/SmartScraper/benchmark_llama3.py` & `scrapegraphai-1.5.0b2/examples/benchmarks/SmartScraper/benchmark_llama3.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/benchmarks/SmartScraper/benchmark_mistral.py` & `scrapegraphai-1.5.0b2/examples/benchmarks/SmartScraper/benchmark_mistral.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/benchmarks/SmartScraper/benchmark_openai_gpt35.py` & `scrapegraphai-1.5.0b2/examples/benchmarks/SmartScraper/benchmark_openai_gpt35.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/benchmarks/SmartScraper/benchmark_openai_gpt4.py` & `scrapegraphai-1.5.0b2/examples/benchmarks/SmartScraper/benchmark_openai_gpt4.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/benchmarks/SmartScraper/inputs/example_1.txt` & `scrapegraphai-1.5.0b2/examples/benchmarks/SmartScraper/inputs/example_1.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/benchmarks/SmartScraper/inputs/example_2.txt` & `scrapegraphai-1.5.0b2/examples/benchmarks/SmartScraper/inputs/example_2.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/deepseek/csv_scraper_deepseek.py` & `scrapegraphai-1.5.0b2/examples/deepseek/csv_scraper_deepseek.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/deepseek/json_scraper_deepseek.py` & `scrapegraphai-1.5.0b2/examples/deepseek/json_scraper_deepseek.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/deepseek/script_generator_deepseek.py` & `scrapegraphai-1.5.0b2/examples/deepseek/script_generator_deepseek.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/deepseek/search_graph_deepseek.py` & `scrapegraphai-1.5.0b2/examples/deepseek/search_graph_deepseek.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/deepseek/smart_scarper_deepseek.py` & `scrapegraphai-1.5.0b2/examples/deepseek/smart_scarper_deepseek.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/deepseek/xml_scraper_deepseek.py` & `scrapegraphai-1.5.0b2/examples/deepseek/xml_scraper_deepseek.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/deepseek/inputs/books.xml` & `scrapegraphai-1.5.0b2/examples/deepseek/inputs/books.xml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/deepseek/inputs/example.json` & `scrapegraphai-1.5.0b2/examples/deepseek/inputs/example.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/gemini/csv_scraper_gemini.py` & `scrapegraphai-1.5.0b2/examples/gemini/csv_scraper_gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/gemini/custom_graph_gemini.py` & `scrapegraphai-1.5.0b2/examples/gemini/custom_graph_gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/gemini/json_scraper_gemini.py` & `scrapegraphai-1.5.0b2/examples/gemini/json_scraper_gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/gemini/scrape_plain_text_gemini.py` & `scrapegraphai-1.5.0b2/examples/gemini/scrape_plain_text_gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/gemini/scrape_xml_gemini.py` & `scrapegraphai-1.5.0b2/examples/gemini/scrape_xml_gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/gemini/script_generator_gemini.py` & `scrapegraphai-1.5.0b2/examples/gemini/script_generator_gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/gemini/search_graph_gemini.py` & `scrapegraphai-1.5.0b2/examples/gemini/search_graph_gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/gemini/smart_scraper_gemini.py` & `scrapegraphai-1.5.0b2/examples/gemini/smart_scraper_gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/gemini/xml_scraper_openai.py` & `scrapegraphai-1.5.0b2/examples/gemini/xml_scraper_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/gemini/inputs/books.xml` & `scrapegraphai-1.5.0b2/examples/gemini/inputs/books.xml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/gemini/inputs/example.json` & `scrapegraphai-1.5.0b2/examples/gemini/inputs/example.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/gemini/inputs/plain_html_example.txt` & `scrapegraphai-1.5.0b2/examples/gemini/inputs/plain_html_example.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/groq/search_graph_groq_openai.py` & `scrapegraphai-1.5.0b2/examples/groq/search_graph_groq_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/groq/smart_scraper_groq_ollama.py` & `scrapegraphai-1.5.0b2/examples/groq/smart_scraper_groq_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/groq/smart_scraper_groq_openai.py` & `scrapegraphai-1.5.0b2/examples/groq/smart_scraper_groq_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/huggingfacehub/smart_scraper_huggingfacehub.py` & `scrapegraphai-1.5.0b2/examples/huggingfacehub/smart_scraper_huggingfacehub.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/knowledge_graph/kg_custom_graph.py` & `scrapegraphai-1.5.0b2/examples/knowledge_graph/kg_custom_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/knowledge_graph/load_vector.py` & `scrapegraphai-1.5.0b2/examples/knowledge_graph/load_vector.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/knowledge_graph/save_vector.py` & `scrapegraphai-1.5.0b2/examples/knowledge_graph/save_vector.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/knowledge_graph/input/job_postings.json` & `scrapegraphai-1.5.0b2/examples/knowledge_graph/input/job_postings.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/knowledge_graph/output/faiss_index/index.faiss` & `scrapegraphai-1.5.0b2/examples/knowledge_graph/output/faiss_index/index.faiss`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/knowledge_graph/output/faiss_index/index.pkl` & `scrapegraphai-1.5.0b2/examples/knowledge_graph/output/faiss_index/index.pkl`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/local_models/csv_scraper_ollama.py` & `scrapegraphai-1.5.0b2/examples/local_models/csv_scraper_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/local_models/json_scraper_ollama.py` & `scrapegraphai-1.5.0b2/examples/local_models/json_scraper_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/local_models/scrape_plain_text_ollama.py` & `scrapegraphai-1.5.0b2/examples/local_models/scrape_plain_text_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/local_models/scrape_xml_ollama.py` & `scrapegraphai-1.5.0b2/examples/local_models/scrape_xml_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/local_models/script_generator_ollama.py` & `scrapegraphai-1.5.0b2/examples/local_models/script_generator_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/local_models/search_graph_ollama.py` & `scrapegraphai-1.5.0b2/examples/local_models/search_graph_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/local_models/smart_scraper_ollama.py` & `scrapegraphai-1.5.0b2/examples/local_models/smart_scraper_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/local_models/xml_scraper_ollama.py` & `scrapegraphai-1.5.0b2/examples/local_models/xml_scraper_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/local_models/inputs/books.xml` & `scrapegraphai-1.5.0b2/examples/local_models/inputs/books.xml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/local_models/inputs/example.json` & `scrapegraphai-1.5.0b2/examples/local_models/inputs/example.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/local_models/inputs/plain_html_example.txt` & `scrapegraphai-1.5.0b2/examples/local_models/inputs/plain_html_example.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/mixed_models/search_graph_groq_ollama.py` & `scrapegraphai-1.5.0b2/examples/mixed_models/search_graph_groq_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/mixed_models/smart_scraper_mixed.py` & `scrapegraphai-1.5.0b2/examples/mixed_models/smart_scraper_mixed.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/mixed_models/inputs/books.xml` & `scrapegraphai-1.5.0b2/examples/mixed_models/inputs/books.xml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/mixed_models/inputs/example.json` & `scrapegraphai-1.5.0b2/examples/mixed_models/inputs/example.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/mixed_models/inputs/plain_html_example.txt` & `scrapegraphai-1.5.0b2/examples/mixed_models/inputs/plain_html_example.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/openai/csv_scraper_openai.py` & `scrapegraphai-1.5.0b2/examples/openai/csv_scraper_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/openai/custom_graph_openai.py` & `scrapegraphai-1.5.0b2/examples/openai/custom_graph_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/openai/deep_scraper_openai.py` & `scrapegraphai-1.5.0b2/examples/openai/deep_scraper_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/openai/json_scraper_openai.py` & `scrapegraphai-1.5.0b2/examples/openai/json_scraper_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/openai/omni_scraper_openai.py` & `scrapegraphai-1.5.0b2/examples/openai/omni_scraper_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/openai/omni_search_graph_openai.py` & `scrapegraphai-1.5.0b2/examples/openai/omni_search_graph_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/openai/scrape_plain_text_openai.py` & `scrapegraphai-1.5.0b2/examples/openai/scrape_plain_text_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/openai/script_generator_openai.py` & `scrapegraphai-1.5.0b2/examples/openai/script_generator_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/openai/search_graph_openai.py` & `scrapegraphai-1.5.0b2/examples/openai/search_graph_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/openai/smart_scraper_multi_openai.py` & `scrapegraphai-1.5.0b2/examples/openai/smart_scraper_multi_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/openai/smart_scraper_openai.py` & `scrapegraphai-1.5.0b2/examples/openai/smart_scraper_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/openai/smart_scraper_schema_openai.py` & `scrapegraphai-1.5.0b2/examples/openai/smart_scraper_schema_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/openai/speech_graph_openai.py` & `scrapegraphai-1.5.0b2/examples/openai/speech_graph_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/openai/xml_scraper_openai.py` & `scrapegraphai-1.5.0b2/examples/openai/xml_scraper_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/openai/inputs/books.xml` & `scrapegraphai-1.5.0b2/examples/openai/inputs/books.xml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/openai/inputs/example.json` & `scrapegraphai-1.5.0b2/examples/openai/inputs/example.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/openai/inputs/plain_html_example.txt` & `scrapegraphai-1.5.0b2/examples/openai/inputs/plain_html_example.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/single_node/fetch_node.py` & `scrapegraphai-1.5.0b2/examples/single_node/fetch_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/single_node/image2text_node.py` & `scrapegraphai-1.5.0b2/examples/single_node/image2text_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/single_node/kg_node.py` & `scrapegraphai-1.5.0b2/examples/single_node/kg_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/examples/single_node/robot_node.py` & `scrapegraphai-1.5.0b2/examples/single_node/robot_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/manual deployment/commit_and_push.sh` & `scrapegraphai-1.5.0b2/manual deployment/commit_and_push.sh`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/manual deployment/commit_and_push_with_tests.sh` & `scrapegraphai-1.5.0b2/manual deployment/commit_and_push_with_tests.sh`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/builders/graph_builder.py` & `scrapegraphai-1.5.0b2/scrapegraphai/builders/graph_builder.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/docloaders/chromium.py` & `scrapegraphai-1.5.0b2/scrapegraphai/docloaders/chromium.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/graphs/__init__.py` & `scrapegraphai-1.5.0b2/scrapegraphai/graphs/__init__.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/graphs/abstract_graph.py` & `scrapegraphai-1.5.0b2/scrapegraphai/graphs/abstract_graph.py`

 * *Files 4% similar despite different names*

```diff
@@ -192,60 +192,69 @@
             try:
                 if "model_tokens" in llm_params:
                     self.model_token = llm_params["model_tokens"]
                 elif llm_params["model"] in models_tokens["ollama"]:
                     try:
                         self.model_token = models_tokens["ollama"][llm_params["model"]]
                     except KeyError as exc:
+                        print("model not found, using default token size (8192)")
                         self.model_token = 8192
                 else:
                     self.model_token = 8192
             except AttributeError:
                 self.model_token = 8192
 
             return Ollama(llm_params)
         elif "hugging_face" in llm_params["model"]:
             try:
                 self.model_token = models_tokens["hugging_face"][llm_params["model"]]
-            except KeyError as exc:
-                raise KeyError("Model not supported") from exc
+            except KeyError:
+                print("model not found, using default token size (8192)")
+                self.model_token = 8192
             return HuggingFace(llm_params)
         elif "groq" in llm_params["model"]:
             llm_params["model"] = llm_params["model"].split("/")[-1]
 
             try:
                 self.model_token = models_tokens["groq"][llm_params["model"]]
-            except KeyError as exc:
-                raise KeyError("Model not supported") from exc
+            except KeyError:
+                print("model not found, using default token size (8192)")
+                self.model_token = 8192
             return Groq(llm_params)
         elif "bedrock" in llm_params["model"]:
             llm_params["model"] = llm_params["model"].split("/")[-1]
             model_id = llm_params["model"]
             client = llm_params.get("client", None)
             try:
                 self.model_token = models_tokens["bedrock"][llm_params["model"]]
-            except KeyError as exc:
-                raise KeyError("Model not supported") from exc
+            except KeyError:
+                print("model not found, using default token size (8192)")
+                self.model_token = 8192
             return Bedrock(
                 {
                     "client": client,
                     "model_id": model_id,
                     "model_kwargs": {
                         "temperature": llm_params["temperature"],
                     },
                 }
             )
         elif "claude-3-" in llm_params["model"]:
-            self.model_token = models_tokens["claude"]["claude3"]
+            try:
+                self.model_token = models_tokens["claude"]["claude3"]
+            except KeyError:
+                print("model not found, using default token size (8192)")
+                self.model_token = 8192
             return Anthropic(llm_params)
         elif "deepseek" in llm_params["model"]:
             try:
                 self.model_token = models_tokens["deepseek"][llm_params["model"]]
-            except KeyError as exc:
-                raise KeyError("Model not supported") from exc
+            except KeyError:
+                print("model not found, using default token size (8192)")
+                self.model_token = 8192
             return DeepSeek(llm_params)
         else:
             raise ValueError("Model provided by the configuration not supported")
 
     def _create_default_embedder(self, llm_config=None) -> object:
         """
         Create an embedding model instance based on the chosen llm model.
```

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/graphs/base_graph.py` & `scrapegraphai-1.5.0b2/scrapegraphai/graphs/base_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/graphs/csv_scraper_graph.py` & `scrapegraphai-1.5.0b2/scrapegraphai/graphs/csv_scraper_graph.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from typing import Optional
 
 from .base_graph import BaseGraph
 from .abstract_graph import AbstractGraph
 
 from ..nodes import (
     FetchNode,
-    ParseNode,
     RAGNode,
     GenerateAnswerCSVNode
 )
 
 
 class CSVScraperGraph(AbstractGraph):
     """
@@ -31,50 +30,41 @@
 
     def _create_graph(self):
         """
         Creates the graph of nodes representing the workflow for web scraping.
         """
         fetch_node = FetchNode(
             input="csv | csv_dir",
-            output=["doc", "link_urls", "img_urls"],
-        )
-        parse_node = ParseNode(
-            input="doc",
-            output=["parsed_doc"],
-            node_config={
-                "chunk_size": self.model_token,
-            }
+            output=["doc"],
         )
         rag_node = RAGNode(
-            input="user_prompt & (parsed_doc | doc)",
+            input="user_prompt & doc",
             output=["relevant_chunks"],
             node_config={
                 "llm_model": self.llm_model,
                 "embedder_model": self.embedder_model,
             }
         )
         generate_answer_node = GenerateAnswerCSVNode(
-            input="user_prompt & (relevant_chunks | parsed_doc | doc)",
+            input="user_prompt & (relevant_chunks | doc)",
             output=["answer"],
             node_config={
                 "llm_model": self.llm_model,
                 "schema": self.schema,
             }
         )
 
         return BaseGraph(
             nodes=[
                 fetch_node,
-                parse_node,
                 rag_node,
                 generate_answer_node,
             ],
             edges=[
-                (fetch_node, parse_node),
-                (parse_node, rag_node),
+                (fetch_node, rag_node),
                 (rag_node, generate_answer_node)
             ],
             entry_point=fetch_node
         )
 
     def run(self) -> str:
         """
```

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/graphs/deep_scraper_graph.py` & `scrapegraphai-1.5.0b2/scrapegraphai/graphs/deep_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/graphs/json_scraper_graph.py` & `scrapegraphai-1.5.0b2/scrapegraphai/graphs/json_scraper_graph.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from typing import Optional
 
 from .base_graph import BaseGraph
 from .abstract_graph import AbstractGraph
 
 from ..nodes import (
     FetchNode,
-    ParseNode,
     RAGNode,
     GenerateAnswerNode
 )
 
 
 class JSONScraperGraph(AbstractGraph):
     """
@@ -58,21 +57,14 @@
             BaseGraph: A graph instance representing the web scraping workflow.
         """
 
         fetch_node = FetchNode(
             input="json | json_dir",
             output=["doc", "link_urls", "img_urls"],
         )
-        parse_node = ParseNode(
-            input="doc",
-            output=["parsed_doc"],
-            node_config={
-                "chunk_size": self.model_token
-            }
-        )
         rag_node = RAGNode(
             input="user_prompt & (parsed_doc | doc)",
             output=["relevant_chunks"],
             node_config={
                 "llm_model": self.llm_model,
                 "embedder_model": self.embedder_model
             }
@@ -85,21 +77,19 @@
                 "schema": self.schema
             }
         )
 
         return BaseGraph(
             nodes=[
                 fetch_node,
-                parse_node,
                 rag_node,
                 generate_answer_node,
             ],
             edges=[
-                (fetch_node, parse_node),
-                (parse_node, rag_node),
+                (fetch_node, rag_node),
                 (rag_node, generate_answer_node)
             ],
             entry_point=fetch_node
         )
 
     def run(self) -> str:
         """
```

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/graphs/omni_scraper_graph.py` & `scrapegraphai-1.5.0b2/scrapegraphai/graphs/omni_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/graphs/omni_search_graph.py` & `scrapegraphai-1.5.0b2/scrapegraphai/graphs/omni_search_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/graphs/pdf_scraper_graph.py` & `scrapegraphai-1.5.0b2/scrapegraphai/graphs/smart_scraper_graph.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-PDFScraperGraph Module
+SmartScraperGraph Module
 """
 
 from typing import Optional
 
 from .base_graph import BaseGraph
 from .abstract_graph import AbstractGraph
 
@@ -11,76 +11,79 @@
     FetchNode,
     ParseNode,
     RAGNode,
     GenerateAnswerNode
 )
 
 
-class PDFScraperGraph(AbstractGraph):
+class SmartScraperGraph(AbstractGraph):
     """
-    PDFScraperGraph is a scraping pipeline that extracts information from pdf files using a natural
-    language model to interpret and answer prompts.
+    SmartScraper is a scraping pipeline that automates the process of 
+    extracting information from web pages
+    using a natural language model to interpret and answer prompts.
 
     Attributes:
         prompt (str): The prompt for the graph.
         source (str): The source of the graph.
         config (dict): Configuration parameters for the graph.
         schema (str): The schema for the graph output.
         llm_model: An instance of a language model client, configured for generating answers.
         embedder_model: An instance of an embedding model client, 
         configured for generating embeddings.
         verbose (bool): A flag indicating whether to show print statements during execution.
         headless (bool): A flag indicating whether to run the graph in headless mode.
-        model_token (int): The token limit for the language model.
 
     Args:
         prompt (str): The prompt for the graph.
         source (str): The source of the graph.
         config (dict): Configuration parameters for the graph.
         schema (str): The schema for the graph output.
 
     Example:
-        >>> pdf_scraper = PDFScraperGraph(
+        >>> smart_scraper = SmartScraperGraph(
         ...     "List me all the attractions in Chioggia.",
-        ...     "data/chioggia.pdf",
+        ...     "https://en.wikipedia.org/wiki/Chioggia",
         ...     {"llm": {"model": "gpt-3.5-turbo"}}
         ... )
-        >>> result = pdf_scraper.run()
+        >>> result = smart_scraper.run()
+        )
     """
 
     def __init__(self, prompt: str, source: str, config: dict, schema: Optional[str] = None):
         super().__init__(prompt, config, source, schema)
 
-        self.input_key = "pdf" if source.endswith("pdf") else "pdf_dir"
+        self.input_key = "url" if source.startswith("http") else "local_dir"
 
     def _create_graph(self) -> BaseGraph:
         """
         Creates the graph of nodes representing the workflow for web scraping.
 
         Returns:
             BaseGraph: A graph instance representing the web scraping workflow.
         """
-
         fetch_node = FetchNode(
-            input='pdf | pdf_dir',
+            input="url | local_dir",
             output=["doc", "link_urls", "img_urls"],
+            node_config={
+                "loader_kwargs": self.config.get("loader_kwargs", {}),
+            }
         )
         parse_node = ParseNode(
             input="doc",
             output=["parsed_doc"],
             node_config={
-                "chunk_size": self.model_token,
+                "chunk_size": self.model_token
             }
         )
         rag_node = RAGNode(
             input="user_prompt & (parsed_doc | doc)",
             output=["relevant_chunks"],
             node_config={
                 "llm_model": self.llm_model,
-                "embedder_model": self.embedder_model,
+                "embedder_model": self.embedder_model
             }
         )
         generate_answer_node = GenerateAnswerNode(
             input="user_prompt & (relevant_chunks | parsed_doc | doc)",
             output=["answer"],
             node_config={
                 "llm_model": self.llm_model,
@@ -101,15 +104,15 @@
                 (rag_node, generate_answer_node)
             ],
             entry_point=fetch_node
         )
 
     def run(self) -> str:
         """
-        Executes the web scraping process and returns the answer to the prompt.
+        Executes the scraping process and returns the answer to the prompt.
 
         Returns:
             str: The answer to the prompt.
         """
 
         inputs = {"user_prompt": self.prompt, self.input_key: self.source}
         self.final_state, self.execution_info = self.graph.execute(inputs)
```

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/graphs/script_creator_graph.py` & `scrapegraphai-1.5.0b2/scrapegraphai/graphs/script_creator_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/graphs/search_graph.py` & `scrapegraphai-1.5.0b2/scrapegraphai/graphs/search_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/graphs/smart_scraper_graph.py` & `scrapegraphai-1.5.0b2/scrapegraphai/graphs/xml_scraper_graph.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,120 +1,107 @@
 """
-SmartScraperGraph Module
+XMLScraperGraph Module
 """
 
 from typing import Optional
 
 from .base_graph import BaseGraph
 from .abstract_graph import AbstractGraph
 
 from ..nodes import (
     FetchNode,
-    ParseNode,
     RAGNode,
     GenerateAnswerNode
 )
 
 
-class SmartScraperGraph(AbstractGraph):
+class XMLScraperGraph(AbstractGraph):
     """
-    SmartScraper is a scraping pipeline that automates the process of 
-    extracting information from web pages
-    using a natural language model to interpret and answer prompts.
+    XMLScraperGraph is a scraping pipeline that extracts information from XML files using a natural
+    language model to interpret and answer prompts.
 
     Attributes:
         prompt (str): The prompt for the graph.
         source (str): The source of the graph.
         config (dict): Configuration parameters for the graph.
         schema (str): The schema for the graph output.
         llm_model: An instance of a language model client, configured for generating answers.
         embedder_model: An instance of an embedding model client, 
         configured for generating embeddings.
         verbose (bool): A flag indicating whether to show print statements during execution.
         headless (bool): A flag indicating whether to run the graph in headless mode.
+        model_token (int): The token limit for the language model.
 
     Args:
         prompt (str): The prompt for the graph.
         source (str): The source of the graph.
         config (dict): Configuration parameters for the graph.
         schema (str): The schema for the graph output.
 
     Example:
-        >>> smart_scraper = SmartScraperGraph(
+        >>> xml_scraper = XMLScraperGraph(
         ...     "List me all the attractions in Chioggia.",
-        ...     "https://en.wikipedia.org/wiki/Chioggia",
+        ...     "data/chioggia.xml",
         ...     {"llm": {"model": "gpt-3.5-turbo"}}
         ... )
-        >>> result = smart_scraper.run()
-        )
+        >>> result = xml_scraper.run()
     """
 
     def __init__(self, prompt: str, source: str, config: dict, schema: Optional[str] = None):
         super().__init__(prompt, config, source, schema)
 
-        self.input_key = "url" if source.startswith("http") else "local_dir"
+        self.input_key = "xml" if source.endswith("xml") else "xml_dir"
 
     def _create_graph(self) -> BaseGraph:
         """
         Creates the graph of nodes representing the workflow for web scraping.
 
         Returns:
             BaseGraph: A graph instance representing the web scraping workflow.
         """
+
         fetch_node = FetchNode(
-            input="url | local_dir",
-            output=["doc", "link_urls", "img_urls"],
-            node_config={
-                "loader_kwargs": self.config.get("loader_kwargs", {}),
-            }
-        )
-        parse_node = ParseNode(
-            input="doc",
-            output=["parsed_doc"],
-            node_config={
-                "chunk_size": self.model_token
-            }
+            input="xml | xml_dir",
+            output=["doc", "link_urls", "img_urls"]
         )
         rag_node = RAGNode(
-            input="user_prompt & (parsed_doc | doc)",
+            input="user_prompt & doc",
             output=["relevant_chunks"],
             node_config={
                 "llm_model": self.llm_model,
                 "embedder_model": self.embedder_model
             }
         )
         generate_answer_node = GenerateAnswerNode(
-            input="user_prompt & (relevant_chunks | parsed_doc | doc)",
+            input="user_prompt & (relevant_chunks | doc)",
             output=["answer"],
             node_config={
                 "llm_model": self.llm_model,
-                "schema": self.schema,
+                "schema": self.schema
             }
         )
 
         return BaseGraph(
             nodes=[
                 fetch_node,
-                parse_node,
                 rag_node,
                 generate_answer_node,
             ],
             edges=[
-                (fetch_node, parse_node),
-                (parse_node, rag_node),
+                (fetch_node, rag_node),
                 (rag_node, generate_answer_node)
             ],
             entry_point=fetch_node
         )
 
     def run(self) -> str:
         """
-        Executes the scraping process and returns the answer to the prompt.
+        Executes the web scraping process and returns the answer to the prompt.
 
         Returns:
             str: The answer to the prompt.
         """
 
         inputs = {"user_prompt": self.prompt, self.input_key: self.source}
         self.final_state, self.execution_info = self.graph.execute(inputs)
 
-        return self.final_state.get("answer", "No answer found.")
+        return self.final_state.get("answer", "No answer found.")
```

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/graphs/smart_scraper_multi_graph.py` & `scrapegraphai-1.5.0b2/scrapegraphai/graphs/smart_scraper_multi_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/graphs/speech_graph.py` & `scrapegraphai-1.5.0b2/scrapegraphai/graphs/speech_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/graphs/xml_scraper_graph.py` & `scrapegraphai-1.5.0b2/scrapegraphai/graphs/pdf_scraper_graph.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 """
-XMLScraperGraph Module
+PDFScraperGraph Module
 """
 
 from typing import Optional
 
 from .base_graph import BaseGraph
 from .abstract_graph import AbstractGraph
 
 from ..nodes import (
     FetchNode,
-    ParseNode,
     RAGNode,
-    GenerateAnswerNode
+    GenerateAnswerPDFNode
 )
 
 
-class XMLScraperGraph(AbstractGraph):
+class PDFScraperGraph(AbstractGraph):
     """
-    XMLScraperGraph is a scraping pipeline that extracts information from XML files using a natural
+    PDFScraperGraph is a scraping pipeline that extracts information from pdf files using a natural
     language model to interpret and answer prompts.
 
     Attributes:
         prompt (str): The prompt for the graph.
         source (str): The source of the graph.
         config (dict): Configuration parameters for the graph.
         schema (str): The schema for the graph output.
@@ -35,74 +34,64 @@
     Args:
         prompt (str): The prompt for the graph.
         source (str): The source of the graph.
         config (dict): Configuration parameters for the graph.
         schema (str): The schema for the graph output.
 
     Example:
-        >>> xml_scraper = XMLScraperGraph(
+        >>> pdf_scraper = PDFScraperGraph(
         ...     "List me all the attractions in Chioggia.",
-        ...     "data/chioggia.xml",
+        ...     "data/chioggia.pdf",
         ...     {"llm": {"model": "gpt-3.5-turbo"}}
         ... )
-        >>> result = xml_scraper.run()
+        >>> result = pdf_scraper.run()
     """
 
     def __init__(self, prompt: str, source: str, config: dict, schema: Optional[str] = None):
-        super().__init__(prompt, config, source, schema)
+        super().__init__(prompt, config, source)
 
-        self.input_key = "xml" if source.endswith("xml") else "xml_dir"
+        self.input_key = "pdf" if source.endswith("pdf") else "pdf_dir"
 
     def _create_graph(self) -> BaseGraph:
         """
         Creates the graph of nodes representing the workflow for web scraping.
 
         Returns:
             BaseGraph: A graph instance representing the web scraping workflow.
         """
 
         fetch_node = FetchNode(
-            input="xml | xml_dir",
-            output=["doc", "link_urls", "img_urls"]
-        )
-        parse_node = ParseNode(
-            input="doc",
-            output=["parsed_doc"],
-            node_config={
-                "chunk_size": self.model_token
-            }
+            input='pdf | pdf_dir',
+            output=["doc"],
         )
         rag_node = RAGNode(
-            input="user_prompt & (parsed_doc | doc)",
+            input="user_prompt & doc",
             output=["relevant_chunks"],
             node_config={
                 "llm_model": self.llm_model,
                 "embedder_model": self.embedder_model
             }
         )
-        generate_answer_node = GenerateAnswerNode(
-            input="user_prompt & (relevant_chunks | parsed_doc | doc)",
+        generate_answer_node_pdf = GenerateAnswerPDFNode(
+            input="user_prompt & (relevant_chunks | doc)",
             output=["answer"],
             node_config={
                 "llm_model": self.llm_model,
-                "schema": self.schema
             }
         )
 
         return BaseGraph(
             nodes=[
                 fetch_node,
-                parse_node,
                 rag_node,
-                generate_answer_node,
+                generate_answer_node_pdf,
             ],
             edges=[
-                (fetch_node, parse_node),
-                (parse_node, rag_node),
-                (rag_node, generate_answer_node)
+                (fetch_node, rag_node),
+                (rag_node, generate_answer_node_pdf)
             ],
             entry_point=fetch_node
         )
 
     def run(self) -> str:
         """
         Executes the web scraping process and returns the answer to the prompt.
```

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/helpers/__init__.py` & `scrapegraphai-1.5.0b2/scrapegraphai/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/helpers/generate_answer_node_csv_prompts.py` & `scrapegraphai-1.5.0b2/scrapegraphai/helpers/generate_answer_node_csv_prompts.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/helpers/generate_answer_node_omni_prompts.py` & `scrapegraphai-1.5.0b2/scrapegraphai/helpers/generate_answer_node_omni_prompts.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/helpers/generate_answer_node_pdf_prompts.py` & `scrapegraphai-1.5.0b2/scrapegraphai/helpers/generate_answer_node_pdf_prompts.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/helpers/generate_answer_node_prompts.py` & `scrapegraphai-1.5.0b2/scrapegraphai/helpers/generate_answer_node_prompts.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/helpers/models_tokens.py` & `scrapegraphai-1.5.0b2/scrapegraphai/helpers/models_tokens.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/helpers/nodes_metadata.py` & `scrapegraphai-1.5.0b2/scrapegraphai/helpers/nodes_metadata.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/helpers/schemas.py` & `scrapegraphai-1.5.0b2/scrapegraphai/helpers/schemas.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/models/bedrock.py` & `scrapegraphai-1.5.0b2/scrapegraphai/models/bedrock.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/models/gemini.py` & `scrapegraphai-1.5.0b2/scrapegraphai/models/gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/models/openai_itt.py` & `scrapegraphai-1.5.0b2/scrapegraphai/models/openai_itt.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/models/openai_tts.py` & `scrapegraphai-1.5.0b2/scrapegraphai/models/openai_tts.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/nodes/__init__.py` & `scrapegraphai-1.5.0b2/scrapegraphai/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/nodes/base_node.py` & `scrapegraphai-1.5.0b2/scrapegraphai/nodes/base_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/nodes/blocks_identifier.py` & `scrapegraphai-1.5.0b2/scrapegraphai/nodes/blocks_identifier.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/nodes/conditional_node.py` & `scrapegraphai-1.5.0b2/scrapegraphai/nodes/conditional_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/nodes/fetch_node.py` & `scrapegraphai-1.5.0b2/scrapegraphai/nodes/fetch_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,16 +86,17 @@
         if (
             input_keys[0] == "json_dir"
             or input_keys[0] == "xml_dir"
             or input_keys[0] == "csv_dir"
             or input_keys[0] == "pdf_dir"
         ):
             compressed_document = [
-                Document(page_content=source, metadata={"source": "local_dir"})
+                source
             ]
+            
             state.update({self.output[0]: compressed_document})
             return state
         # handling for pdf
         elif input_keys[0] == "pdf":
             loader = PyPDFLoader(source)
             compressed_document = loader.load()
             state.update({self.output[0]: compressed_document})
```

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/nodes/generate_answer_csv_node.py` & `scrapegraphai-1.5.0b2/scrapegraphai/nodes/generate_answer_csv_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/nodes/generate_answer_node.py` & `scrapegraphai-1.5.0b2/scrapegraphai/nodes/generate_answer_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/nodes/generate_answer_omni_node.py` & `scrapegraphai-1.5.0b2/scrapegraphai/nodes/generate_answer_omni_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/nodes/generate_answer_pdf_node.py` & `scrapegraphai-1.5.0b2/scrapegraphai/nodes/generate_answer_pdf_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/nodes/generate_scraper_node.py` & `scrapegraphai-1.5.0b2/scrapegraphai/nodes/generate_scraper_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/nodes/get_probable_tags_node.py` & `scrapegraphai-1.5.0b2/scrapegraphai/nodes/get_probable_tags_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/nodes/graph_iterator_node.py` & `scrapegraphai-1.5.0b2/scrapegraphai/nodes/graph_iterator_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/nodes/image_to_text_node.py` & `scrapegraphai-1.5.0b2/scrapegraphai/nodes/image_to_text_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/nodes/knowledge_graph_node.py` & `scrapegraphai-1.5.0b2/scrapegraphai/nodes/knowledge_graph_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/nodes/merge_answers_node.py` & `scrapegraphai-1.5.0b2/scrapegraphai/nodes/merge_answers_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/nodes/parse_node.py` & `scrapegraphai-1.5.0b2/scrapegraphai/nodes/parse_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/nodes/rag_node.py` & `scrapegraphai-1.5.0b2/scrapegraphai/nodes/rag_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/nodes/robots_node.py` & `scrapegraphai-1.5.0b2/scrapegraphai/nodes/robots_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/nodes/search_internet_node.py` & `scrapegraphai-1.5.0b2/scrapegraphai/nodes/search_internet_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/nodes/search_link_node.py` & `scrapegraphai-1.5.0b2/scrapegraphai/nodes/search_link_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/nodes/search_node_with_context.py` & `scrapegraphai-1.5.0b2/scrapegraphai/nodes/search_node_with_context.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/nodes/text_to_speech_node.py` & `scrapegraphai-1.5.0b2/scrapegraphai/nodes/text_to_speech_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/utils/__init__.py` & `scrapegraphai-1.5.0b2/scrapegraphai/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/utils/cleanup_html.py` & `scrapegraphai-1.5.0b2/scrapegraphai/utils/cleanup_html.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/utils/convert_to_csv.py` & `scrapegraphai-1.5.0b2/scrapegraphai/utils/convert_to_csv.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/utils/convert_to_json.py` & `scrapegraphai-1.5.0b2/scrapegraphai/utils/convert_to_json.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/utils/knowledge_graph.py` & `scrapegraphai-1.5.0b2/scrapegraphai/utils/knowledge_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/utils/logging.py` & `scrapegraphai-1.5.0b2/scrapegraphai/utils/logging.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/utils/parse_state_keys.py` & `scrapegraphai-1.5.0b2/scrapegraphai/utils/parse_state_keys.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/utils/prettify_exec_info.py` & `scrapegraphai-1.5.0b2/scrapegraphai/utils/prettify_exec_info.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/utils/proxy_rotation.py` & `scrapegraphai-1.5.0b2/scrapegraphai/utils/proxy_rotation.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/utils/research_web.py` & `scrapegraphai-1.5.0b2/scrapegraphai/utils/research_web.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/utils/save_audio_from_bytes.py` & `scrapegraphai-1.5.0b2/scrapegraphai/utils/save_audio_from_bytes.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/utils/sys_dynamic_import.py` & `scrapegraphai-1.5.0b2/scrapegraphai/utils/sys_dynamic_import.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/scrapegraphai/utils/token_calculator.py` & `scrapegraphai-1.5.0b2/scrapegraphai/utils/token_calculator.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/tests/graphs/scrape_json_ollama.py` & `scrapegraphai-1.5.0b2/tests/graphs/scrape_json_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/tests/graphs/scrape_plain_text_llama3_test.py` & `scrapegraphai-1.5.0b2/tests/graphs/scrape_plain_text_llama3_test.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/tests/graphs/scrape_plain_text_mistral_test.py` & `scrapegraphai-1.5.0b2/tests/graphs/scrape_plain_text_mistral_test.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/tests/graphs/scrape_xml_ollama_test.py` & `scrapegraphai-1.5.0b2/tests/graphs/scrape_xml_ollama_test.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/tests/graphs/script_generator_test.py` & `scrapegraphai-1.5.0b2/tests/graphs/script_generator_test.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/tests/graphs/smart_scraper_ollama_test.py` & `scrapegraphai-1.5.0b2/tests/graphs/smart_scraper_ollama_test.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/tests/graphs/inputs/books.xml` & `scrapegraphai-1.5.0b2/tests/graphs/inputs/books.xml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/tests/graphs/inputs/example.json` & `scrapegraphai-1.5.0b2/tests/graphs/inputs/example.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/tests/graphs/inputs/plain_html_example.txt` & `scrapegraphai-1.5.0b2/tests/graphs/inputs/plain_html_example.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/tests/nodes/fetch_node_test.py` & `scrapegraphai-1.5.0b2/tests/nodes/fetch_node_test.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/tests/nodes/robot_node_test.py` & `scrapegraphai-1.5.0b2/tests/nodes/robot_node_test.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/tests/nodes/search_link_node_test.py` & `scrapegraphai-1.5.0b2/tests/nodes/search_link_node_test.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/tests/nodes/inputs/books.xml` & `scrapegraphai-1.5.0b2/tests/nodes/inputs/books.xml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/tests/nodes/inputs/example.json` & `scrapegraphai-1.5.0b2/tests/nodes/inputs/example.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/tests/nodes/inputs/plain_html_example.txt` & `scrapegraphai-1.5.0b2/tests/nodes/inputs/plain_html_example.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/tests/utils/test_proxy_rotation.py` & `scrapegraphai-1.5.0b2/tests/utils/test_proxy_rotation.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/tests/utils/test_sys_dynamic_import.py` & `scrapegraphai-1.5.0b2/tests/utils/test_sys_dynamic_import.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/LICENSE` & `scrapegraphai-1.5.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/README.md` & `scrapegraphai-1.5.0b2/README.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b1/pyproject.toml` & `scrapegraphai-1.5.0b2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "scrapegraphai"
 
 
-version = "1.5.0b1"
+version = "1.5.0b2"
 
 
 description = "A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines."
 authors = [
     { name = "Marco Vinciguerra", email = "mvincig11@gmail.com" },
     { name = "Marco Perini", email = "perinim.98@gmail.com" },
     { name = "Lorenzo Padoan", email = "lorenzo.padoan977@gmail.com" }
```

### Comparing `scrapegraphai-1.5.0b1/PKG-INFO` & `scrapegraphai-1.5.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: scrapegraphai
-Version: 1.5.0b1
+Version: 1.5.0b2
 Summary: A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines.
 Author-email: Marco Vinciguerra <mvincig11@gmail.com>, Marco Perini <perinim.98@gmail.com>, Lorenzo Padoan <lorenzo.padoan977@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: ai,artificial intelligence,gpt,graph,langchain,machine learning,natural language processing,nlp,openai,rag,scrapegraph,scrapegraphai,scraping,web scraping,web scraping library,web scraping tool,webscraping
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

