noinst_LTLIBRARIES = libbase.la

noinst_HEADERS = array_view.h \
		 arraysize.h \
		 atomicops.h \
		 basictypes.h \
		 constructormagic.h \
		 deprecation.h \
		 function_view.h \
		 gtest_prod_util.h \
		 ignore_wundef.h \
		 protobuf_utils.h \
		 safe_conversions.h \
		 safe_conversions_impl.h \
		 sanitizer.h \
		 swap_queue.h \
		 template_util.h \
		 thread_annotations.h \
		 trace_event.h \
		 type_traits.h

libbase_la_SOURCES = criticalsection.cc \
		     criticalsection.h \
		     checks.cc \
		     checks.h \
		     event.cc \
		     event.h \
		     event_tracer.cc \
		     event_tracer.h \
		     logging.cc \
		     logging.h \
		     optional.cc \
		     optional.h \
		     platform_thread.cc \
		     platform_thread_types.h \
		     platform_file.cc \
		     platform_file.h \
		     race_checker.cc \
		     race_checker.h \
		     stringencode.cc \
		     stringencode.h \
		     stringutils.cc \
		     stringutils.h \
		     thread_checker.h \
		     thread_checker_impl.cc \
		     thread_checker_impl.h \
		     timeutils.cc \
		     timeutils.h

libbase_la_CXXFLAGS = $(AM_CXXFLAGS) $(COMMON_CXXFLAGS)

EXTRA_DIST = BUILD.gn
