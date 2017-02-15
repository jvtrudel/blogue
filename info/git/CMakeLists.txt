cmake_minimum_required(VERSION 3.0)

project(jvtrudel_git_documentation)

find_package(Git)

# get pandocology
# problèmes à résoudres...
#   - ne pas downloader à chaque fois
#   - mettre dans le répertoire sources et non dans le build
# solution1 :
#    - Si le répertoire n'existe pas, on applique clone
#    - si il existe, on pull
  execute_process(COMMAND
      ${GIT_EXECUTABLE} clone https://github.com/jeetsukumaran/cmake-pandocology.git ${CMAKE_CURRENT_SOURCE_DIR}/cmake-pandocology
      )
LIST(APPEND CMAKE_MODULE_PATH "${CMAKE_SOURCE_DIR}/cmake-pandocology")

include(pandocology)


add_document(
    docu.rtf
    SOURCES fork.md

)
