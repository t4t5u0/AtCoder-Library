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
  code: "# \u8A08\u7B97\u91CF\uFF1AO(|V||E|)\ndef bellman_ford(s: int) -> list:\n\
    \    '\u8CA0\u306E\u30B3\u30B9\u30C8\u3092\u6301\u3064\u6700\u77ED\u7D4C\u8DEF\
    \u554F\u984C'\n    INF = 10 ** 18\n    dist = [INF] * n\n    dist[s] = 0\n   \
    \ for i in range(n):\n        update = False # \u7D4C\u8DEF\u66F4\u65B0\u3092\u884C\
    \u3063\u305F\u304B\n        for a, b, cost in g:\n            if dist[a] > dist[b]\
    \ + cost:\n                dist[a] = dist[b] + cost\n                update =\
    \ True\n\n        # \u66F4\u65B0\u304C\u884C\u308F\u308C\u306A\u3051\u308C\u3070\
    \u305D\u308C\u304C\u6700\u77ED\u7D4C\u8DEF\u3068\u306A\u308B\n        if not update:\n\
    \            break\n\n        if i == n - 1:\n            return -1\n\n    return\
    \ dist\n\nn, m = map(int, input().split())\ng = []\nfor _ in range(m):\n    u,\
    \ v, cost = map(int, input().split())\n    u -= 1\n    v -= 1\n    g.append((u,\
    \ v, cost))\n    g.append((v, u, cost))\n\nans = bellman_ford(0)\n\nif ans ==\
    \ -1:\n    print('Yes')\nelse:\n    print(ans)"
  dependsOn: []
  isVerificationFile: false
  path: Graph/bellman_ford.py
  requiredBy: []
  timestamp: '2022-02-06 18:44:34+09:00'
  verificationStatus: LIBRARY_NO_TESTS
  verifiedWith: []
documentation_of: Graph/bellman_ford.py
layout: document
redirect_from:
- /library/Graph/bellman_ford.py
- /library/Graph/bellman_ford.py.html
title: Graph/bellman_ford.py
---
