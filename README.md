[![Build Status](https://dev.azure.com/mhirsch0512/netlib-blas/_apis/build/status/scivision.netlib-blas?branchName=master)](https://dev.azure.com/mhirsch0512/netlib-blas/_build/latest?definitionId=14&branchName=master)

# Netlib BLAS

...provided with meson.build for easy inclusion as subproject in your Meson project(s).
The source code is unmodified. THe .tgz from Netlib comes with numerous extraneous virus scan quarantine files. This repo emits the junk files.

## build

Requires Fortran compiler and Meson build system.

```sh
meson build

meson test -C build
```

## reference

examples from https://scc.ustc.edu.cn/zlsc/sugon/intel/mkl/mkl_manual/GUID-71558CA4-1077-4203-B0BB-165BAB18899E.htm