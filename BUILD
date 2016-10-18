package(default_visibility = ['//visibility:public'])
licenses(['notice'])

load('lemonscript', 'cc_lemonscript_library')

py_binary(
  name = 'lemonscript_transpiler',
  srcs = ['transpiler.py'] + glob(['objects/*.py']),
  main = 'transpiler.py'
)

cc_lemonscript_library(
  name = 'wait_func',
  srcs = ['tests/files/transpiler/auto_functions/wait.func'],
  deps = ['//muan/utils:timing'],
)
