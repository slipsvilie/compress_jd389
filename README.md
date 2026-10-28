# compress_jd389

**追溯模型压缩工程师·算子融合的收益边界里每一份贡献来自哪里。**

`compress_jd389` —— 统计各来源片段的贡献量与占比，标出模型压缩工程师·算子融合的收益边界上最主要的来源

- 零依赖，Python 3.10+ 标准库即可运行
- 单文件，`compress_jd389.py` 拷走就能用
- 不联网、不写文件

## 对应的岗位

- 目标岗位：**微软 · 实习模型压缩工程师**
- 技能主线：模型压缩、推理加速、PyTorch、ONNX
- 领域标签：大模型推理、AI基础设施
- 研究方向：模型压缩工程师·算子融合的收益边界

工具里的规则表就是照着上面这条岗位要求建的——每条规则都挂在技能线或领域标签上，命中时能指回具体要求。

<!-- ipos:install -->
## 安装

零依赖，Python 3.10+ 即可：

```bash
pip install slipsvilie-compress_jd389
```

装完直接用命令名调用：

```bash
compress_jd389 --help
```

也可以不用安装，直接把 `compress_jd389.py` 拷走用——它只依赖标准库。

## 为什么需要它

贡献占比按字符量算而不是按出现次数，避免长句主导统计

它遵守下面几条自己定的规矩：

1. **只报告能定位到具体位置的结论**，不做语义猜测。
2. **规则表公开**，每条命中都能对应到岗位要求的一条明示规则。
3. **输入为空或格式不对时明确报错**，不静默返回空结果。

## 用法

```bash
python compress_jd389.py --file input.txt
python compress_jd389.py --text "示例内容"
python compress_jd389.py --file input.txt --json
```

加 `--json` 可以拿到机器可读的结果，便于接到流水线里。

## 已知局限

- 计数按字面 token 统计，不做词形还原。
- 只报告分布，不判断该保留哪些。

## 跑测试

```bash
python test_compress_jd389.py
```

测试用独立的断言与临时数据，不污染工作目录。

## 来源与参考

- Python 标准库文档：<https://docs.python.org/3/>
- GitHub 仓库：<https://github.com/slipsvilie/compress_jd389>

---

## 关于作者

slipsvilie 做模型压缩工程师·算子融合的收益边界相关的问题，方向对标微软的实习模型压缩工程师岗位。这个工具先替你回答一个具体问题，再谈别的。

- 个人主页：<https://slipsvilie.github.io>
- 仓库：<https://github.com/slipsvilie/compress_jd389>

## 许可

MIT，见 [LICENSE](LICENSE)。
