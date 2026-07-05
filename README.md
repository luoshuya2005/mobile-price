# 手机市场价格区间预测与用户画像分析

## 项目背景
随着智能手机市场的饱和，厂商需要更精准地定位不同价格区间的用户群体。本项目基于 2000 款手机的配置参数（如 RAM、电池容量、摄像头等），构建机器学习模型，实现手机价格的自动分类，并挖掘不同价位段的核心竞争力特征。

## 技术栈
*   **数据处理**：Python (Pandas, NumPy)
*   **数据可视化**：Matplotlib, Seaborn
*   **机器学习**：Scikit-learn (SVM, Random Forest, XGBoost)
*   **开发环境**：Jupyter Notebook

## 核心成果
*   **数据清洗**：处理了 2000+ 条原始数据，解决了缺失值与异常值问题。
*   **探索性分析 (EDA)**：通过热力图和分布图，发现 RAM 大小和电池容量是影响价格的最关键因素。
*   **模型构建**：对比了 5 种主流分类算法，**SVM 模型准确率高达 95.75%**，显著优于传统模型。
*   **业务洞察**：识别出高端机与低端机在硬件配置上的关键阈值，为产品定价策略提供数据支持。

## 关键图表
<!-- 示例：![Feature Importance](results/feature_importance.png) -->

## 运行方式
由于本项目主要展示分析过程，推荐直接在浏览器中查看：

1.  **在线预览**（推荐）：
    点击仓库中的 `mobile_price_analysis.ipynb` 文件，GitHub 会自动渲染展示。
2.  **本地运行**：
    ```bash
    # 安装依赖
    pip install pandas numpy scikit-learn matplotlib seaborn jupyter
    # 启动 Notebook
    jupyter notebook
    ```
    业务结论摘要
    结论一：RAM 对价格的影响权重最高（约 35%），是用户付费意愿最强的指标。
    结论二：当电池容量超过 4000mAh 时，对价格的边际贡献递减。
    建议：针对中端市场（2000-3000元），应优先保障 RAM 配置，而非盲目增加电池容量。
