project(
  'mongoose',
  'c',
  version: '6.15',
  license: 'GPLv2')

incdir = include_directories('src')

libmongoose = library(
  'mongoose',
  'mongoose.c',
  include_directories: incdir,
  install: true)

install_headers('mongoose.h')

pkg = import('pkgconfig')
pkg.generate(
  libmongoose,
  description: 'Embedded Web Server Library.')
