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
  code: "def PrimaryCheck(x):\n    if n == 1: return False\n    for i in range(2,\
    \ int(x ** 0.5) + 1):\n        if x % i == 0:\n            return False\n    return\
    \ True\n\nn = int(input())\nnum = PrimaryCheck(n)\nprint(num)"
  dependsOn: []
  isVerificationFile: false
  path: MathLibrary/PrimaryCheck.py
  requiredBy: []
  timestamp: '2022-07-14 11:56:28+09:00'
  verificationStatus: LIBRARY_NO_TESTS
  verifiedWith: []
documentation_of: MathLibrary/PrimaryCheck.py
layout: document
redirect_from:
- /library/MathLibrary/PrimaryCheck.py
- /library/MathLibrary/PrimaryCheck.py.html
title: MathLibrary/PrimaryCheck.py
---
