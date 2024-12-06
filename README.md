# 开源AI手册

这个仓库包含了社区驱动的AI应用示例，展示了如何使用开源工具和模型解决各种任务。

## 如何贡献

欢迎大家贡献自己的力量，我们非常重视每一位贡献者！你可以通过以下方式为[开源AI手册](https://huggingface.co/learn/cookbook/index)做出贡献：

* 在[GitHub Issues](https://github.com/huggingface/cookbook/issues)提交你希望看到的示例或教程的想法。
* 提交新的笔记本，包含实用的AI示例。
* 改进已有的示例，修复问题或拼写错误。

在贡献之前，请检查一下当前的[开放问题](https://github.com/huggingface/cookbook/issues)和[拉取请求](https://github.com/huggingface/cookbook/pulls)，避免重复劳动。

贡献完成后，你可以申请加入[这个组织](https://huggingface.co/huggingcooks)，获得徽章奖励。 🏅

### 一个好的Cookbook笔记本应具备哪些特点？

我们认为，如果Jupyter笔记本具有以下特点，AI手册会对社区最有帮助：

* *实用性*：笔记本应展示一个完整的项目或AI开发的某个方面。最好是面向真实场景的应用，但不要过于复杂。清晰地说明目标、挑战和解决步骤。
* *使用开源工具和模型*：利用开源库、数据集和许可宽松的预训练模型。并在笔记本中提供所用资源的链接。
* *简明易懂*：确保笔记本内容简洁清晰，没有语法错误。用友好的语气说明你解决问题的步骤、遇到的挑战以及可能的其他方法。
* *无运行错误*：测试笔记本，确保没有运行时错误。
* *有新增内容*：在提交前，检查现有笔记本，确认你的内容没有重复。我们欢迎多样化的应用场景、方法和技巧！

### 如何创建拉取请求

如果你想贡献新的示例或教程，打开一个拉取请求，并@标签@merveenoyan 和 @stevhliu。

一些注意事项：

* 确保笔记本文件名为小写字母。
* 别忘了将笔记本添加到`_toctree.yml`和`index.md`中。
* 在笔记本的第一个标题后，添加你的作者信息，例如：`_Authored by: [Aymeric Roucher](https://huggingface.co/m-ric)_`。你可以链接到你的Hugging Face或GitHub个人资料。
* 删除无关的代码输出（如`pip install`）。确保笔记本没有空的代码单元。
* 如果使用了图像，上传到[huggingface/cookbook-images](https://huggingface.co/datasets/huggingface/cookbook-images)数据集，并在Markdown中使用图像链接，如：
```![RAG diagram](https://huggingface.co/datasets/huggingface/cookbook-images/resolve/main/rag-diagram.png)```

一旦拉取请求合并，笔记本将显示在[开源AI手册](https://hf.co/learn/cookbook)中。

### 将Cookbook翻译成你的语言

我们希望AI手册能支持更多语言！如果你愿意帮助翻译笔记本，请按照以下步骤操作🙏。

如果某些笔记本已经翻译成你的语言，可以将新的翻译文件添加到`notebooks/your_language`中。别忘了将新的笔记本添加到`notebooks/your_language/_toctree.yml`和`notebooks/your_language/index.md`中。

如果没有翻译成你的语言，创建一个以你的语言代码命名的目录，放在`notebooks`下。例如，`en`表示英文，`zh-CN`表示中文。语言代码应遵循ISO 639-1标准（见[这里](https://www.loc.gov/standards/iso639-2/php/code_list.php)）。你也可以使用`{两位小写字母}-{两位大写字母}`格式，如`zh-CN`。

在`notebooks/LANG-ID/_toctree.yml`和`notebooks/LANG-ID/index.md`中创建文件，并添加翻译后的笔记本。

最后，将你的语言代码（即`LANG-ID`）添加到`.github/workflows`文件夹中的`build_documentation.yml`和`build_pr_documentation.yml`文件里。