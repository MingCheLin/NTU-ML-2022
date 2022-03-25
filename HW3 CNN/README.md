這次要跑的時間比預想的還久，

train完後ensemble來不及寫完只好Late submission了QQ，

這次使用ResNeXt與se-Resnet進行ensemble，

有嘗試過如ConvNeXt、efficientNet等但都train不起來不確定原因，

技巧方面用了mixup、augmentation、Time augmentation、learning rate scheduling，

在此基礎上RestNeXt單獨使用有約0.89的acc，

se-resnet則是0.85左右，

但兩者訓練時間不同，

若是再久點兩者應該都可以更好，

將兩者結果合併為22維input加上一層fully connected layer作為ensemble後可以提高1~2%準確度。

感覺mixup再做好一點再使用ConvNeXt應該可以做到更好。
