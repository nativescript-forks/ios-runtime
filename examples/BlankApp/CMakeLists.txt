    cmake_policy(VERSION 3.1)
set(RESOURCES app)

include(CreateNativeScriptApp)
CreateNativeScriptApp(BlankApp main.m "${INFO_PLIST_TEMPLATE}" "${RESOURCES}")

include(LinkTestFixtures)
LinkTestFixtures(BlankApp)
