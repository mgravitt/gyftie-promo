project(gyftiepromo)

set(EOSIO_WASM_OLD_BEHAVIOR "Off")
find_package(eosio.cdt)

add_contract( gyftietoken gyftietoken gyftietoken.cpp )
target_include_directories( gyftietoken PUBLIC ${CMAKE_SOURCE_DIR}/../include )
