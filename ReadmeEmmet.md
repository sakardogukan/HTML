# VsCode İçin Emmet ile Daha Hızlı HTML Yapıları Oluşturulması...
<!-- https://docs.emmet.io/cheat-sheet/ sayfasında kısayollar mevcut... Önemli bir dokuman !!!! -->

<!--
    Emmet web geliştiricilerinin sıklıkla zamandan tasarruf etmek ve daha hızlı kod yazmak için kullandığı bir eklentidir. Emmet’in temel mantığı, yazılımcıya kodlama yaparken zaman kazandırmasıdır. Emmet'in Kısa Yolları:

    ! + TAB tuşu ile HTML dokumanında ana yapı direkt oluşturulur. Örnek yapı:
        <!DOCTYPE html>
        <html lang="en">
            <head>
                <meta charset="UTF-8">
                <meta http-equiv="X-UA-Compatible" content="IE=edge">
                <meta name="viewport" content="width=device-width, initial-scale=1.0">
                <title>Document</title>
            </head>
            <body>            
            </body>
        </html>

    > ifadesini kullanarak kardeş element oluşturuyoruz. Örneğin; ul>li
        <ul>
            <li></li>
        </ul>

    Bu işlemi yaptıktan sonra ul tagına eklemek istediğimiz bir kardeş eleman kalmayınca ise ^ ifadesini kullanarak ul tagı dışına çıkıp yeni taglar oluşturabiliriz. ul>li^p
        <ul>
            <li></li>
        </ul>
        <p></p>
    
    ul veya ol tagları içerisine birden fazla li oluşturmak istiyorsak ul>li*3 veya ul>li+li+li
        <ul>
            <li></li>
            <li></li>
            <li></li>
        </ul>
    
    Tag eklerken onlara class özelliği vermek için de . ifadesini kullanırız. ul.class1>li.class2
        <ul class="class1">
            <li class="class2"></li>
        </ul>    
    
    Bir id özelliği eklemek için ise # ifadesini kullanırız. ul#id1>li#id2
        <ul id="id1">
            <li id="id2"></li>
        </ul>
    
    Burada + ve * ifadesinin farkını da daha kolay anlayabiliriz. Örneğin ul tagının içine aynı id’ye sahip 3 adet li eklemek istiyorsam * ifadesi kullanılabilir. Fakat amacım farklı id’lere sahip üç adetli tag oluşturmak için ul>li#id1+li#id2+li#id3
        <ul>
            <li id="id1"></li>
            <li id="id2"></li>
            <li id="id3"></li>
        </ul>
    
    Otomatik artış sağlayan değerleri tek tek yazmak amacımız zaman tasarrufu iken ne kadar mantıklıdır? Emmet bunun için de bir kısa yola sahip $ ifadesi. Yani yukarda görmüş olduğunuz ul>li#id1+li#id2+li#id3 şeklinde yazdığımız kod bloğunu çok daha basit bir biçimde ul>li#idNo$*3 diyerek yazabiliriz. Böylece otomatik olarak idNo1, idNo2 ve idNo3 idlerine sahip üç adet li tagımız olur.
        <ul>
            <li id="idNo1"></li>
            <li id="idNo2"></li>
            <li id="idNo3"></li>
        </ul>
    
    Sırada oluşturulan tagların içine text yazılması işlemi. Textlerimizi {} ifadesinin içine yazmamız yeterlidir. 
    p{Emmet ile tag içine text yazma}
    
    Bir diğer emmet kısa yolunu ise kodumuzda içerik olmadığı zamanlarda kullandığımız anlamsız yazıları yani “lorem ipsum”ları oluşturmak için kullanıyoruz. Örneğin bir paragraf oluşturacaksınız ve bu paragrafın henüz bi içeriği yok fakat boş durmasındansa oraya metin geleceğini belirtmek istiyorsunuz veya metin geldiğinde nasıl görüneceğini görmek istiyorsunuz. Anlamsız harfler veya zaman gerektiren rastgele cümleler oluşturmak yerine bu kısayolu kullanabilirsiniz : p>lorem Taba bastığınızda aşağıdaki gibi bir çıktı alacaksınız.

    Uzun bir lorem yazısı istemiyorsanız yapmanız gereken tek şey lorem yazdıktan sonra yanına kaç kelimeli bir lorem oluşturmak istediğinizi eklemek. Örneğin 5 kelimeli bir lorem yazısı istiyorsunuz. Bunun için p>lorem5 yazmanız yeterlidir.

    Son olarak; li.className yazıp Tab’a bastığımızda ne oluşmasını bekleriz? Evet className class’ına ait bir li tagı oluşmasını. peki herhangi bir tag koymaksızın sadece .className yazdıktan sonra Tab’a basarsak ne olur?
        <div class="className"></div>

    Emmet’e bir tag vermeksizin . veya # ifadelerini kullandığımızda bunun div tagı olduğunu biliyor.
    Sadece . ifadesi verildiğinde; <div class=""></div>
    .# ifaedi birlikte verildiğinde; <div class="" id=""></div>

    h3.deneme#idolussun>lorem2 ifadesi ile; <h3 class="deneme" id="idolussun">Lorem, ipsum.</h3> oluşur.

    etiket isimleri direkt yazılabilir.
    + kardeş oge (ya da element)
    > içinde oge (ya da element)
    ^ yukarı çık ve oge oluştur
    * çarp -> p*3
    lorem -> uzun bir yazı
    lorem3 -> 3 kelimelik bir yazı oluşur
    . -> div etiketli bir class oluşur.
    # -> ID
 -->