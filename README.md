# Alzheimer MRI Sınıflandırma

Bu proje, MRI görüntülerinden Alzheimer hastalığının evrelerini sınıflandırmak amacıyla geliştirilmiştir. Transfer öğrenme yöntemiyle **DenseNet121** mimarisi kullanılmıştır.

##  Özellikler
- 4 sınıf: `MildDemented`, `ModerateDemented`, `NonDemented`, `VeryMildDemented`
- Model eğitimi Google Colab üzerinde gerçekleştirilmiştir.
- DenseNet121 modeli önceden eğitilmiş ImageNet ağırlıklarıyla kullanılmıştır.
- Eğitim sürecinde `EarlyStopping`, `ReduceLROnPlateau`, `ModelCheckpoint`, `class_weight` ve `TensorBoard` gibi stratejiler uygulanmıştır.
- Kullanıcı dostu tahmin arayüzü için Gradio kullanılmıştır.

##  Model Kullanımı
Gradio arayüzü ile kullanıcılar MRI görüntüsü yükleyerek modelin tahminini görebilir.

##  Veri Kümesi
Veri setine aşağıdaki bağlantıdan erişebilirsiniz:

🔗 [Veri Setini İndir](https://www.kaggle.com/code/mohamedgobara/augmented-alzheimer-mri-dataset-with-93-5/input)
