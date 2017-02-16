SET(PROJ_NAME "Cuisinez_avec_git")
PROJECT(${PROJ_NAME})


SET(${PROJ_NAME}_DOCS commit.md)

SET(${PROJ_NAME}_TEMPLATE "--template=${CMAKE_SOURCE_DIR}/github-markdown-css/github-markdown.css")

ADD_DOCUMENT(
    ${PROJ_NAME}.pdf
    SOURCES             ${${PROJ_NAME}_DOCS}
    PANDOC_DIRECTIVES   ${PANDOC_PDF_CONFIG} ${${PROJ_NAME}_TEMPLATE}
    PRODUCT_DIRECTORY   ${CMAKE_SOURCE_DIR}/doc
)
