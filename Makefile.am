SUBDIRS = webrtc

pkgconfigdir = $(libdir)/pkgconfig
pkgconfig_DATA = webrtc-audio-processing.pc

webrtcincludedir = $(includedir)/webrtc_audio_processing
nobase_webrtcinclude_HEADERS = webrtc/api/video/video_rotation.h \
			       webrtc/api/video/video_content_type.h \
			       webrtc/base/arraysize.h \
			       webrtc/base/array_view.h \
			       webrtc/base/checks.h \
			       webrtc/base/constructormagic.h \
			       webrtc/base/basictypes.h \
			       webrtc/base/optional.h \
			       webrtc/base/platform_file.h \
			       webrtc/base/safe_compare.h \
			       webrtc/base/sanitizer.h \
			       webrtc/base/type_traits.h \
			       webrtc/common_types.h \
			       webrtc/typedefs.h \
			       webrtc/modules/audio_processing/beamformer/array_util.h \
			       webrtc/modules/audio_processing/include/audio_processing.h \
			       webrtc/modules/audio_processing/include/config.h \
			       webrtc/modules/include/module_common_types.h \
			       webrtc/system_wrappers/include/trace.h

EXTRA_DIST = NEWS \
	     README.md \
	     UPDATING.md
