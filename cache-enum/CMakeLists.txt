cmake_minimum_required(VERSION 2.8)
project(foo LANGUAGES NONE)

set(FOO_CRYPTO "OpenSSL" CACHE STRING "Backend for cryptography")

set_property(CACHE FOO_CRYPTO PROPERTY STRINGS "OpenSSL;Libgcrypt;WinCNG")
