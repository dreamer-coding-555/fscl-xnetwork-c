code = files('module.c')

common_dep = dependency('fscl-xcommon-c')
curl_dep = dependency('libcurl', default_options: ['warning_level=0']) # issue from CURL test file for strdup

lib = library('fscl-xnetwork-c',
    code,
    dependencies : [common_dep, curl_dep],
    install: true,
    include_directories: dir)

fscl_xnetwork_c_dep = declare_dependency(
    link_with: lib,
    dependencies : [common_dep, curl_dep],
    include_directories: dir)
