project(
  'zagra',
  'cpp',
  version : '0.1.0',
  default_options : [
    'cpp_std=c++17',
    'buildtype=debugoptimized',
    'warning_level=3',
  ],
)

libzagra_inc = include_directories('include')

libzagra = static_library(
  'zagra',
  'src/zagra.cpp',
  include_directories : libzagra_inc,
  install : true,
)

zagra_dep = declare_dependency(
  link_with : libzagra,
  include_directories : libzagra_inc,
)

install_headers(
  'include/zagra.hpp',
  subdir: 'zagra'
)

if get_option('tests').enabled()
  subdir('tests')
endif
