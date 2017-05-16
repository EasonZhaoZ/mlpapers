## postive and unlabeled data问题

[conversion delay](http://www0.cs.ucl.ac.uk/staff/w.zhang/rtb-papers/delayed-feedback.pdf)使得negative label不一定真的是negative的，论文通过对conversion delay建模，提出的DFM(Delayed Feedback Model)模型可以理论上获得更准的cvr预估结果，而且可以使用SGD算法求解，实用性很强。

