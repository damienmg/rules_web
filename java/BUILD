# Copyright 2016 Google Inc.
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
#
################################################################################
#
load("//web:web.bzl", "web_test_named_executable")

java_binary(
    name = "SeleniumServer",
    main_class = "org.openqa.grid.selenium.GridLauncherV3",
    runtime_deps = ["@org_seleniumhq_server//jar"],
)

web_test_named_executable(
    name = "SELENIUM_SERVER",
    executable = ":SeleniumServer",
    visibility = ["//browsers:__pkg__"],
)
