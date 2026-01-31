# BoidsExample
## 概述
UE5.6 基于 Niagara 和 Boids 算法实现的生物集群系统。
## 基础效果

**集群数量 : 500**

https://github.com/user-attachments/assets/b94cd96a-a9d8-4333-96fc-00c820938876

**集群数量 ：1500**

https://github.com/user-attachments/assets/c307779d-bd2f-46d1-9858-67f34447e969

## 使用方法
直接将 BP_BoidsNiagara 拖拽至场景，结合蓝图和 Niagara 参数调整。
## 基本功能
**个体随机目标点**

集群个体会跟随随机目标点进行运动。

https://github.com/user-attachments/assets/830780b5-4746-4333-b19c-11f69a819798

**个体自动避障**

根据 Niagara 全局距离场计算障碍物距离，实现个体自动避障转向。

https://github.com/user-attachments/assets/75fd95a3-cff7-4038-834b-bb1dca900469

**集群自动避障**

接入集群的自动避障。

https://github.com/user-attachments/assets/87b13aee-710c-4762-abaa-a4d226b56579

**鱼群顶点动画**

鱼的动画使用材质的顶点动画实现，使用加速度和转向加速度参数控制摆尾频率和幅度。

https://github.com/user-attachments/assets/42cf24c6-1b7d-4fdb-b8d2-59c3075120a1

**风暴鱼群效果**

可以开启球形力，控制鱼群做环绕圆周运动，实现风暴鱼群效果。

https://github.com/user-attachments/assets/8e1c175d-7dd3-4b78-a1ce-71743d3d7421

可以控制球形力和区域限制参数，实现不同形状的风暴鱼群效果。

https://github.com/user-attachments/assets/16c00be3-d0c6-4a63-9ebd-46c0cc84074c

**躲避捕食者**

开启捕食者后，在接近捕食者一段距离内会加速逃离捕食者。

https://github.com/user-attachments/assets/10b55f5d-e2ef-4a31-9aa4-9e3f310cfaf7

**速度爆发**

开启速度爆发后，集群个体会在随机的间隔时间内快速游动。

**区域限制**

开启区域限制后，可以控制集群的活动范围（比如制作鱼缸的集群效果）。

https://github.com/user-attachments/assets/3d28217e-d967-44e2-be7e-d04b8715fc72

**Boids集群行为控制**

控制 Boids 算法中描述集群的三个行为（跟随、聚集、分离）的参数，实现不同的集群效果。

<img width="551" height="422" alt="image" src="https://github.com/user-attachments/assets/13e721c0-9fda-4804-ad21-92ca3976b814" />

**NeighborGrid3D 领域网格**

使用 Niagara 的 NeighborGrid3D 领域网格优化粒子查询算法，降低个体查询周围粒子运动属性的复杂度。

**接入BAT动画**

使用同一个 Niagara 集群系统接入 BAT 鸟群动画案例。

使用 AimToTexture 插件将骨骼动画转化为静态网格的 BAT 动画（骨骼动画纹理）。

https://github.com/user-attachments/assets/e9703314-0b12-4720-9199-39bfb24365b3

