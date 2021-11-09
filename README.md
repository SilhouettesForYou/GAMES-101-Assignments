## GAMES-101 Assignments

### 旋转与投影

本次作业的任务是填写一个旋转矩阵和一个透视投影矩阵。给定三维下三个点 v<sub>0</sub>(2.0, 0.0, −2.0)，v<sub>1</sub>(0.0, 2.0, −2.0)，v<sub>2</sub>(-2.0, 0.0, −2.0)， 你需要将这三个点的坐标变换为屏幕坐标并在屏幕上绘制出对应的线框三角形 （在代码框架中，我们已经提供了`draw_triangle`函数，所以你只需要去构建变换矩阵即可）。简而言之，我们需要进行模型、视图、投影、视口等变换来将三角形显示在屏幕上。在提供的代码框架中，我们留下了模型变换和投影变换的部分给你去完成。[more>>](/doc/Assignment1/Assignment1.pdf)



### Triangles and Z-buffering

在上次作业中，虽然我们在屏幕上画出一个线框三角形，但这看起来并不是那么的有趣。所以这一次我们继续推一步——在屏幕上画出一个实心三角形，换言之，栅格化一个三角形。上一次作业中，在视口变化之后，我们调用了函数`rasterize_wireframe(const Triangle& t)`。但这一次，你需要自己填写并调用函数 `rasterize_triangle(const Triangle& t)`。[more>>](/doc/Assignment2/Assignment2.pdf)



### Pipeline and Shading

在这次编程任务中，我们会进一步模拟现代图形技术。我们在代码中添加了**Object Loader**（用于加载三维模型），**Vertex Shader**与**Fragment Shader**，并且支持了纹理映射。[more>>](/doc/Assignment3/Assignment3.pdf)



### **Bézier** 曲线

**Bézier**曲线是一种用于计算机图形学的参数曲线。在本次作业中，你需要实现**de Casteljau**算法来绘制由 4 个控制点表示的**Bézier**曲线 （当你正确实现该算法时，你可以支持绘制由更多点来控制的**Bézier**曲线）。[more>>](/doc/Assignment4/Assignment4.pdf)



### 光线与三角形相交

在这部分的课程中，我们将专注于使用光线追踪来渲染图像。在光线追踪中最重要的操作之一就是找到光线与物体的交点。一旦找到光线与物体的交点，就可以执行着色并返回像素颜色。在这次作业中，我们需要实现两个部分：光线的生成和光线与三角的相交。[more>>](/doc/Assignment5/Assignment5.pdf)



### 加速结构

在之前的编程练习中，我们实现了基础的光线追踪算法，具体而言是光线传输、光线与三角形求交。我们采用了这样的方法寻找光线与场景的交点：遍历场景中的所有物体，判断光线是否与它相交。在场景中的物体数量不大时，该做法可以取得良好的结果，但当物体数量增多、模型变得更加复杂，该做法将会变得非常低效。因此，我们需要加速结构来加速求交过程。在本次练习中，我们重点关注物体划分算法**Bounding Volume Hierarchy (BVH)**。本练习要求你实现**Ray-BoundingVolume** 求交与**BVH**查找。[more>>](/doc/Assignment6/Assignment6.pdf)



### 路径追踪

在之前的练习中，我们实现了**Whitted-Style Ray Tracing**算法，并且用**BVH**等加速结构对于求交过程进行了加速。在本次实验中，我们将在上一次实验的基础上实现完整的**Path Tracing**算法。至此，我们已经来到了光线追踪版块的最后一节内容。[more>>](/doc/Assignment7/Assignment7.pdf)



### 质点弹簧系统

本次作业需要预先安装**OpenGL**，**Freetype**还有**RandR**这三个库。[more>>](/doc/assignment8/Assignment8.pdf)