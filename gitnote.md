1:

CONFİG.----------------

# git --version   > git yüklümü değilmi versiyon kontrolu 
# git config -- global user.name "kullanicı adı"
enter
# git config --list      > kullanıcıları listeleriz

# git config --global user.email "mail adresi"      > kullanıcı mail adresi ekledik
# git config --list      > kullanıcıları listeleriz




2:

GİT İNİT----------------------------

uygulama:
# mkdir app
# cd app
# touch index.html
# touch test.txt
# ls

-------------
içinde bulunduğumuz klasöre gir #pwd ile kontrol et 

# git init >  klasör git özellikli proje dosyası haline geldi initialize oldu ---------klasöre master ünvanı geldi mi? kontrol et   master sana ait bir branch !!
# ls -a    >  . ile başlayan git gizli klasörünü gördün mü?




3:


GİT STATUS ---------------------------------
# git status    >   initlenmiş ama staging areaya aktarılmamış dosyaları gösterir / branch gösterir    kırmızı ile olanlar stage areaya girmemiş yeşiller hazır ??




4:


GİT ADD-------------------------

local repolardaki yapılan değişiklikleri push öncesi staging areya gönderme sürecidir (git add .)
# git add .     >  directorydeki tüm doyaları "." koyarak aktarabiliriz
veya
# git add "filename"    > commit etmek istediğin file veya değişiklikleri push etmeden önce add ile stagin areaya yani localdeki hazır haldeki kuyruğa alma işlemi


enter sonrası son durumu sana gösterecektir yeşi,l klasörlere dikkat edelim ....



uygulama 2 :
# touch deneme.txt 
# git status 
>>>dikkat edelim yeni oluşan klasör kırmızı yani, add edilmedi ve stagin area da yok .

# git add .
# git status    >> kontrol et tüm dosyalar stagin Area da 





5:


GİT COMMİT----------------------
# git commit -m "commit mesajımızı yazalım neden ne için olay ne"
# git status     >>   herhangibir commit bekleyen olay olmadığı yazar.


uygulama 3 :
# touch deneme2.txt
# git status
# git add deneme2.txt veya git add .
# git status 
# git commit -m "deneme2.txt dosyaını klasöre eklendi"
# git status 


6:

GİT LOG------------------------------------------

# git log      > yapılan commitlerin sıralı listeleri ve id ve branchleri gelir 



7:


GİT VERSİON----------------------- VERSİYON DEĞİŞİKLİĞİ

uygulama4:
# touch deneme4.txt
# git status
# git add .
# git commit -m "deneme4.txt eklendi"
# git status
# git log 
q ile çık 


örnek olay manuel olarak masaüstünden yanlışlıkla bir personel yeni açılan deneme 4 . txt sildi diyelim ve bizde silelim .????

# git status  >>>>>> kayıp dosya uyarısını alacağız  

# git add .
# git status >>>>> dediğimizde doya silindi şeklinde gözükür
# git commit -m "deneme4.txt silindi"
# git status 

 # git log


 sonuç olarak biz bu klasören yanlışlıkla silinen deneme4.txt dosyasını geri getirmek için önceki versiyona yani deneme4.txt silinmeden önceki versiyon commit işlemine geri dönelim .!!!


 # git log 
 >>>>> deneme 4 ü eklediğimiz açıklaması mevcuttur commit id sini kopyalayalım 

 # git checkout <versiyon commit id yapıştır> -- .
 enter sonrası eski hale geri döndük  ama bu dosyayı staging areaya tekrar aldı commit repostorysine değil .

 # git commit -m "deneme4.txt tekrar eklendi versiyon dönüldü"
 # git status 
 # git log 
 ls -la 



 8:
 
 
  GİT DİFF----------------

UYGULAMA 5 :
deneme 4.txt dosyasını masaüstünden ıu olarak açalım ve içine herhangi notlar yazalım kaydedelim ve terminale geri dönelim.


# git diff >>>>>   içinde değişiklik yapılan dosyayı gösterir .

# git add .

# git status 

# git commit -m " deneme4.txt içinde değişiklik yapıldı "

# git status
# git log



 9:

 GİT RESTORE--------------------- değişiklikleri geri alma 





 10:

 GİT REMOVE---------------------------



 11:

 GİT MOVE--------------------


 12:

 GİT ALİAS-----------------------------




 13:

 GİT PUSH-----------------------------


 14:
  GİT PULL---------------------------




  15:


  GİT İGNORE---------------------------


  16.


  GİT BRANCH-------------------------------------------


https://www.youtube.com/watch?v=zcOZJGHEEw8&list=PLld6WWpFK1nEhFvvYi5ts-_JoUL3wF3zz&index=10





















