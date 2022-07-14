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
  code: "def FloatToInt(FLOAT):\n    return int(FLOAT.replace(\".\", \"\")), len(FLOAT)\
    \ - FLOAT.index(\".\") - 1 # tuple \u3067return\n\nn = \"314.1592653589\" # \u958B\
    \u59CB\u306Fstr\u3067\u6E21\u3059\nx, y = FloatToInt(n)\nprint(x, y)"
  dependsOn: []
  isVerificationFile: false
  path: MathLibrary/FromFloatToInt.py
  requiredBy: []
  timestamp: '2022-07-14 11:56:28+09:00'
  verificationStatus: LIBRARY_NO_TESTS
  verifiedWith: []
documentation_of: MathLibrary/FromFloatToInt.py
layout: document
redirect_from:
- /library/MathLibrary/FromFloatToInt.py
- /library/MathLibrary/FromFloatToInt.py.html
title: MathLibrary/FromFloatToInt.py
---
