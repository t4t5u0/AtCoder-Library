---
data:
  _extendedDependsOn: []
  _extendedRequiredBy: []
  _extendedVerifiedWith: []
  _isVerificationFailed: false
  _pathExtension: py
  _verificationStatusIcon: ':warning:'
  attributes:
    links:
    - https://atcoder.jp/contests/typical-algorithm/tasks/typical_algorithm_f
  bundledCode: "Traceback (most recent call last):\n  File \"/Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/onlinejudge_verify/documentation/build.py\"\
    , line 71, in _render_source_code_stat\n    bundled_code = language.bundle(stat.path,\
    \ basedir=basedir, options={'include_paths': [basedir]}).decode()\n  File \"/Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/onlinejudge_verify/languages/python.py\"\
    , line 96, in bundle\n    raise NotImplementedError\nNotImplementedError\n"
  code: "# \u30AF\u30E9\u30B9\u30AB\u30EB\u6CD5\n# \u51FA\u5178\uFF1Ahttps://atcoder.jp/contests/typical-algorithm/tasks/typical_algorithm_f\n\
    \nclass UnionFind:\n  def __init__(self, n):\n    self.n = n\n    self.p = [-1]\
    \ * n\n\n  def leader(self, a):\n    while self.p[a] >= 0:\n      a = self.p[a]\n\
    \    return a\n\n  def merge(self, a, b):\n    x = self.leader(a)\n    y = self.leader(b)\n\
    \    if x == y: return x\n    if self.p[x] > self.p[y]:\n      x, y = y, x\n \
    \   self.p[x] += self.p[y]\n    self.p[y] = x\n    return x\n\n  def same(self,\
    \ a, b): return self.leader(a) == self.leader(b)\n\n  def size(self, a): return\
    \ -self.p[self.leader(a)]\n\nn, m = map(int, input().split())\n\nuf = UnionFind(n)\n\
    \n# (a, b, cost)\u306E\u7121\u5411\u30B0\u30E9\u30D5\n\ng = [list(map(int, input().split()))\
    \ for _ in range(m)]\ng.sort(key=lambda x: x[2])\n\nans = 0\nfor i, j, cost in\
    \ g:\n    if uf.same(i, j): continue\n    uf.merge(i, j)\n    ans += cost\n\n\
    print(ans)"
  dependsOn: []
  isVerificationFile: false
  path: Graph/Kruskal.py
  requiredBy: []
  timestamp: '2022-02-06 18:39:20+09:00'
  verificationStatus: LIBRARY_NO_TESTS
  verifiedWith: []
documentation_of: Graph/Kruskal.py
layout: document
redirect_from:
- /library/Graph/Kruskal.py
- /library/Graph/Kruskal.py.html
title: Graph/Kruskal.py
---
