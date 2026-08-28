## 已知 $`n`$ 阶实矩阵 $`\mathbf{A}`$ 可相似对角化，其特征值均非负，待定实矩阵 $`\mathbf{X}`$ 满足 $`r(\mathbf{X})=r(\mathbf{A})`$，$`\mathbf{X}^2=\mathbf{A}`$，求 $`\mathbf{X}`$

设 $`\mathbf{A}`$ 的 $`k_i`$ 重特征值 $`\lambda_i`$ 的线性无关的特征向量为 $`\mathbf{\xi}_{i1},\mathbf{\xi}_{i2},...,\mathbf{\xi}_{ik_i}`$，记 $`\mathbf{\xi}_i=[\mathbf{\xi}_{i1},\mathbf{\xi}_{i2},...,\mathbf{\xi}_{ik_i}]`$，则 $`\mathbf{A}\mathbf{\xi}_i=\lambda_i\mathbf{\xi}_i\ (i\in[1,m])`$

易知 $`\mathbf{A}\mathbf{X}=\mathbf{X}^3=\mathbf{X}\mathbf{A}`$

则 $`\mathbf{A}(\mathbf{X}\mathbf{\xi}_i)=\mathbf{X}(\mathbf{A}\mathbf{\xi}_i)=\mathbf{X}(\lambda_i\mathbf{\xi}_i)=\lambda_i(\mathbf{X}\mathbf{\xi}_i)`$

即 $`\mathbf{X}\mathbf{\xi}_i`$ 各列均为 $`(\lambda_i\mathbf{E}_{n}-\mathbf{A})\mathbf{\alpha}=\mathbf{0}`$ 的解，即 $`\mathbf{X}\mathbf{\xi}_i`$ 各列均可由 $`\mathbf{\xi}_i`$ 的列向量线性表出

则 $`\exists\ k_i`$ 阶方阵 $`\mathbf{Y}_i`$ ，使 $`\mathbf{X}\mathbf{\xi}_i=\mathbf{\xi}_i\mathbf{Y}_i`$

记 $`\mathbf{Y}=diag(\mathbf{Y}_1,\mathbf{Y}_2,...,\mathbf{Y}_m)`$，可逆矩阵 $`\mathbf{P}=[\mathbf{\xi}_1,\mathbf{\xi}_2,...,\mathbf{\xi}_m]`$

则 $`\mathbf{X}\mathbf{P}=[\mathbf{X}\mathbf{\xi}_1,\mathbf{X}\mathbf{\xi}_2,...,\mathbf{X}\mathbf{\xi}_m]=[\mathbf{\xi}_1\mathbf{Y}_1,\mathbf{\xi}_2\mathbf{Y}_2,...,\mathbf{\xi}_m\mathbf{Y}_m]=\mathbf{P}\mathbf{Y}`$

则 $`\mathbf{X}=\mathbf{P}\mathbf{Y}\mathbf{P}^{-1}`$

记 $`\mathbf{\Lambda}=diag(\lambda_1\mathbf{E}_{k_1},\lambda_2\mathbf{E}_{k_2},...,\lambda_m\mathbf{E}_{k_m})`$

则 $`\mathbf{X}^2=\mathbf{P}\mathbf{Y}^2\mathbf{P}^{-1}=\mathbf{A}=\mathbf{P}\mathbf{\Lambda}\mathbf{P}^{-1}`$ 得 $`\mathbf{Y}^2=\mathbf{\Lambda}`$ 即 $`\mathbf{Y}_i^2=\lambda_i\mathbf{E}_{k_i}`$

（1）当 $`\lambda_i>0`$ 时，由 $`\mathbf{Y}_i`$ 特征值 $`\mu_i`$ 满足 $`\mu_i^2=\lambda_i`$ 得 $`\mu_i=\pm\sqrt{\lambda_i}`$

且 $`(\sqrt{\lambda_i}\mathbf{E}_{k_i}-\mathbf{Y}_i)(-\sqrt{\lambda_i}\mathbf{E}_{k_i}-\mathbf{Y}_i)=\mathbf{O}`$

得 $`k_i=r(2\sqrt{\lambda_i}\mathbf{E}_{k_i})=r[\sqrt{\lambda_i}\mathbf{E}_{k_i}-\mathbf{Y}_i-(-\sqrt{\lambda_i}\mathbf{E}_{k_i}-\mathbf{Y}_i)]\le r(\sqrt{\lambda_i}\mathbf{E}_{k_i}-\mathbf{Y}_i)+r(-\sqrt{\lambda_i}\mathbf{E}_{k_i}-\mathbf{Y}_i)\le k_i`$

即 $`r(\sqrt{\lambda_i}\mathbf{E}_{k_i}-\mathbf{Y}_i)+r(-\sqrt{\lambda_i}\mathbf{E}_{k_i}-\mathbf{Y}_i)=k_i`$

记 $`p_i=r(\sqrt{\lambda_i}\mathbf{E}_{k_i}-\mathbf{Y}_i)\in[0,k_i]`$，则 $`r(-\sqrt{\lambda_i}\mathbf{E}_{k_i}-\mathbf{Y}_i)=k_i-p_i`$

则 $`\mathbf{Y}_i`$ 的特征值 $`\sqrt{\lambda_i}`$、$`-\sqrt{\lambda_i}`$ 分别有 $`k_i-p_i`$、$`k_i-(k_i-p_i)=p_i`$ 个线性无关的特征向量

则 $`\mathbf{Y}_i`$ 有 $`k_i-p_i+p_i=k_i`$ 个线性无关的特征向量

记 $`\mathbf{D}_i=diag(\sqrt{\lambda_i}\mathbf{E}_{k_i-p_i},-\sqrt{\lambda_i}\mathbf{E}_{p_i})`$，则 $`\exists\ k_i`$ 阶可逆矩阵 $`\mathbf{R}_i`$，使 $`\mathbf{Y}_i=\mathbf{R}_i\mathbf{D}_i\mathbf{R}_i^{-1}`$

（2）当 $`\lambda_i=0`$ 时，设 $`\mathbf{\beta}`$ 为 $`\mathbf{X}\mathbf{\beta}=\mathbf{0}`$ 的解

则 $`\mathbf{A}\mathbf{\beta}=\mathbf{X}(\mathbf{X}\mathbf{\beta})=\mathbf{0}`$，即 $`\mathbf{\beta}`$ 也为 $`\mathbf{A}\mathbf{\beta}=\mathbf{0}`$ 的解

即 $`\mathbf{A}\mathbf{\beta}=\mathbf{0}`$ 的解空间包含 $`\mathbf{X}\mathbf{\beta}=\mathbf{0}`$ 的解空间

由 $`r(\mathbf{X})=r(\mathbf{A})`$ 得 $`\mathbf{X}\mathbf{\beta}=\mathbf{0}`$ 和 $`\mathbf{A}\mathbf{\beta}=\mathbf{0}`$ 的基础解系的向量个数（维度）相等

则 $`\mathbf{X}\mathbf{\beta}=\mathbf{0}`$ 和 $`\mathbf{A}\mathbf{\beta}=\mathbf{0}`$ 同解

则 $`\mathbf{X}\mathbf{\xi}_i=\mathbf{O}=\mathbf{\xi}_i\mathbf{Y}_i`$ 得 $`\mathbf{Y}_i=\mathbf{O}`$，则取 $`p_i=0`$，$`\mathbf{D}_i=\mathbf{O}`$，$`\mathbf{R}_i=\mathbf{E}_{k_i}`$

记 $`\mathbf{D}=diag(\mathbf{D}_1,\mathbf{D}_2,...,\mathbf{D}_m)`$，$`\mathbf{R}=diag(\mathbf{R}_1,\mathbf{R}_2,...,\mathbf{R}_m)`$，则 $`\mathbf{Y}=\mathbf{R}\mathbf{D}\mathbf{R}^{-1}`$

则 $`|\mathbf{Y}_i|=(\sqrt{\lambda_i})^{k_i-p_i}(-\sqrt{\lambda_i})^{p_i}=(-1)^{p_i}(\sqrt{\lambda_i})^{k_i}`$

则 $`|\mathbf{X}|=|\mathbf{Y}|=\prod\limits_{i=1}^{m}|\mathbf{Y}_i|=(-1)^{\sum\limits^{m}_{i=1}{p_i}}\sqrt{\prod\limits^{m}_{i=1}\lambda_i^{k_i}}=(-1)^{\sum\limits^{m}_{i=1}{p_i}}\sqrt{|\mathbf{A}|}`$

则 $`tr(\mathbf{X})=tr(\mathbf{Y})=\sum\limits_{i=1}^{m}(k_i-p_i)\sqrt{\lambda_i}+p_i(-\sqrt{\lambda_i})=\sum\limits_{i=1}^{m}(k_i-2p_i)\sqrt{\lambda_i}`$

则 $`\mathbf{X}^2=\mathbf{A}`$ 的解 $`\mathbf{X}=\mathbf{P}(\mathbf{R}\mathbf{D}\mathbf{R}^{-1})\mathbf{P}^{-1}=(\mathbf{P}\mathbf{R})\mathbf{D}(\mathbf{P}\mathbf{R})^{-1}`$

其中，$`\mathbf{R}`$ 为待定分块对角可逆矩阵，但满足上述结论

可结合其他条件确定 $`p_i`$，从而排除大部分解：

- 若 $`\mathbf{A}`$ 对称，$`\mathbf{X}`$ 半正定，则 $`\lambda_{\mathbf{X}}=\lambda_{\mathbf{Y}}\ge 0`$ 即 $`\mu_i\ge 0`$ 得 $`p_i=0`$ 即 $`\mathbf{D}_i=\sqrt{\lambda_i}\mathbf{E}_{k_i}`$，则 $`\mathbf{Y}_i=\mathbf{R}_i\mathbf{D}_i\mathbf{R}_i^{-1}=\mathbf{D}_i`$，则 $`\mathbf{X}=\mathbf{P}diag(\sqrt{\lambda_1}\mathbf{E}_{k_1},\sqrt{\lambda_2}\mathbf{E}_{k_2},...,\sqrt{\lambda_m}\mathbf{E}_{k_m})\mathbf{P}^{-1}`$ 唯一

- 若 $`k_i\equiv 1`$ 即 $`\mathbf{A}`$ 特征值互异，则 $`p_i\in\{0,1\}`$，由 $`\mathbf{Y}_i^2=[\lambda_i]`$ 得 $`\mathbf{Y}_i=[\pm\sqrt{\lambda_i}]`$，则 $`\mathbf{X}=\mathbf{P}diag(\pm\sqrt{\lambda_1},\pm\sqrt{\lambda_2},...,\pm\sqrt{\lambda_n})\mathbf{P}^{-1}`$ 有 $`2^{r(\mathbf{A})}`$ 个解

- 设 $`f(x)`$ 为多项式函数，若 $`\mathbf{X}=f(\mathbf{A})`$，则 $`\mathbf{Y}=\mathbf{P}^{-1}\mathbf{X}\mathbf{P}=\mathbf{P}^{-1}f(\mathbf{A})\mathbf{P}=f(\mathbf{\Lambda})`$，则 $`\mu_i=f(\lambda_i)`$ 唯一，即 $`\mathbf{Y}_i`$ 内特征值同号，即 $`p_i\in\{0,k_i\}`$
