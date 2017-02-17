!["Python iii"](https://sudo.ubuntu-tr.net/assets/post/pyhton-programlama-seri-ii/pyhton-programlama-seri-ii.jpeg)

# 1. Giriş
Bilgisayarlarımızın gücü ne kadardır? Gerçekten ne kadar hızlı hesap yapabilirler? Yalnızca hesap mı yapabilirler? Sadece sayılar üzerinde dört işlemden biraz fazlasını yapabilen ufak bir çip ile nasıl böylesine harikalar oluşturabiliniyor? Programlama adına hiçbir şey bilmiyorken aklımı kurcalayan sorulardan bazıları bunlardı.. Bu bölümde bu soruların cevabını, uygulayarak bulacağız.

# 2. Neler yaptık?
Python'da koşula bağlı ifadeleri _if_ deyimiyle yazıyorduk. _If_, _elif_, _else_ deyimleri bize yazdığımız programa ilkelce akıl katmamızı sağlıyordu.

Python'daki yazdığımız kodları dosyalar halinde kaydederek (\*.py uzantıları ile) gerçek bir program gibi çalıştırdık. Python kabuğunu genel olarak denemelerimiz için kullanabileceğimizi gördük, asıl programlarımız metin dosyalarının içinde tutulup Python yorumlayıcıya teslim edilir.

Bunun yanında Python'da yorumlayıcıya verdiğimiz değerlerin her birinin belirli tiplerinin olduğunu öğrendik.
+ Karakter dizilerine **String**
+ Tam sayılara **Integer**
+ Ondalıklı sayılara **Float**
+ Doğru ya da yanlış değerlerini tutan ifadeye **Boolean**

deniliyordu. Bu değerleri değişkenlere atayarak bellekte (RAM) saklayabiliyorduk. Böylece istediğimiz zaman kullanabiliyorduk. Değişkenlerin tiplerini de _type()_ metodu ile öğrenebiliyorduk.

Bu kez, girişte de sorulan sorulara cevap niteliğinde konular göreceğiz. Yani bilgisayar gerçekten ne kadar hızlı çalışabiliyor? Ya da işleri kolaylaştırmakta programlama dili ne kadar işimize yarıyabilir?

# Listeler
Integer (tam sayı), float (ondalıklı sayı), string (karakter dizisi) gibi veri tiplerini beraber tutabileceğimiz bir veri yapısı listelerdir. Listeler verileri toplu biçimde saklamamızı ve onları kullanmamızı sağlarlar.

Listeler programlama için oldukça önemlidir ve verileri saklamada temel yapı kabul edilir. Python'daki diğer veri tiplerini daha ileride işleyeceğiz.

Listeleri köşeli parantezlerle tanımlarız. Mesela:

```python
liste = []
```
bizim için içi boş bir liste oluşturur. İçi dolu bir liste oluşturmak istersek şöyle bir satır yazabilirdik:

```python
liste = [1, 2, 50, "yazı", 10.25]
```

Gördüğünüz gibi listemizin içinde farklı veri tipleri bulundurabiliyoruz. İlk programlama dili olarak Python gören biri için bu çok da anlam ifade etmeyebilir ama bu özellik diğer birçok programlama dilinde olmayan işleri kolaylaştıran bir özelliktir.

Listeyi bu şekilde tanımlıyoruz. Listenin elemanlarına erişmek ve listenin bazı özelliklerini tanımak için şöyle bir program yazalım:

```python
dagitimlar = ["Ubuntu", "Fedora", "Arch", "Suse", "Mint"]

#Listenin elemanları teker teker yazdırılır
print(dagitimlar[0])
print(dagitimlar[1])
print(dagitimlar[2])
print(dagitimlar[4])
print(dagitimlar[3])
#Listenin elemanları yazdırıldı

#Listenin kaç elemandan oluştuğu yazdırılır.
print(len(dagitimlar))

#Liste yazdırılır ve bir eleman silinir.
print(dagitimlar)
del dagitimlar[2]
print(dagitimlar)
```
