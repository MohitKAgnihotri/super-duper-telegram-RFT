cmake_minimum_required(VERSION 3.16)
project(super_duper_telegram_RFT C)

set(CMAKE_C_STANDARD 11)

add_executable(rft_client rft_client.c rft_util.c rft_client_util.c rft_client_logging.c)

add_executable(rft_server rft_server.c rft_util.c)

add_executable(test_rft_client_util test_rft_client_util.c rft_util.c rft_client_util.c rft_client_logging.c munit.c )