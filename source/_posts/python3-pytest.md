---
title: python3-pytest
toc: true
date: 2020-12-05 10:36:02
tags: [python3, pytest]
categories: 技术
---

配置文件：

pytest.ini

`[pytest]
required_plugins = pytest-flask>=1.1.0 pytest-html>=3.0.0 pytest-xdist>=2.0.0

addopts = -v --html=tests/report.html -n 4 -rxXs
; -v 详细信息
; -html 输出HTML报告
; -n 4 并发4
; -rxXs  # show extra info on xfailed, xpassed, and skipped tests
testpaths = tests

markers =
  webtest:  Run the webtest case
  hello: Run the hello case

 xfail_strict = true`