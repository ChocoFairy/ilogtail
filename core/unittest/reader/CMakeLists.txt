# Copyright 2022 iLogtail Authors
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
#      http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.

cmake_minimum_required(VERSION 2.9)
project(log_file_reader_unittest)

add_executable(log_file_reader_deleted_file_unittest DeletedFileUnittest.cpp)
target_link_libraries(log_file_reader_deleted_file_unittest unittest_base)

add_executable(log_file_reader_unittest LogFileReaderUnittest.cpp)
target_link_libraries(log_file_reader_unittest unittest_base)
