---
data:
  _extendedDependsOn: []
  _extendedRequiredBy: []
  _extendedVerifiedWith: []
  _isVerificationFailed: true
  _pathExtension: py
  _verificationStatusIcon: ':x:'
  attributes:
    PROBLEM: https://judge.yosupo.jp/problem/unionfind
    links:
    - https://judge.yosupo.jp/problem/unionfind
  bundledCode: "Traceback (most recent call last):\n  File \"/Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/onlinejudge_verify/documentation/build.py\"\
    , line 71, in _render_source_code_stat\n    bundled_code = language.bundle(stat.path,\
    \ basedir=basedir, options={'include_paths': [basedir]}).decode()\n  File \"/Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/onlinejudge_verify/languages/python.py\"\
    , line 96, in bundle\n    raise NotImplementedError\nNotImplementedError\n"
  code: "# verification-helper: PROBLEM https://judge.yosupo.jp/problem/unionfind\n\
    \nclass UnionFind:\n    def __init__(self, n):\n        self.n = n\n        self.p\
    \ = [-1] * n\n\n\n    def leader(self, a):\n        while self.p[a] >= 0:\n  \
    \          a = self.p[a]\n        return a\n\n\n    def merge(self, a, b):\n \
    \       x = self.leader(a)\n        y = self.leader(b)\n\n        if x == y:\n\
    \            return x\n\n        if self.p[x] > self.p[y]:\n            x, y =\
    \ y, x\n\n        self.p[x] += self.p[y]\n        self.p[y] = x\n\n        return\
    \ x\n\n    def same(self, a, b):\n        return self.leader(a) == self.leader(b)\n\
    \n    def size(self, a):\n        return -self.p[self.leader(a)]\n\nn, q = map(int,input().split())\n\
    \nuf = UnionFind(n)\n\nfor _ in range(q):\n    t, u, v = map(int,input().split())\n\
    \    if t == 0:\n        uf.merge(u, v)\n    elif t == 1:\n        print(1) if\
    \ uf.same(u, v) else print(0)"
  dependsOn: []
  isVerificationFile: true
  path: test/yosupo/Unionfind.test.py
  requiredBy: []
  timestamp: '2022-07-14 23:33:07+09:00'
  verificationStatus: TEST_WRONG_ANSWER
  verifiedWith: []
documentation_of: test/yosupo/Unionfind.test.py
layout: document
redirect_from:
- /verify/test/yosupo/Unionfind.test.py
- /verify/test/yosupo/Unionfind.test.py.html
title: test/yosupo/Unionfind.test.py
---
