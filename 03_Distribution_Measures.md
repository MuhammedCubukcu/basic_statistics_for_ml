# 3. Dağılım Ölçüleri
## Varyans ve Standart Sapma
Varyans ve standart sapma, veri setinin ne kadar yayıldığını ölçen önemli istatistiksel kavramlardır.

### Varyans (Variance)
Varyans, bir veri setindeki değerlerin ortalama etrafında ne kadar yayıldığını ölçen bir istatistiksel ölçüdür. Daha spesifik olarak, her bir veri noktasının ortalama değerden ne kadar uzak olduğunu gösteren bir ölçüdür.
Formülü şu şekildedir:
```scss
Var(X) = Σ(xi - μ)² / N
```
Burada:
- xi veri setindeki her bir değer,
- μ veri setinin ortalaması,
- \(N\) gözlem sayısını temsil eder.

### Standart Sapma (Standard Deviation)
Standart sapma, varyansın kareköküdür. Veri setinin ne kadar yayıldığını ifade eder. Daha küçük bir standart sapma, veri noktalarının ortalamaya yakın olduğunu gösterirken, daha büyük bir standart sapma, veri noktalarının daha geniş bir aralığa yayıldığını gösterir.

Standart sapma, varyansın karekökü olarak hesaplanır. 
Formülü şu şekildedir:
```css
σ = √Var(X)
```
Örnek:
Diyelim ki elimizde şu veri seti bulunuyor:
```python
data = [3, 5, 7, 9, 11]
```
Önce ortalamayı hesaplayalım:
```python
mean = sum(data) / len(data)  # mean = 7
```
Sonrasında varyansı hesaplayalım:
```python
variance = sum((x - mean) ** 2 for x in data) / len(data)  # variance = 8
```
Ve son olarak standart sapmayı alalım:
```python
std_deviation = variance ** 0.5  # std_deviation = 2.8284
```

* Varyans ve standart sapma, veri setinin dağılımını ve değişkenliğini anlamak için önemli istatistiksel araçlardır. Daha büyük bir varyans veya standart sapma, veri setinin daha yayıldığını gösterirken, daha küçük bir değer daha az yayılmış bir veri setini temsil eder.

## Varyans ve standart sapma, istatistiksel veri analizinde kullanılan önemli ölçümlerdir. İşte bu kavramların neden kullanıldığına dair bazı nedenler:

### 1. Veri Dağılımını Anlama:

* Varyans: Veri noktalarının ortalamadan ne kadar uzak olduğunu gösterir. Büyük varyans, veri noktalarının dağılımının geniş olduğunu gösterir.
* Standart Sapma: Varyansın kareköküdür. Bu da veri setinin ne kadar yayıldığını gösterir. Daha küçük bir standart sapma, veri noktalarının ortalamaya daha yakın olduğunu gösterir.
### 2. Değişkenliği Karşılaştırma:

* F*arklı veri setlerinin değişkenliğini karşılaştırmak için kullanılır. Örneğin, iki farklı ürünün satış verilerinin varyansı karşılaştırılabilir.
### 3. Aykırı Değerleri Belirleme:

* Standart sapma, veri setindeki aykırı değerleri belirlemek için kullanılabilir. Eğer bir değer, ortalamanın birkaç standart sapma ötesinde ise, bu değer aykırı olarak kabul edilebilir.
### 4. Tahmin ve Kestirimler:

* Standart sapma, bir tahminin güvenilirliğini değerlendirmek için kullanılabilir. Daha küçük bir standart sapma, tahminin daha güvenilir olduğunu gösterir.

### 5. Kalite Kontrol:

* Üretim süreçlerinde varyans ve standart sapma, ürünlerin kalitesini kontrol etmek için kullanılır. Daha düşük varyans, üretim sürecinin daha istikrarlı olduğunu gösterebilir.
### 6. Finansal Analiz:

* Finansal piyasalarda risk değerlendirmesi yapmak için kullanılır. Daha yüksek standart sapma, yatırımın daha riskli olduğunu gösterir.

### 7. Bilimsel Araştırmalar:

* Bilimsel çalışmalarda, veri setlerinin dağılımını ve değişkenliğini anlamak için kullanılır. Bu, sonuçların güvenilirliğini artırabilir.

### 8. Eğitim ve Öğrenme:

* Eğitimde, öğrenci başarılarının değişkenliği değerlendirilebilir. Daha düşük varyans, öğrencilerin başarılarının daha homojen olduğunu gösterebilir.
Varyans ve standart sapma, istatistiksel analizlerin temel taşlarıdır ve veri setinin özelliklerini anlamak için yaygın olarak kullanılır.

