noinst_LTLIBRARIES = libsystem_wrappers.la

noinst_HEADERS = include/aligned_array.h \
		 include/asm_defines.h \
		 include/compile_assert_c.h \
		 include/event_wrapper.h \
		 include/static_instance.h

libsystem_wrappers_la_SOURCES = include/aligned_malloc.h \
				include/cpu_features_wrapper.h \
				include/file_wrapper.h \
				include/metrics.h \
				include/rw_lock_wrapper.h \
				include/sleep.h \
				include/thread_wrapper.h \
				include/trace.h \
				source/aligned_malloc.cc \
				source/cpu_features.cc \
				source/event.cc \
				source/event_timer_posix.h \
				source/event_timer_win.h \
				source/file_impl.cc \
				source/metrics_default.cc \
				source/metrics_default.h \
				source/rw_lock.cc \
				source/rw_lock_posix.h \
				source/rw_lock_win.h \
				source/sleep.cc \
				source/trace_impl.cc \
				source/trace_impl.h \
				source/trace_posix.h \
				source/trace_win.h

EXTRA_DIST = BUILD.gn

if HAVE_POSIX
libsystem_wrappers_la_SOURCES += source/event_timer_posix.cc \
				 source/rw_lock_posix.cc \
				 source/trace_posix.cc
else
EXTRA_DIST += source/event_timer_posix.cc \
	      source/rw_lock_posix.cc \
	      source/trace_posix.cc
endif

if HAVE_WIN
libsystem_wrappers_la_SOURCES += include/fix_interlocked_exchange_pointer_win.h \
				 source/event_timer_win.cc \
				 source/rw_lock_win.cc \
				 source/rw_lock_win.cc \
				 source/trace_win.cc
else
EXTRA_DIST += include/fix_interlocked_exchange_pointer_win.h \
	      source/event_timer_win.cc \
	      source/rw_lock_generic.cc \
	      source/rw_lock_win.cc \
	      source/trace_win.cc
endif

libsystem_wrappers_la_CXXFLAGS = $(AM_CXXFLAGS) $(COMMON_CXXFLAGS)
