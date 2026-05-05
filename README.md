# find_good_cases
整个任务是AI FOR CHEMICAL当中的Molecular Captioning的任务，我们做了一个模型来完成他

我们现在的任务是要去测试一些我们的数据在其他模型上运行的成果，然后提取出一些case(我们跑的比较好的和他们跑的没我们好的，进行case分析)

现在我们有的数据信息如下:
predictions.json是我们预测的结果，img2caption_test.jsonl是image的目录 
img2caption.gz是测试集，但是可能需要处理一下，我们的输入是image+svg，要测试的其它LLMs应该只需要image就行

然后我们目前目标的测试的模型有Qwen-VL-Chat (7B)，ChemLLM-7B-Chat,ChemVLM-8B和ChemMLLM