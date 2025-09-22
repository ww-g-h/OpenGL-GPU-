# OpenGL-GPU-
基于OpenGL计算着色器的实时光线追踪渲染系统。

## 项目结构
```
RayTracing/
├── outputs/                             # 渲染结果输出目录
│   └── output1.png ... output16.png   
├── assets/                              # 资源：纹理、HDR、模型
│   ├── earth.jpg
│   ├── wood.png
│   ├── sky_light.hdr
│   ├── sky_night.hdr
│   ├── sky_star.hdr
│   └── models/
├── shaders/                              # GLSL 着色器
│   ├── vertex.vs 
│   └── fragment_1.frag 
├── src/                                  # 应用主程序
│   ├── main.cpp                          # 程序入口：初始化渲染器、相机、场景、开始渲染
│   ├── GenData.cpp                       # 将 BVH/材质/纹理等打包为 GPU 纹理的数据生成器
│   ├── RayTracingRenderer.h/.cpp         # 渲染器封装（窗口/GL/帧缓冲/纹理/着色器/进度/保存）
│   ├── SceneBuilder.h/.cpp               # 场景构建器（多套场景：随机球、贴图、模型）
│   ├── Log.h 
│   ├── glad.c 
│   ├── assimp-vc143-mtd.dll 
├── OpenGl/                               # 引擎/库源码（几何体、材质、BVH、工具等）
│   ├── Include/                          # 公共头文件
│   ├── Src/                              # 对应实现文件
│   └── Libs/                             # 预编译静态库
│       ├── assimp-vc143-mtd.lib
│       ├── glfw3.lib
│       └── libglfw3.a
```
<img width="800" height="600" alt="output16" src="https://github.com/user-attachments/assets/b01ed266-4994-4de8-8662-481030770ee4" />
<img width="800" height="600" alt="output15" src="https://github.com/user-attachments/assets/a9985868-9194-4ef5-84e6-577a9c684cb5" />
<img width="800" height="600" alt="output12" src="https://github.com/user-attachments/assets/7dab8610-8897-41ff-8f5a-1ab9a718a1a6" />
<img width="1280" height="720" alt="output11" src="https://github.com/user-attachments/assets/73b7774f-d415-4ebe-a567-1cbbd395f837" />
<img width="1280" height="720" alt="output5" src="https://github.com/user-attachments/assets/ea868bc8-f649-42b8-9d66-56096b9a6ec6" />

