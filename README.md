# NotUygulamasiWithSqlite

## Özet

Swift programlama dili kullanarak, kendimi geliştirmek amacıyla yapmış olduğum ikinci projem. Bu proje stoaryboard kullanılarak geliştirildi. Temelde 3 adet viewController yapısından oluşuyor;
1. Anasayfa
2. Not Ekle
3. Not Detay

Anasayfa üzerinde tableview yapısı kullanılarak sqlite üzerinde kayıtlı olan not verilerimizi gösteriyoruz. Burada isteğimize göre bir hücre yapısı 
oluşturduktan sonra bunun için ve sqlite yapısı için gerekli olan sınıf yapılarımızı oluşturup sayfa üzerine bağladık. TableView protocollerini 
anasayfamıza extension yapısını kullanarak bağladıktan sonra hücreye tıklama özelliğini didRowSelect hazır fonksiyonu yardımı ile genel bir performsegue 
oluşturup not detay sayfasına geçişimizi sağladık. Oluşturduğumuz genel perform segue üzerinden aldığımız tıklanan hücrenin indeksini prepare fonksiyonu 
ile not detay sayfasına aktardık ve verilerimizi not detay sayfasında yeniden gösterdik. Burada ki iki adet gereksinimiz olan güncelleme ve silme 
gereksinimlerimizi Notlardao sınıfından yazmış olduğumuz fonksiyonlar sayesinde gerçekleştirebilmek için Notlardao sınıfından bir nesne oluşturduk ve 
gereksinimlerin gerçekleştirilmesini sağladık. Anasayfa üzerinde navigation component üzerinde yer alan nav bar button sayesinde veritabanımıza veri 
ekleyeçeğimiz not ekle sayfasına geçişimizi sağladık ve yine Notlardao sınıfından oluşturduğumuz fonksiyonları kullanarak veritabanına verilerimizi 
ekledik. Sayfalar arası geçişlerde gerek veri ekleme gerek ise veri güncelleme gibi gereksinimlerden sonra tableview yapısının stabil bir şekilde çalışıp 
anında güncellenebilmesi için Notlardao sınıfında oluşturduğumuz butunNotlarıGetir fonksiyonunu viewDidLoad methodu içerisinde değil viewWillApperance 
methodunda kullandık bu sayede proje de yaşam döngüsünüde kullanmış olduk. Projenin resimlerine aşağıdan ulaşabilirsiniz.  


<img src="https://i.hizliresim.com/7syxm4t.png" alt="alt text" width="280" height="500"> <img src="https://i.hizliresim.com/shkyc0o.png" alt="alt text" width="280" height="500"> <img src="https://i.hizliresim.com/5qwy74e.png" alt="alt text" width="280" height="500">
