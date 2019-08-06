project('Netlib-BLAS', 'fortran',
  version: '3.7.0',
  default_options : ['default_library=static', 'buildtype=release', 'warning_level=0'])

install_dir = 'blas-'+meson.project_version()

arith = get_option('arith')
message('using arithmatic: '+ arith)

subdir('src')

if arith=='d'
  exe1 = executable('blas1_example', 'tests/ex1.F90',
    link_with: blas,
    fortran_args: '-Darith='+arith)
  test('BLAS L1', exe1, timeout: 10)

  exe2 = executable('blas2_example', 'tests/ex2.F90',
    link_with: blas,
    fortran_args: '-Darith='+arith)
  test('BLAS L2', exe2, timeout: 10)

    exe3 = executable('blas3_example', 'tests/ex3.F90',
    link_with: blas,
    fortran_args: '-Darith='+arith)
  test('BLAS L3', exe3, timeout: 10)
endif