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
  code: "def check(arg):\n    if 1:\n        return True\n    else:\n       return\
    \ False\n\ndef binary_search(left: int, right: int) -> int:\n    while right -\
    \ left > 1:\n        mid = (left + right) // 2\n        if check(mid):\n     \
    \       left = mid\n        else:\n            right = mid\n\n    return left\n\
    \nINF = 10 ** 18\nl, r = -1, INF\nprint(binary_search(l, r))"
  dependsOn: []
  isVerificationFile: false
  path: Search/BinarySearch.py
  requiredBy: []
  timestamp: '2022-02-06 18:49:09+09:00'
  verificationStatus: LIBRARY_NO_TESTS
  verifiedWith: []
documentation_of: Search/BinarySearch.py
layout: document
redirect_from:
- /library/Search/BinarySearch.py
- /library/Search/BinarySearch.py.html
title: Search/BinarySearch.py
---
