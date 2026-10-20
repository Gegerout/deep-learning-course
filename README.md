# Глубокое обучение

## HW1

* 1.1 conv2d через F.unfold и одно матричное умножение, поддержаны stride, padding, dilation и groups
* 1.2 backward свёртки через conv_transpose2d с output_padding, проверен gradcheck
* 1.3 empirical_rf по градиенту центрального выхода и erf_std для effective receptive field
* 2.1 MyBatchNorm2d с running статистиками, совместим по state_dict с nn.BatchNorm2d
* 2.2 вывод весов после слияния, fuse_conv_bn и fuse_sequential, замер скорости
* 3.1 вывод дисперсии для ReLU и tanh, activation_stds для MLP глубины 50 с разными инициализациями
* 3.2 MyAdamW с группами параметров и флагом bias_correction, вывод длины шага без поправки
* 3.3 cosine_lr для LambdaLR, проверено совпадение с CosineAnnealingLR
* 4.1 ResNetCIFAR глубины 6n + 2 с флагами residual и separable
* 4.2 train_cifar с MyAdamW, cosine schedule до нуля и test accuracy после каждой эпохи
* 4.3 сравнение plain-20 и plain-56 при одинаковом бюджете
