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
![1](https://github.com/user-attachments/assets/55908f11-62a2-4b29-90af-6145ab702658)

