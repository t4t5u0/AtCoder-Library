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
  code: "from collections import deque\n\ndef bfs(sy: int, sx: int) -> list:\n   \
    \ '\u59CB\u70B9\u5EA7\u6A19\u3092\u53D7\u3051\u53D6\u3063\u3066BFS'\n    INF =\
    \ 10 ** 18\n    dist = [[INF] * w for _ in range(h)]\n    dist[sy][sx] = 0\n \
    \   \n    # \u969C\u5BB3\u7269\u306E\u78BA\u8A8D\n    for i in range(h):\n   \
    \     for j in range(w):\n            if grid[i][j] == '#':\n                dist[i][j]\
    \ = -1\n    \n    # BFS\n    d = ((0, 1), (0, -1), (1, 0), (-1, 0))\n    q = deque()\n\
    \    q.append((sy, sx))\n\n    while q:\n        vy, vx = q.popleft()\n      \
    \  for dy, dx in d:\n            y = vy + dy\n            x = vx + dx\n      \
    \      if not (0 <= x < w and 0 <= y < h): continue\n            if grid[y][x]\
    \ == '#': continue\n            if dist[y][x] != INF: continue\n            dist[y][x]\
    \ = dist[vy][vx] + 1\n            q.append((y, x))\n    \n    return dist\n\n\
    h, w = map(int, input().split())\ngrid = [list(input()) for _ in range(h)]\n\n\
    dist = bfs(0, 0)\nprint(*dist, sep='\\n')"
  dependsOn: []
  isVerificationFile: false
  path: Search/BreadthFirstSearch.py
  requiredBy: []
  timestamp: '1970-01-01 00:00:00+00:00'
  verificationStatus: LIBRARY_NO_TESTS
  verifiedWith: []
documentation_of: Search/BreadthFirstSearch.py
layout: document
redirect_from:
- /library/Search/BreadthFirstSearch.py
- /library/Search/BreadthFirstSearch.py.html
title: Search/BreadthFirstSearch.py
---
