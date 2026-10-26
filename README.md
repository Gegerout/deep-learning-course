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
* 5.1 pgd_l2 с нормированным шагом и проекцией на шар, сравнение с PGD в L_inf
* 5.3 transfer атак FGSM и PGD-20 с model A на model B и MLP
* 6.1 adversarial_train с PGD-7 и кривые robust accuracy по радиусу атаки
* 6.2 sanity_checks с FGSM, PGD-20, PGD-100 с пятью рестартами и атакой радиуса 1
* 6.3 input_gradient и доля массы градиента на фоне для обычной и робастной модели
* 7.2 conv2d_fft через rfft2 и einsum с поддержкой stride, padding и groups
* 7.3 newton_schulz и ConvMuon для свёрточных весов, обучение ResNet-20 с Muon
* 7.4 L0 атака на обычную и робастную модель
* 7.5 catastrophic overfitting при обучении с FGSM и FGSM-RS
