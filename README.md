# Knowledge Dialogue Generation paper reading

学习记录。

## Commonsense Knowledge

**Commonsense Knowledge Aware Conversation Generation with Graph Attention.** Zhou, Hao, Tom Young, Minlie Huang, Haizhou Zhao, Jingfang Xu, and Xiaoyan Zhu. (IJCAI 2018) **[paper](https://www.ijcai.org/proceedings/2018/643)**

文章首次将大规模commonsense knowledge融合到对话生成中，首次将knowledge以KG形式，attention方式融合到对话生成中。（基于KG的对话生成经典文章）

**Diverse and informative dialogue generation with context-specific commonsense knowledge awareness.** Wu, Sixing, Ying Li, Dawei Zhang, Yang Zhou, and Zhonghai Wu. (ACL 2020) **[paper](https://aclanthology.org/2020.acl-main.515/)**

文章用dialogue context增强了KG的表示，并且用context和response分别构建了knowledge的先验和后验分布，用KL散度作为loss使两者相似。

**Grounded Conversation Generation as Guided Traverses in Commonsense Knowledge Graphs.** Zhang, Houyu, Zhenghao Liu, Chenyan Xiong, and Zhiyuan Liu. (ACL 2020) **[paper](https://aclanthology.org/2020.acl-main.184/)**

文章考虑2-hop的KG关联（过去通常都是与当前turn直接关联的concept），增强模型实现concept shift的能力。

## Unclassified

**Improving Knowledge-Aware Dialogue Generation via Knowledge Base Question Answering.** Wang, Jian, Junhao Liu, Wei Bi, Xiaojiang Liu, Kejing He, Ruifeng Xu, and Min Yang. (AAAI 2020) **[paper](https://ojs.aaai.org/index.php/AAAI/article/view/6453)**

**Knowledge-Aware Dialogue Generation via Hierarchical Infobox Accessing and Infobox-Dialogue Interaction Graph Network.** Wu, Sixing, Minghui Wang, Dawei Zhang, Yang Zhou, Ying Li, and Zhonghai Wu. (IJCAI 2021) **[paper](https://www.ijcai.org/proceedings/2021/546)**

**Learning to Select Knowledge for Response Generation in Dialog Systems.** Lian, Rongzhong, Min Xie, Fan Wang, Jinhua Peng, and Hua Wu. (IJCAI 2021) **[paper](https://www.ijcai.org/proceedings/2021/546)**

**Plato: Pre-trained dialogue generation model with discrete latent variable.** Bao, Siqi, Huang He, Fan Wang, Hua Wu, and Haifeng Wang. (ACL 2020) **[paper](https://arxiv.org/abs/1910.07931)**

**Conversational Graph Grounded Policy Learning for Open-Domain Conversation Generation.** Xu, Jun, Haifeng Wang, Zheng-Yu Niu, Hua Wu, Wanxiang Che, and Ting Liu. (ACL 2020) **[paper](https://aclanthology.org/2020.acl-main.166/)**

## Knowledge Document

**Knowledge-Grounded Dialogue Generation with Pre-trained Language Models.** Zhao, Xueliang, Wei Wu, Can Xu, Chongyang Tao, Dongyan Zhao, and Rui Yan. (EMNLP 2020) **[paper](https://arxiv.org/abs/2010.08824)**

文章构建了一种融合knowledge document的对话生成模型，其中document选择和对话生成共同进行优化，用RL方法无监督地调整document选择的模型。（无需对相关knowledge document进行人工标记）

**Bridging the Gap between Prior and Posterior Knowledge Selection for Knowledge-Grounded Dialogue Generation.** Chen, Xiuyi, Fandong Meng, Peng Li, Feilong Chen, Shuang Xu, Bo Xu, and Jie Zhou. (EMNLP 2020) **[paper](https://aclanthology.org/2020.emnlp-main.275/)**

文章在训练阶段用后验信息增强先验信息，并设计蒸馏模型以消除exposure bias。

**Sequential Latent Knowledge Selection for Knowledge-Grounded Dialogue.** Kim, Byeongchang, Jaewoo Ahn, and Gunhee Kim. (ICLR 2020) **[paper](https://arxiv.org/abs/2002.07510)**

文章同样在训练阶段用后验信息增强先验信息，此外将knowledge selection作为**序列**决策过程，构建多轮knowledge selection的联合推断。

**Low-Resource Knowledge-Grounded Dialogue Generation.** Zhao, Xueliang, Wei Wu, Chongyang Tao, Can Xu, Dongyan Zhao, and Rui Yan. (ICLR 2020) **[paper](https://arxiv.org/abs/2002.10348)**

## Response Generation

**Graph-Structured Context Understanding for Knowledge-grounded Response Generation.** Li, Yanran, Wenjie Li, and Zhitao Wang. (SIGIR 2021 short) **[paper](https://dl.acm.org/doi/abs/10.1145/3404835.3463000)**

文章构建了context graph，涉及utterance节点（u）和entity mention节点（m），节点通过GCN进行融合交互学习，response generation参照过去研究，从候选entity中进行copy。

**Response-anticipated memory for on-demand knowledge integration in response generation.** Tian, Zhiliang, Wei Bi, Dongkyu Lee, Lanqing Xue, Yiping Song, Xiaojiang Liu, and Nevin L. Zhang. (ACL 2020) **[paper](https://arxiv.org/abs/2005.06128)**

**Multi-hop Selector Network for Multi-turn Response Selection in Retrieval-based Chatbots.** Yuan, Chunyuan, Wei Zhou, Mingming Li, Shangwen Lv, Fuqing Zhu, Jizhong Han, and Songlin Hu. (EMNLP 2019) **[paper](https://aclanthology.org/D19-1011/)**

