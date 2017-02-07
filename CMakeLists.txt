
cmake_minimum_required(VERSION 3.7)
project(sqllite)
add_library(sqllite sqlite-amalgamation-3160200/sqlite3.c)
file(COPY sqlite-amalgamation-3160200/sqlite3.h DESTINATION ${CMAKEIFY_REDIST_INCLUDE_DIRECTORY})
