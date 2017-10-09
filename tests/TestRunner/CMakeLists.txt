    cmake_policy(VERSION 3.1)
set(RESOURCES app)

include(CreateNativeScriptApp)
CreateNativeScriptApp(TestRunner "${MAIN_TEMPLATE}" "${INFO_PLIST_TEMPLATE}" "${RESOURCES}")

include(LinkTestFixtures)
LinkTestFixtures(TestRunner)
