# SPDX-FileCopyrightText: 2021 The meson-python developers
#
# SPDX-License-Identifier: MIT

project('meson-python', version: '0.13.2')

py_mod = import('python')
py = py_mod.find_installation()

if py.language_version().version_compare('< 3.6')
  error('Invalid Python version, only >= 3.6 is supported.')
endif

py.install_sources(
  'mesonpy/__init__.py',
  'mesonpy/_compat.py',
  'mesonpy/_dylib.py',
  'mesonpy/_editable.py',
  'mesonpy/_elf.py',
  'mesonpy/_tags.py',
  'mesonpy/_util.py',
  'mesonpy/_wheelfile.py',
  subdir: 'mesonpy',
)
