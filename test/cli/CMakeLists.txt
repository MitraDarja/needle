cmake_minimum_required (VERSION 3.9)

add_cli_test (needle_options_test.cpp)
add_cli_test (ibf_options_test.cpp)
target_use_datasources (ibf_options_test FILES exp_01.fasta mini_example.fasta mini_example.header mini_example.minimiser)
add_cli_test (minimiser_options_test.cpp)
target_use_datasources (minimiser_options_test FILES mini_example.fasta)
add_cli_test (estimate_options_test.cpp)
target_use_datasources (estimate_options_test FILES IBF_1 mini_gen.fasta mini_gen2.fasta)
