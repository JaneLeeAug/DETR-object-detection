# 2D Gaussian Splatting (2DGS)
### 2024 Fall / DIP Group_09

###3D Reconstruction of Jupiter Using Gaussian Splatting
## 環境設置與執行

### 1. 2DGS 執行環境 (Colab):
```
nvcc: NVIDIA (R) Cuda compiler driver
Copyright (c) 2005-2023 NVIDIA Corporation
Built on Tue_Aug_15_22:02:13_PDT_2023
Cuda compilation tools, release 12.2, V12.2.140
Build cuda_12.2.r12.2/compiler.33191640_0
```

### 2. 2DGS 資料與程式碼
- [共享資料夾與程式碼下載](https://drive.google.com/drive/folders/1fMcdwrM9AHdz3TGHmQf-YlDe8rdcjxye?usp=sharing)

### 3. Colab 執行網址
- [執行 2DGS 測試蘋果和香蕉的圖像](https://colab.research.google.com/drive/1KGf5ooBJOHNDnFGNY0lHbiI6hvmMewsF?usp=sharing)

### 4. 蘋果與香蕉圖像路徑
- **香蕉圖像**：`2d-gaussian-splatting/banana/input`
- **蘋果圖像**：`2d-gaussian-splatting/apple/input`

### 5. 訓練成果 (fuse.ply 和 fuse_post.ply)
- **香蕉成果**：`2d-gaussian-splatting/output/banana/train/ours_30000`
- **蘋果成果**：`2d-gaussian-splatting/output/apple/train/ours_30000`

## Non-2DGS 技術

### 1. Non-2DGS 技術程式碼
- **JUPTER-image.py** 位於 `source` 資料夾中，需在 Python 3 環境執行。

### 2. 資料與成果
- **木星圖像**：`source/enhance`
- **產生的 3D 圖像**：`jupiter_3d_reconstruction2.png`
- **PLY 格式圖像**：`jupiter_sphere_from_enhance.ply` (從 `jupiter_3d_reconstruction2.png` 轉化而來)

### 3. 相關 GIF 圖檔
- 所有 GIF 圖檔位於 `source` 資料夾中。
