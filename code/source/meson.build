code = files('module.c')

common_dep = dependency('fscl-xcommon-c')
curl_dep = dependency('curl')

lib = library('fscl-c',
    code,
    dependencies : [common_dep, curl_dep],
    install: true,
    include_directories: dir)

fscl_xnetwork_c_dep = declare_dependency(
    link_with: lib,
    dependencies : [common_dep, curl_dep],
    include_directories: dir)
