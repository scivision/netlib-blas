allblas = files('lsame.f', 'xerbla.f', 'xerbla_array.f')

if arith.contains('s')
   blas1 = files('isamax.f', 'sasum.f', 'saxpy.f', 'scopy.f', 'sdot.f', 'snrm2.f', 'srot.f', 'srotg.f', 'sscal.f', 'sswap.f', 'sdsdot.f', 'srotmg.f', 'srotm.f')

  blas2 = files('sgemv.f', 'sgbmv.f', 'ssymv.f', 'ssbmv.f', 'sspmv.f', 'strmv.f', 'stbmv.f', 'stpmv.f', 'strsv.f', 'stbsv.f', 'stpsv.f', 'sger.f', 'ssyr.f', 'sspr.f', 'ssyr2.f', 'sspr2.f')

  blas3 = files('sgemm.f', 'ssymm.f', 'ssyrk.f', 'ssyr2k.f', 'strmm.f', 'strsm.f')
endif

if arith.contains('c')
  blas1 = files('scabs1.f', 'scasum.f', 'scnrm2.f', 'icamax.f', 'caxpy.f', 'ccopy.f', 'cdotc.f', 'cdotu.f', 'csscal.f', 'crotg.f', 'cscal.f', 'cswap.f', 'csrot.f',
  'isamax.f', 'sasum.f', 'saxpy.f', 'scopy.f', 'snrm2.f', 'sscal.f')

  blas2 = files('cgemv.f', 'cgbmv.f', 'chemv.f', 'chbmv.f', 'chpmv.f', 'ctrmv.f', 'ctbmv.f', 'ctpmv.f', 'ctrsv.f', 'ctbsv.f', 'ctpsv.f', 'cgerc.f', 'cgeru.f', 'cher.f', 'chpr.f', 'cher2.f', 'chpr2.f')

  blas3 = files('cgemm.f', 'csymm.f', 'csyrk.f', 'csyr2k.f', 'ctrmm.f', 'ctrsm.f', 'chemm.f', 'cherk.f', 'cher2k.f')
endif

if arith.contains('d')
  blas1 = files('idamax.f', 'dasum.f', 'daxpy.f', 'dcopy.f', 'ddot.f', 'dnrm2.f', 'drot.f', 'drotg.f', 'dscal.f', 'dsdot.f', 'dswap.f', 'drotmg.f', 'drotm.f')

  blas2 = files('dgemv.f', 'dgbmv.f', 'dsymv.f', 'dsbmv.f', 'dspmv.f', 'dtrmv.f', 'dtbmv.f', 'dtpmv.f', 'dtrsv.f', 'dtbsv.f', 'dtpsv.f', 'dger.f', 'dsyr.f', 'dspr.f', 'dsyr2.f', 'dspr2.f')

  blas3 = files('dgemm.f', 'dsymm.f', 'dsyrk.f', 'dsyr2k.f', 'dtrmm.f', 'dtrsm.f')
endif

if arith.contains('z')
  blas1 = files('dcabs1.f', 'dzasum.f', 'dznrm2.f', 'izamax.f', 'zaxpy.f', 'zcopy.f', 'zdotc.f', 'zdotu.f', 'zdscal.f', 'zrotg.f', 'zscal.f', 'zswap.f', 'zdrot.f',
  'idamax.f', 'dasum.f', 'daxpy.f', 'dcopy.f', 'dnrm2.f', 'dscal.f')

  blas2 = files('zgemv.f', 'zgbmv.f', 'zhemv.f', 'zhbmv.f', 'zhpmv.f', 'ztrmv.f', 'ztbmv.f', 'ztpmv.f', 'ztrsv.f', 'ztbsv.f', 'ztpsv.f', 'zgerc.f', 'zgeru.f', 'zher.f', 'zhpr.f', 'zher2.f', 'zhpr2.f')

  blas3 = files('zgemm.f', 'zsymm.f', 'zsyrk.f', 'zsyr2k.f', 'ztrmm.f', 'ztrsm.f', 'zhemm.f', 'zherk.f', 'zher2k.f')
endif


blas = library('blas',
  sources: [blas1, allblas, blas2, blas3],
  install: true,
  install_dir: install_dir,
)