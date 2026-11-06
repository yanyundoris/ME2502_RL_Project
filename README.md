# ME2502_RL_Project

ME2502 Reinforcement Learning Course Project

## DecisionRL

**DecisionRL: Enhancing Decision Calibration through Reinforcement Learning**
研究通过监督微调（SFT）与 Reinforcement Learning for Calibrated Decisions（RLCD）
改善语言模型的决策准确性和概率校准，探索 ModernBERT、EuroBERT 等编码器骨干及 RLCD 优化策略。
评估指标包括 Accuracy、Macro F1、Expected Calibration Error（ECE）和 Brier Score。

团队成员：Taihua Chen、Yanyun LIU。

## 项目提案

- LaTeX 源文件：[materials/rlcd_proposal.tex](materials/rlcd_proposal.tex)
- 编译后的 PDF：[materials/build/rlcd_proposal.pdf](materials/build/rlcd_proposal.pdf)

## LaTeX 编译

使用 [Tectonic](https://tectonic-typesetting.github.io/book/latest/installation/)，
首次编译会联网下载所需的 TeX 宏包，后续复用本机缓存。macOS 可通过 Homebrew 安装：

```sh
brew install tectonic
```

在项目根目录执行：

```sh
mkdir -p materials/build
tectonic --synctex --keep-logs --outdir materials/build materials/rlcd_proposal.tex
```

输出为 `materials/build/rlcd_proposal.pdf`，编译日志为同目录下的 `rlcd_proposal.log`。
修改源文件后重新运行上述命令即可更新 PDF。

## 文件跟踪规则

除已跟踪的 README 和 `.gitignore` 外，仓库只新增 `.tex` 与 `.pdf` 文件。
编译日志、SyncTeX 文件和本地编辑器配置会被忽略。
