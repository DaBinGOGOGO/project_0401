## 模型思路
    样本MSE衡量样本间面积差距,样本MSE取自topK的均值
## 执行步骤
#### 1.生成数字矩阵
    运行inference_code.py,在data文件下生成data_matric.npy和node_id.npy文件.
#### 2.生成样本对应的 MSE 矩阵
    运行gen_MSE_matrix.py,在data文件夹下生成
    mse_matrix_torch_20000.npy
    mse_matrix_torch_40000.npy
    mse_matrix_torch_60000.npy
    mse_matrix_torch_80000.npy
    mse_matrix_torch_final.npy
#### 3.生成样本 mark 标记
    运行retain_nodeid.py,在out_data文件夹下生成
    retain_nodeid_20000.npy
    retain_mark_20000.npy
    retain_nodeid_40000.npy
    retain_mark_40000.npy
    retain_nodeid_60000.npy
    retain_mark_60000.npy
    retain_nodeid_80000.npy
    retain_mark_80000.npy
    retain_nodeid_final.npy
    retain_mark_final.npy
#### 4.根据 mark 进行抽样
    运行gen_txt.py,在out_text文件夹在生成chaofanwei_{}.txt

