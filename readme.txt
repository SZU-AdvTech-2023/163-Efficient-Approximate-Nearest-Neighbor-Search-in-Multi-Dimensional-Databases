Prerequisites:
- GCC
- CMake
- Boost
- TCMalloc
- libgoogle-perftools-dev
- libunwind-0.99-beta


Run:
- test_taumng_index.cpp: it is the main file to construct a tauMNG
- test_taumng_search.cpp: it is the main file to perform ANN search on tauMNG

本论文基于NSG（https://gitee.com/code0_FC/nsg?_from=gitee_search），代码所有的修改都在NSG的基础上，只需要按照NSG的安装步骤下载，然后替换对应的代码部分即可

主要命令：
$ tau-mg1.0/build/tests/test_nsg_index sift.fvecs sift_200nn.graph 40 50 500 8 8 sift.tmg
$ tau-mg1.0/build/tests/test_nsg_search sift.fvecs query.fvecs data_sum.fvecs true.ivecs sift.tmg 100 100 0.5 100 tau_result.ivecs

