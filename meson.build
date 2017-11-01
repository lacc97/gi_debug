project('gi_debug', 'c', version : '0.9.5')

pkg = import('pkgconfig')

gi_debug_lib = static_library('gi_debug', 'gi_debug.c', install : true, install_dir : get_option('libdir') + '/glk/debug')
install_headers('gi_debug.h', subdir : 'glk/debug')
pkg.generate(
    name :          'gi_debug',
    description :   'Glk debug layer',
    version :       meson.project_version(),
    subdirs :       'glk/debug',
    libraries :     gi_debug_lib
) 
