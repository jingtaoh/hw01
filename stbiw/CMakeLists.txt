# Define stbiw library
add_library(stbiw SHARED stbiw.cpp)
# 允许通过尖括号导入头文件 <stb_image_write.h>
target_include_directories(stbiw PUBLIC .)
# 保证仅在 stbiw.cpp 中 define 一次
target_compile_definitions(stbiw PRIVATE STB_IMAGE_WRITE_IMPLEMENTATION)