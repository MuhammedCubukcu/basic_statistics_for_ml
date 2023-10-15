## 9. Konfüzyon Matrisi ve Performans Metrikleri

Konfüzyon matrisi, sınıflandırma modellerinin performansını değerlendirmek için kullanılan bir matris türüdür. Bu matris, modelin doğru ve yanlış sınıflandırdığı örnek sayılarını gösterir. Performans metrikleri, bu matrisin değerlerini kullanarak modelin performansını ölçen istatistiksel ölçütlerdir.

### Konfüzyon Matrisi

Bir sınıflandırma problemi için 2 sınıfı (örneğin, pozitif ve negatif) düşünelim:

|               | Gerçek Pozitif (TP) | Gerçek Negatif (TN) |
|---------------|---------------------|---------------------|
| Tahmin Pozitif (PP)  | TP                  | False Positive (FP)|
| Tahmin Negatif (PN)  | False Negative (FN)| TN                  |

- **True Positive (TP):** Gerçek pozitif durumda, modelin doğru bir şekilde pozitif olarak tahmin ettiği örnek sayısı.
- **True Negative (TN):** Gerçek negatif durumda, modelin doğru bir şekilde negatif olarak tahmin ettiği örnek sayısı.
- **False Positive (FP):** Gerçek negatif durumda, modelin yanlış bir şekilde pozitif olarak tahmin ettiği örnek sayısı.
- **False Negative (FN):** Gerçek pozitif durumda, modelin yanlış bir şekilde negatif olarak tahmin ettiği örnek sayısı.

### Performans Metrikleri

1. **Hassasiyet (Precision):**
   - TP / (TP + FP)
   - Pozitif olarak tahmin edilenler içinde gerçekten pozitif olanların oranını gösterir. Yanlış pozitiflerin etkisini ölçer.

2. **Duyarlılık (Recall):**
   - TP / (TP + FN)
   - Gerçek pozitiflerin ne kadarının tespit edildiğini gösterir. Yanlış negatiflerin etkisini ölçer.

3. **F1-Skoru:**
   - 2 * (Precision * Recall) / (Precision + Recall)
   - Hassasiyet ve duyarlılığın harmonik ortalamasıdır. Dengeli bir performans metriği olarak kullanılır.

### Örnek:

Bir kanser tarama testi düşünelim. Test pozitif olduğunda, gerçekten kanserli olan bir kişiyi doğru bir şekilde teşhis edebilme yeteneğini ölçmek istiyoruz.

- TP (Gerçek Pozitif): 150
- TN (Gerçek Negatif): 850
- FP (False Positive): 50
- FN (False Negative): 50

Bu durumda, performans metrikleri:

- Hassasiyet (Precision): 150 / (150 + 50) = 0.75
- Duyarlılık (Recall): 150 / (150 + 50) = 0.75
- F1-Skoru: 2 * (0.75 * 0.75) / (0.75 + 0.75) = 0.75

Bu örnekte, testin kanserli durumları doğru bir şekilde teşhis etme yeteneği yüksek hassasiyete sahiptir.

Bu, konfüzyon matrisi ve performans metriklerinin temel kavramlarından bir örnektir. Daha fazla detay veya örnek isterseniz, lütfen belirtin!