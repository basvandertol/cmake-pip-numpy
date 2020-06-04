cmake_minimum_required(VERSION 3.1)

project(Numpy)

function(pip_install)
    execute_process("python3", "-m", "pip", "install", "numpy", "--prefix", "${CMAKE_INSTALL_PREFIX}")
endfunction()


install(CODE "pip_install()" )


