# Глубокое обучение

## HW1

* 1.1 conv2d через F.unfold и одно матричное умножение, поддержаны stride, padding, dilation и groups
* 1.2 backward свёртки через conv_transpose2d с output_padding, проверен gradcheck
* 1.3 empirical_rf по градиенту центрального выхода и erf_std для effective receptive field
* 2.1 MyBatchNorm2d с running статистиками, совместим по state_dict с nn.BatchNorm2d
* 2.2 вывод весов после слияния, fuse_conv_bn и fuse_sequential, замер скорости
