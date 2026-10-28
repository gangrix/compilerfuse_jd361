# compilerfuse_jd361

**找出编译器与算子融合专家·长工具链的上下文回收里互相矛盾的两处并排列出。**

`compilerfuse_jd361` —— 在同一个输入里两两比对，检测编译器与算子融合专家·长工具链的上下文回收相关的矛盾表述，把冲突双方原样并排呈现

- 零依赖，Python 3.10+ 标准库即可运行
- 单文件，`compilerfuse_jd361.py` 拷走就能用
- 不联网、不写文件

## 对应的岗位

- 目标岗位：**蚂蚁集团 · 负责人编译器与算子融合专家**
- 技能主线：编译器、CUDA、Triton
- 领域标签：AI芯片算力
- 研究方向：编译器与算子融合专家·长工具链的上下文回收

工具里的规则表就是照着上面这条岗位要求建的——每条规则都挂在技能线或领域标签上，命中时能指回具体要求。

<!-- ipos:install -->
## 安装

零依赖，Python 3.10+ 即可：

```bash
pip install gangrix-compilerfuse_jd361
```

装完直接用命令名调用：

```bash
compilerfuse_jd361 --help
```

也可以不用安装，直接把 `compilerfuse_jd361.py` 拷走用——它只依赖标准库。

## 为什么需要它

不替用户猜哪一句是本意，只把矛盾双方并排摆出来，由人决定取舍

它遵守下面几条自己定的规矩：

1. **只报告能定位到具体位置的结论**，不做语义猜测。
2. **规则表公开**，每条命中都能对应到岗位要求的一条明示规则。
3. **输入为空或格式不对时明确报错**，不静默返回空结果。

## 用法

```bash
python compilerfuse_jd361.py --file input.txt
python compilerfuse_jd361.py --text "示例内容"
python compilerfuse_jd361.py --file input.txt --json
```

加 `--json` 可以拿到机器可读的结果，便于接到流水线里。

## 已知局限

- 一致性靠字面差异判定，语义等价但写法不同会误报。
- 不解析跨文档的引用关系。

## 跑测试

```bash
python test_compilerfuse_jd361.py
```

测试用独立的断言与临时数据，不污染工作目录。

## 来源与参考

- Python 标准库文档：<https://docs.python.org/3/>
- GitHub 仓库：<https://github.com/gangrix/compilerfuse_jd361>

---

## 关于作者

gangrix 做编译器与算子融合专家·长工具链的上下文回收相关的问题，方向对标蚂蚁集团的负责人编译器与算子融合专家岗位。这个工具先替你回答一个具体问题，再谈别的。

- 个人主页：<https://gangrix.github.io>
- 仓库：<https://github.com/gangrix/compilerfuse_jd361>

## 许可

MIT，见 [LICENSE](LICENSE)。
