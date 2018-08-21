use_relative_paths = True

deps = {
  "vendor/python-patch": "https://github.com/svn2github/python-patch@a336a458016ced89aba90dfc3f4c8222ae3b1403",
}

hooks = [
  {
    'name': 'build-patches',
    'pattern': '.',
    'action': ['python', 'src/cipatches/bin/apply-patches.py'],
  }
]
