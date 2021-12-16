# 定义 stbiw 库
add_library(stbiw SHARED stbiw.cpp)
# 允许通过尖括号导入头文件 <stb_image_write.h>
target_include_directories(stbiw PUBLIC .)
