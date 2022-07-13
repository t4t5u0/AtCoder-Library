---
data:
  _extendedDependsOn: []
  _extendedRequiredBy: []
  _extendedVerifiedWith: []
  _isVerificationFailed: false
  _pathExtension: py
  _verificationStatusIcon: ':warning:'
  attributes:
    links: []
  bundledCode: "Traceback (most recent call last):\n  File \"/Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/onlinejudge_verify/documentation/build.py\"\
    , line 71, in _render_source_code_stat\n    bundled_code = language.bundle(stat.path,\
    \ basedir=basedir, options={'include_paths': [basedir]}).decode()\n  File \"/Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/onlinejudge_verify/languages/python.py\"\
    , line 96, in bundle\n    raise NotImplementedError\nNotImplementedError\n"
  code: "from itertools import product\n\ndef BitSearch(x, l): # \u30EA\u30B9\u30C8\
    \u30FB\u6570\n    num = 0\n    for i in product([0, 1], repeat = l):\n       \
    \ for j in range(l):\n            if i[j] == 1: # 1 <-> bit\u304C\u7ACB\u3063\u3066\
    \u3044\u308B\u6642\n                # O(1)"
  dependsOn: []
  isVerificationFile: false
  path: Search/BitSearch.py
  requiredBy: []
  timestamp: '2021-04-29 00:25:13+09:00'
  verificationStatus: LIBRARY_NO_TESTS
  verifiedWith: []
documentation_of: Search/BitSearch.py
layout: document
redirect_from:
- /library/Search/BitSearch.py
- /library/Search/BitSearch.py.html
title: Search/BitSearch.py
---
