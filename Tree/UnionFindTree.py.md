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
  code: "class UnionFind:\n    def __init__(self, n):\n        self.n = n\n      \
    \  self.p = [-1] * n\n\n\n    def leader(self, a):\n        while self.p[a] >=\
    \ 0:\n            a = self.p[a]\n        return a\n\n\n    def merge(self, a,\
    \ b):\n        x = self.leader(a)\n        y = self.leader(b)\n\n        if x\
    \ == y:\n            return x\n\n        if self.p[x] > self.p[y]:\n         \
    \   x, y = y, x\n\n        self.p[x] += self.p[y]\n        self.p[y] = x\n\n \
    \       return x\n\n    def same(self, a, b):\n        return self.leader(a) ==\
    \ self.leader(b)\n\n    def size(self, a):\n        return -self.p[self.leader(a)]\n\
    \nn, m = map(int,input().split())\n\nuf = UnionFind(n)\n\nfor _ in range(m):\n\
    \    a, b = map(int,input().split())\n    uf.merge(a - 1, b - 1)\n\nans = 0\n\
    for i in range(n):\n    ans = max(ans, uf.size(i))\n\nprint(ans)"
  dependsOn: []
  isVerificationFile: false
  path: Tree/UnionFindTree.py
  requiredBy: []
  timestamp: '2022-05-07 23:18:50+09:00'
  verificationStatus: LIBRARY_NO_TESTS
  verifiedWith: []
documentation_of: Tree/UnionFindTree.py
layout: document
redirect_from:
- /library/Tree/UnionFindTree.py
- /library/Tree/UnionFindTree.py.html
title: Tree/UnionFindTree.py
---
