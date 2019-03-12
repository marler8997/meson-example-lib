project('libexample', 'c',
  version : '1.0.0')

libexample = library('libexample',
  'examplestuff.c',
  include_directories : include_directories('.'),
  install : true)

install_headers('example.h')

pkgconfig = import('pkgconfig')
pkgconfig.generate(
  libraries : libexample,
  version : '1.0',
  name : 'libexample',
  description : 'An example library')
