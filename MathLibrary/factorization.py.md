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
  code: "def factorization(n):\n    arr = []\n    tmp = n\n    for i in range(2, int(-(-n**0.5//1))+1):\n\
    \        if tmp % i == 0:\n            cnt = 0\n            while tmp % i == 0:\n\
    \                cnt += 1\n                tmp //= i\n            arr.append([i,\
    \ cnt])\n    if tmp != 1:\n        arr.append([tmp, 1])\n    if arr == []:\n \
    \       arr.append([n, 1])\n    return arr\n\nprint(factorization(2592))"
  dependsOn: []
  isVerificationFile: false
  path: MathLibrary/factorization.py
  requiredBy: []
  timestamp: '2022-07-14 11:56:28+09:00'
  verificationStatus: LIBRARY_NO_TESTS
  verifiedWith: []
documentation_of: MathLibrary/factorization.py
layout: document
redirect_from:
- /library/MathLibrary/factorization.py
- /library/MathLibrary/factorization.py.html
title: MathLibrary/factorization.py
---
