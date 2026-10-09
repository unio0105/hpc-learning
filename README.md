# hpc-learning

高性能计算（HPC）学习记录仓库。用来存放学习笔记、实验代码、跑过的脚本和踩坑记录。

## 我想做什么

- [ ] 理解 HPC 基本概念：并行计算、MPI、OpenMP、GPU 加速
- [ ] 在本地和服务器上编译运行 C/C++ / Fortran 并行程序
- [ ] 学习 SLURM / PBS 等作业调度系统的使用
- [ ] 记录每一次实验的环境、命令和结果，方便复现

## 当前环境

| 项目 | 配置 |
|------|------|
| 本地系统 | Windows 11 |
| Git 版本 | 2.55.0.windows.5 |
| 编译器 | （待安装：MSYS2 / MinGW-w64 或 WSL） |
| 远程集群 | （待补充：学校 / 实验室 HPC 集群地址） |

## 目录结构（计划）

```
hpc-learning/
├── README.md           # 本文件
├── notes/              # 学习笔记（Markdown）
├── code/              # 示例代码
│   ├── mpi/           # MPI 并行程序
│   ├── openmp/        # OpenMP 共享内存并行
│   └── cuda/          # GPU 程序（如有条件）
├── scripts/            # 提交脚本、编译脚本
└── results/           # 实验结果输出
```

## 怎样运行项目

### 1. 克隆仓库

```bash
git clone https://github.com/unio0105/hpc-learning.git
cd hpc-learning
```

### 2. 配置 Git 署名（第一次）

```bash
git config user.name  "你的名字"
git config user.email "你的GitHub noreply邮箱"
```

### 3. 编译并运行示例（以后补充）

```bash
cd code/openmp/hello
g++ -fopenmp hello.cpp -o hello
./hello
```

## 自检清单

- [x] GitHub 账号已注册并验证邮箱
- [x] 本仓库已在 GitHub 上创建（含 README）
- [x] 本地 `git clone` 能成功
- [ ] 修改 README 后 `git add / commit / push` 流程跑通
- [ ] `.gitignore` 已排除 `.env`、密钥文件、编译产物
