# Numo::LAPACK : LAPACK binding with Numo::NArray

## Introduction

This is a binding of LAPACK with Numo::NArray .

## ToDo

rewrite this README

## Implemented Methods

    x = Numo::Linalg.matmul(a,b)   (_gemm) Matrix multiply
    x = Numo::Linalg.solve(a,b)    (_gesv) Solve Linear equation with LU factorization
    x,y = Numo::Linalg.eigen(a)  (_geev) Eigen value and Eigen vector

* [GitHub](https://github.com/ruby-numo/linalg)

## Installation

* Install [Numo::NArray](https://github.com/ruby-numo/narray)
* Install [LAPACK](http://www.netlib.org/lapack/) or [OpenBLAS](http://www.openblas.net/)
  * Yum intall:
  ```shell
$ yum install openblas-devel
```
  * or, install OpenBLAS from source and enjoy multithread acceleration.

* Install Numo::Linalg
  ```shell
$ git clone git://github.com/ruby-numo/linalg.git
$ cd linalg
$ rake build
$ gem install pkg/numo-linalg-*.gem -- --with-openblas --with-opt-dir=/opt/OpenBLAS
```

## ToDo

* rank
* norm
* det
* lstsq
* inv
* pinv
* cholesky
* qr
* svd
* eigh
* eigvals
* eigvalsh
