set(SRC_HEADERS )

set(SRC_SOURCES main.cpp)

find_package(tree-sitter REQUIRED)
find_package(spdlog CONFIG)

add_executable(SQLSP ${SRC_HEADERS} ${SRC_SOURCES})

target_link_libraries(SQLSP PRIVATE tree-sitter::tree-sitter spdlog::spdlog)