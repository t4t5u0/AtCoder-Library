---
data:
  _extendedDependsOn: []
  _extendedRequiredBy: []
  _extendedVerifiedWith: []
  _isVerificationFailed: false
  _pathExtension: cpp
  _verificationStatusIcon: ':heavy_check_mark:'
  attributes:
    '*NOT_SPECIAL_COMMENTS*': ''
    PROBLEM: https://onlinejudge.u-aizu.ac.jp/courses/lesson/1/ALDS1/4/ALDS1_4_B
    links:
    - https://onlinejudge.u-aizu.ac.jp/courses/lesson/1/ALDS1/4/ALDS1_4_B
  bundledCode: "Traceback (most recent call last):\n  File \"/Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/onlinejudge_verify/documentation/build.py\"\
    , line 71, in _render_source_code_stat\n    bundled_code = language.bundle(stat.path,\
    \ basedir=basedir, options={'include_paths': [basedir]}).decode()\n  File \"/Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/onlinejudge_verify/languages/cplusplus.py\"\
    , line 187, in bundle\n    bundler.update(path)\n  File \"/Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/onlinejudge_verify/languages/cplusplus_bundle.py\"\
    , line 289, in update\n    uncommented_lines = get_uncommented_code(path, iquotes=self.iquotes,\
    \ compiler=self.compiler).splitlines(keepends=True)\n  File \"/Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/onlinejudge_verify/languages/cplusplus_bundle.py\"\
    , line 195, in get_uncommented_code\n    code = _get_uncommented_code(path.resolve(),\
    \ iquotes_options=tuple(iquotes_options), compiler=compiler)\n  File \"/Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/onlinejudge_verify/languages/cplusplus_bundle.py\"\
    , line 185, in _get_uncommented_code\n    raise BundleError(f'A fake g++ is detected.\
    \ Please install the GNU C++ compiler.: {compiler}')\nonlinejudge_verify.languages.cplusplus_bundle.BundleError:\
    \ A fake g++ is detected. Please install the GNU C++ compiler.: g++\n"
  code: "#define PROBLEM \"https://onlinejudge.u-aizu.ac.jp/courses/lesson/1/ALDS1/4/ALDS1_4_B\"\
    \n#include <algorithm>\n#include <iostream>\n#include <vector>\n#define REP(i,\
    \ n) for (int i = 0; (i) < (int)(n); ++ (i))\n#define ALL(x) std::begin(x), std::end(x)\n\
    using namespace std;\n\nint main() {\n    int n; cin >> n;\n    vector<int> s(n);\n\
    \    REP (i, n) {\n        cin >> s[i];\n    }\n    int q; cin >> q;\n    int\
    \ cnt = 0;\n    while (q --) {\n        int t_i; cin >> t_i;\n        cnt += binary_search(ALL(s),\
    \ t_i);\n    }\n    cout << cnt << endl;\n    return 0;\n}\n"
  dependsOn: []
  isVerificationFile: true
  path: example.test.cpp
  requiredBy: []
  timestamp: '2022-02-06 19:51:52+09:00'
  verificationStatus: TEST_ACCEPTED
  verifiedWith: []
documentation_of: example.test.cpp
layout: document
redirect_from:
- /verify/example.test.cpp
- /verify/example.test.cpp.html
title: example.test.cpp
---
