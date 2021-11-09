## GAMES-101 Assignments

### 旋转与投影

​		本次作业的任务是填写一个旋转矩阵和一个透视投影矩阵。给定三维下三个点 `v<sub>0</sub>(2.0, 0.0, −2.0)`，`v<sub>1</sub>(0.0, 2.0, −2.0)`，`v<sub>2</sub>(-2.0, 0.0, −2.0)`， 你需要将这三个点的坐标变换为屏幕坐标并在屏幕上绘制出对应的线框三角形 （在代码框架中，我们已经提供了`draw_triangle`函数，所以你只需要去构建变换矩阵即可）。简而言之，我们需要进行模型、视图、投影、视口等变换来将三角形显示在屏幕上。在提供的代码框架中，我们留下了模型变换和投影变换的部分给你去完成。[more>>](/doc/Assignment1/Assignment1.pdf)



### Triangles and Z-buffering

​		在上次作业中，虽然我们在屏幕上画出一个线框三角形，但这看起来并不是那么的有趣。所以这一次我们继续推一步——在屏幕上画出一个实心三角形，换言之，栅格化一个三角形。上一次作业中，在视口变化之后，我们调用了函数`rasterize_wireframe(const Triangle& t)`。但这一次，你需要自己填写并调用函数 `rasterize_triangle(const Triangle& t)`。[more>>](/doc/Assignment2/Assignment2.pdf)

