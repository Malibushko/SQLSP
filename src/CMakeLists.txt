set(SRC_HEADERS )

set(SRC_SOURCES main.cpp)

find_package(tree-sitter REQUIRED)

add_executable(SQLSP ${SRC_HEADERS} ${SRC_SOURCES})

target_link_libraries(SQLSP PRIVATE tree-sitter::tree-sitter)