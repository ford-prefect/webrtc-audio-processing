pffft_sources = [
  'src/pffft.c',
]

# FIXME: see BUILD.gn for SIMD handling notes

libpffft = static_library('libpffft',
    pffft_sources,
    dependencies: common_deps,
    include_directories: webrtc_inc,
    c_args : common_cflags + ['-D_GNU_SOURCE']
)

pffft_dep = declare_dependency(
    link_with: libpffft
)

