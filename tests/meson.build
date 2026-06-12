catch2_dep = dependency(
  'catch2-with-main',
  fallback : ['catch2', 'catch2_with_main_dep'],
  required : get_option('tests')
)

subdir('unit')
