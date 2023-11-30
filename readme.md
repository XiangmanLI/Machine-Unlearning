 # Machine Unlearning Papers

[2023](#2023) &nbsp;
[2022](#2022) &nbsp;
[2021](#2021) &nbsp;
[2020](#2020) &nbsp;
[2019](#2019) &nbsp;
[2018](#2018) &nbsp;
[2017](#2017) &nbsp;
[< 2017](#before-2017) &nbsp;


---

### 2023
| Author(s) | Title |  Venue |Abstract |
|:--------- | ---------------------- | ----------------- | -------------------------------------------------------------- |
| Xiaoyu Cao et al.| [FedRecover: Recovering from Poisoning Attacks in Federated Learning using Historical Information](https://arxiv.org/abs/2210.10936)| 2023 IEEE Symposium on Security and Privacy (SP) |"Abstract—Federated learning is vulnerable to poisoning attacks in which malicious clients poison the global model via sending malicious model updates to the server. Existing defenses focus on preventing a small number of malicious clients from poisoning the global model via robust federated learning methods and detecting malicious clients when there are a large number of them. However, it is still an open challenge how to recover the global model from poisoning attacks after the malicious clients are detected. A naive solution is to remove the detected malicious clients and train a new global model from scratch using the remaining clients. However, such train-from-scratch recovery method incurs a large computation and communication cost, which may be intolerable for resource-constrained clients such as smartphones and IoT devices. In this work, we propose FedRecover, a method that can recover an accurate global model from poisoning attacks with a small computation and communication cost for the clients. Our key idea is that the server estimates the clients’ model updates instead of asking the clients to compute and communicate them during the recovery process. In particular, the server stores the historical information, including the global models and clients’ model updates in each round, when training the poisoned global model before the malicious clients are detected. During the recovery process, the server estimates a client’s model update in each round using its stored historical information. Moreover, we further optimize FedRecover to recover a more accurate global model using warm-up, periodic correction, abnormality fixing, and final tuning strategies, in which the server asks the clients to compute and communicate their exact model updates. Theoretically, we show that the global model recovered by FedRecover is close to or the same as that recovered by train-from-scratch under some assumptions. Empirically, our evaluation on four datasets, three federated learning methods, as well as untargeted and targeted poisoning attacks (e.g., backdoor attacks) shows that FedRecover is both accurate and efficient. |


###2020
| Author(s) | Title |  Venue |Abstract |
|:--------- | ---------------------- | ----------------- | -------------------------------------------------------------- |
| Yi Liu et al. | The Right to be Forgotten in Federated Learning: An Efficient Realization with Rapid Retraining | IEEE INFOCOM 2022 | In Machine Learning, the emergence of the right to be forgotten gave birth to a paradigm named machine unlearning, which enables data holders to proactively erase their data from a trained model. Existing machine unlearning techniques focus on centralized training, where access to all holders’ training data is a must for the server to conduct the unlearning process. It remains largely underexplored about how to achieve unlearning when full access to all training data becomes unavailable. One noteworthy example is Federated Learning (FL), where each participating data holder trains locally, without sharing their training data to the central server. In this paper, we investigate the problem of machine unlearning in FL systems. We start with a formal definition of the unlearning problem in FL and propose a rapid retraining approach to fully erase data samples from a trained FL model. The resulting design allows data holders to jointly conduct the unlearning process efficiently while keeping their training data locally. Our formal convergence and complexity analysis demonstrate that our design can preserve model utility with high efficiency. Extensive evaluations on four real-world datasets illustrate the effectiveness and performance of our proposed realization. |


###2020
| Author(s) | Title |  Venue |Abstract |
|:--------- | ---------------------- | ----------------- | -------------------------------------------------------------- |
| Yinjun Wu et al. | DeltaGrad: Rapid retraining of machine learning models | Proceedings of the 37 th International Conference on Machine Learning | Machine learning models are not static and may need to be retrained on slightly changed datasets, for instance, with the addition or deletion of a set of datapoints. This has many applications, including privacy, robustness, bias reduction, and uncertainty quantification. However, it is expensive to retrain models from scratch. To address this problem, we propose the DeltaGrad algorithm for rapid retraining machine learning models based on information cached during the training phase. We provide both theoretical and empirical support for the effectiveness of DeltaGrad, and show that it compares favorably to the state of the art.
