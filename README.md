# The Transformer in PyTorch A minimal PyTorch implementation of the Transformer for sequence to sequence learning.

Supported features:
- Mini-batch training with CUDA

## Usage

Training data should be formatted as below:
```
source_sequence \t target_sequence
source_sequence \t target_sequence
...
```

To prepare data:
```
python prepare.py training_data
```

To train:
```
python train.py model vocab.src vocab.tgt training_data.csv num_epoch
```

To predict:
```
python predict.py model.epochN vocab.src vocab.tgt test_data
```

## References

Rami Al-Rfou, Dokook Choe, Noah Constant, Mandy Guo, Llion Jones. [Character-Level Language Modeling with Deeper Self-Attention.](https://arxiv.org/abs/1808.04444) arXiv:1808.04444.

Jimmy Lei Ba, Jamie Ryan Kiros, Geoffrey E. Hinton. 2016. [Layer Normalization.](https://arxiv.org/abs/1607.06450) arXiv:1607.06450.

Zihang Dai, Zhilin Yang, Yiming Yang, Jaime Carbonell, Quoc V. Le, Ruslan Salakhutdinov. 2019. [Transformer-XL: Attentive Language Models Beyond a Fixed-Length Context.](https://arxiv.org/abs/1901.02860) In ACL.

Hideya Mino, Masao Utiyama, Eiichiro Sumita, Takenobu Tokunaga. 2017. [Key-value Attention Mechanism for Neural Machine Translation.](http://aclweb.org/anthology/I17-2049) In Proceedings of the 8th International Joint Conference on Natural Language Processing, pp. 290-295.

Ashish Vaswani, Noam Shazeer, Niki Parmar, Jakob Uszkoreit, Llion Jones, Aidan N. Gomez, Lukasz Kaiser, Illia Polosukhin. 2017. [Attention Is All You Need.](https://arxiv.org/abs/1706.03762) In NIPS.
