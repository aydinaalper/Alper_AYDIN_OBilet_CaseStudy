# Alper_AYDIN_OBilet_CaseStudy
## Soru 1: 

Bu senaryonun cevabı olarak danışman şirketlerin nasıl seçileceğini soruda istenen şekilde iki ayrı senaryoda ele almak istiyorum.

### İki İhtimalli (Go/No Go) Karar Verme Durumu
* **a ve b şıkları:** a şıkkındaki seçenek %85 doğruluk payına sahip yani bu durumda tavsiye dinlendiğinde accuracy %85. b şıkkında accuracy %70.
* **c şıkkı:** c şıkkındaki seçenek %50 doğruluk oranı veriyor. Normal şartlarda da iki seçenekli bir karar durumunda rastgele verilen bir kararın doğru çıkma ihtimali de %50 olur.
* **d şıkkı:** d şıkkında söylenenin yapıldığı durumda %20 fakat söylenenin tersini yapıldığı durumda accuracy %80 olur. 
* **e şıkkı:** e şıkkı için de söylenen yapıldığında %10 ihtimalle doğru ama söylenenin tersi düşünüldüğünde ise bu oran %90 olarak değerlendirilebilir.

Son durumda bu koşullar kıyaslanırken rastgele seçim yapma halinde %50 orana sahip olduğu için, bu oranın üstündeki doğruluk payları değerli tavsiye olarak değerlendirilmelidir. c şıkkındaki doğruluk olarak bu yüzden değerli olarak kabul edilmemelidir. Buna göre:

1. **e'nin önerisinin tersini yapmak** (%90)
2. **a** (%85 accuracy)
3. **d'nin önerisinin tersini uygulamak** (%80)
4. **b** (%70 accuracy)
olarak değerli fikirler sıralanabilir.

**Sıralama:** e > a > d > b

---

### Çok İhtimalli (0/1/2)Karar Verme Durumu
Durum bu sefer daha karmaşık bir hal alıyor. Söylenen ihtimalin tersini düşünme durumu bu sefer burada etkin değil çünkü 0/1/2 gibi 3 veya üzeri ihtimalli senaryoda bu sefer geriye birden fazla durum kalır ve etkin oran değişir. Bu sefer doğrudan verilen accuracy'ler üzerinden hareket etmek daha etkin olacaktır. 

Burada ise rastgele seçim durumunda %33.3 gibi bir ihtimale sahip olunacağı için bunun altındaki oranlar kesin olarak elenir. %50 oranı ise duruma göre kıymetli olabilse de karar verme aşamasında %50 üstü göstergeler bana göre aktif olarak değerli olarak tanımlanmalıdır. Bu durumda:

1. **a** (%85 accuracy)
2. **b** (%70 accuracy)

Bu iki öneren değerli olarak adlandırılıp değerlendirmeye alınmalıdır.
