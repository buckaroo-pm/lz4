load('//:buckaroo_macros.bzl', 'buckaroo_deps')
load('//:subdir_glob.bzl', 'subdir_glob')

cxx_library(
  name = 'lz4',
  header_namespace = '',
  exported_headers = {
    'lz4.h': 'lib/lz4.h',
  },
  headers = subdir_glob([
    ('lib', '*.h'),
    ('', 'lib/**/*.c'),
  ]),
  srcs = [
    'lib/lz4hc.c',
    'lib/lz4.c',
  ],
  deps = buckaroo_deps(),
  visibility = [
    'PUBLIC',
  ],
)
