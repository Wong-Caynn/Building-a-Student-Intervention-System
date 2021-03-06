# Building-a-Student-Intervention-System
# 构建学生成绩预警系统

## 项目描述

随着教育行业对科技的依赖与日俱增，有越来越多的数据可用于检验和预测。现在，通过像 Canvas 和 Edmodo 这样的学习管理系统，可以即时收集
并使用学生活动、分数、与教师和同学的互动等记录。这对于在学校中（甚至是初中和高中）越来越流行的网上教室尤为如此。 

在各级教育中，相关人士努力帮助提高学生成功的可能性，同时确保不削弱教育力度，或者不做出此类举动：在未改善实际的基础学习水平的情况下
，提高学生通过考评的可能性。就此而言，毕业率通常是选择标准，而且教育者和管理者正寻找新的方法尽早预测学生的成功和失败（早到足以实施
有效的干预以及确定不同干预措施的效果）。

为此，作为当地学区聘请的软件工程师，您的目标是，为预测学生有多大可能通过高中期末考试的相关因素建立模型。当地学区的目标是，通过在学
生退学前识别需要干预的学生，在这个十年结束时让毕业率达到 95%。 作为一位聪明的工程师，您决定运用从监督式机器学习课程中学到的概念来
实现学生干预系统。您并没有购买昂贵的服务器或从头开始实现新的数据模型，而是与第三方公司联系，让其提供运行您的软件所需的软件库和服务
器。

但是，由于资源和预算有限，校监会希望您能在最大限度节省计算费用（您按照在服务器上使用的内存和 CPU 时间向该公司付费）的情况下找出最有
效的模型。 为了构建干预软件，您首先需要分析与学生的表现有关的数据集。您的目标是，选择并开发一个能预测指定的学生通过考试的可能性的模
型，从而帮助诊断是否必须进行干预。必须根据我们提供的数据子集来开发模型，而且，将依据对学习算法未知的数据子集来测试该模型，以便测试
模型对训练集外部的数据的有效性。

将根据三个因素来评估您的模型：

•	它的 F1 分数，该因素汇总在所有可能的情况下正确的正样例和正确的负样例的数量。换言之，模型在区分可能通过考试与通不过考试上的表现
	如何？

•	训练集的大小（优先选择较小而不是较大的训练集）。也就是说，模型需要多少数据才能进行合理的预测？

•	进行合理预测所需的计算资源。需要多少时间和内存才能正确识别需要干预的学生？

## 项目报告

	1. 分类与回归

您的目标是识别可能需要早期干预的学生 - 这是哪种类型的监督式机器学习问题，是分类还是回归？为什么？

	2. 研究数据

您能否找出有关此数据集的以下事实？

•	学生总数

•	通过考试的学生人数

•	未通过考试的学生人数

•	班级毕业率 (%)

•	特征数（不包括标签/目标列）

	3. 准备数据

执行以下步骤，以准备供建模、训练和测试用的数据：

•	确定特征列和目标列

•	对特征列进行预处理

•	将数据分解为训练集和测试集

	4. 训练和评估模型

选择 scikit-learn 中提供的适用于此问题的 3 个监督式学习模型。对于每个模型：

•	此模型的常规用途有哪些？它有何优缺点？

•	考虑到您迄今为止对这些数据的认识，您为何选择应用此模型？

•	将此模型拟合到训练数据，尝试为训练集和测试集预测标签，然后测量 F1 分数。对不同的训练集大小（100、200、300）重复此过程，并让测
	试集保持不变。
	
•	生成一个表格，以显示每个训练集大小的训练时间、预测时间、训练集的 F1 分数和测试集的 F1 分数。
注意：需要生成 3 个这样的表格 - 每个模型一个。

	5. 选择最佳模型

根据您前面进行的试验，用 2-3 段话向校监会说明您选择哪个模型作为最佳模型。哪个模型具有最佳测试 F1 分数和时间效率？根据可用的数据、
有限的资源、费用和性能，哪个模型在总体上最为合适？请直接比较和对比记录的数值以证明您的观点。

	6. 模型认识体会

用 1-3 段话从外行人的角度向校监会说明最终选择的模型将会如何工作（例如，如果您选择了决策树或支持向量机，则说明它如何进行预测）。

	7. 微调模型

将 gridsearch 与至少一个要调整的重要参数和至少三个设置一起使用。使用整个训练集来做这件事。

	8. 最终分数

模型的最终 F1 分数是多少？
