**一句话概要**  
KRAMABENCH 提出首个面向数据湖场景的端到端数据科学流程基准测试，揭示当前AI模型在复杂现实数据管道构建中的能力局限。

**主体**  
现实世界的数据科学流程面临多重挑战：从异构数据湖中提取信息、跨源整合数据、执行从清洗到分析的全链路操作，这些任务既需要领域知识又依赖技术专长。尽管当前AI模型展现出强大的代码生成与推理能力，但其能否驾驭如此复杂的现实场景仍是未知数。作者团队通过构建KRAMABENCH填补了这一评估空白，该基准包含104个真实场景数据管道，覆盖6个领域的24种数据源和1700个文件，全面测试数据发现、清洗转换、统计推理等关键能力。

为解决评估标准化问题，研究设计了DS-GURU参考框架，指导AI模型将高层任务分解为子步骤，逐步推理并生成可执行的Python代码。实验对比了5种通用模型和3种代码生成模型，结果显示：虽然现有模型能处理规范明确的数据科学任务，但在需要深度数据处理与领域知识的真实场景中表现欠佳。例如，模型在涉及多源数据融合或非结构化数据转换时，正确率较理想场景下降超过40%。

这项工作为开发自主数据科学代理奠定了基础，其开源的基准框架与评估体系（包含7个可视化分析图与1个综合性能对比表）将推动AI在复杂数据工程中的能力边界探索。未来研究可基于此基准开发更强大的领域适应与多模态推理技术，最终实现从原始数据到商业洞察的自动化飞跃。