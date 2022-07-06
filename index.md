## Welcome to MLSLT Homepage
Most of the research to date focuses on bilingual sign language translation (BSLT).
However, such models are inefficient in building multilingual sign language translation systems.
To solve this problem, we introduce the multilingual sign language translation (MSLT) task. It aims to use a single model to complete the translation between multiple sign languages and spoken languages.
Then, we propose MLSLT, the first MSLT model, which contains two novel dynamic routing mechanisms for controlling the degree of parameter sharing between different languages.
Intra-layer language-specific routing controls the proportion of data flowing through shared parameters and language-specific parameters from the token level through a soft gate within the layer, and inter-layer language-specific routing controls and learns the data flow path of different languages at the language level through a soft gate between layers.
In order to evaluate the performance of MLSLT, we collect the first publicly available multilingual sign language understanding dataset, Spreadthesign-Ten (SP-10), which contains up to 100 language pairs, e.g., CSL->en, GSG->zh.
Experimental results show that the average performance of MLSLT outperforms the baseline MSLT model and the combination of multiple BSLT models in many cases.
In addition, we also explore zero-shot translation in sign language and find that our model can achieve comparable performance to the supervised BSLT model on some language pairs.


SP-10 Dataset
---------------
Please clone our [repository](https://github.com/MLSLT/SP-10) for downloading. We suggest reading [README](https://github.com/MLSLT/SP-10/blob/main/README.md) before using the dataset.

Citation
--------------

Please cite the [MLSLT paper](https://openaccess.thecvf.com/content/CVPR2022/papers/Yin_MLSLT_Towards_Multilingual_Sign_Language_Translation_CVPR_2022_paper.pdf) if it helps your research:
```bibtex
@inproceedings{yin2022mlslt,
  title={MLSLT: Towards Multilingual Sign Language Translation},
  author={Yin, Aoxiong and Zhao, Zhou and Jin, Weike and Zhang, Meng and Zeng, Xingshan and He, Xiaofei},
  booktitle={Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition},
  pages={5109--5119},
  year={2022}
}
```
