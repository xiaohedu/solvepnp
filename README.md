# solvepnp
solvepnp测距，提前push世界坐标，根据图像坐标求解pnp，使用ITERATIVE方法，（P3P结果存在较大误差），结果重投影回图像坐标系，判断误差，测试误差在0.5像素内。

Note:


//相机系到世界系的三轴旋转欧拉角，相机坐标系照此旋转后可以与世界坐标系完全平行。
	//旋转顺序为z、y、x
	Theta_C2W.z = thetaz;
	Theta_C2W.y = thetay;
	Theta_C2W.x = thetax;
