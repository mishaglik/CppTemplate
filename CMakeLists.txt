cmake_minimum_required(VERSION 3.14)

project(C3TEMPLATE)

include(cmake/Logging.cmake)
include(cmake/Ccache.cmake)
include(cmake/Helpers.cmake)
include(cmake/CheckCompiler.cmake)
include(cmake/CompileOptions.cmake)
include(cmake/Sanitize.cmake)
include(cmake/Development.cmake)

add_subdirectory(lib)

# Must be after lib not to affect them.
# include(cmake/Werror.cmake)


add_subdirectory(src)