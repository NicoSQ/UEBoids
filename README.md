# BoidsExample
## 概述
UE5.6 基于 Niagara 和 Boids 算法实现的生物集群系统。
## 基础效果

**集群数量 : 500**

https://github.com/user-attachments/assets/eaf50334-814c-4d33-b982-6685219a0445

**集群数量 ：1500**

https://github.com/user-attachments/assets/8b0b4f9f-5798-4fce-9b34-4ef3df3bdcbe

## 使用方法
直接将 BP_BoidsNiagara 拖拽至场景，结合蓝图和 Niagara 参数调整。
## 基本功能
**个体随机目标点**

集群个体会跟随随机目标点进行运动。

https://github.com/user-attachments/assets/700b7ccc-3de1-4702-a59b-6c807ff51908

**个体自动避障**

根据 Niagara 全局距离场计算障碍物距离，实现个体自动避障转向。

https://github.com/user-attachments/assets/b798aa8b-4d44-4fbe-9fd8-0b2f24dc9ab7

**集群自动避障**

接入集群的自动避障。

https://github.com/user-attachments/assets/2a6c62ba-7dc3-4ee6-bef8-bfb8866a36ed

**鱼群顶点动画**

鱼的动画使用材质的顶点动画实现，使用加速度和转向加速度参数控制摆尾频率和幅度。

https://github.com/user-attachments/assets/7b2bda9e-139c-48be-a74b-564cf8ef661b

**风暴鱼群效果**

可以开启球形力，控制鱼群做环绕圆周运动，实现风暴鱼群效果。

https://github.com/user-attachments/assets/a5426930-5dfd-47f9-b560-f55dfd97b1da

可以控制球形力和区域限制参数，实现不同形状的风暴鱼群效果。

https://github.com/user-attachments/assets/fb883bf5-cbf1-4a25-8a69-6d4106aa9998

**躲避捕食者**

开启捕食者后，在接近捕食者一段距离内会加速逃离捕食者。

https://github.com/user-attachments/assets/ac10b6a2-ca0f-40d9-9fd5-0a6298c32e6e

**速度爆发**

开启速度爆发后，集群个体会在随机的间隔时间内快速游动。

**区域限制**

开启区域限制后，可以控制集群的活动范围（比如制作鱼缸的集群效果）。

https://github.com/user-attachments/assets/516ef150-00d3-43eb-89c5-1eeb7fe6914c

**Boids集群行为控制**

控制 Boids 算法中描述集群的三个行为（跟随、聚集、分离）的参数，实现不同的集群效果。

<img width="404" height="401" alt="image" src="https://github.com/user-attachments/assets/dd001d28-6ec3-4e12-b259-f53394566929" />

**NeighborGrid3D 领域网格**

使用 Niagara 的 NeighborGrid3D 领域网格优化粒子查询算法，降低个体查询周围粒子运动属性的复杂度。

**接入BAT动画**

使用同一个 Niagara 集群系统接入 BAT 鸟群动画案例。

使用 AimToTexture 插件将骨骼动画转化为静态网格的 BAT 动画（骨骼动画纹理）。

https://github.com/user-attachments/assets/853a461b-7cef-4f5a-a92f-7375bdebbc90
