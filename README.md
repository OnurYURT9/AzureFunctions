## AZURE FUNCTİON ÖZELLİKLERİ

Herhangi bir altyapı işlemine gerek kalmaksızın kodu ayağa kaldırıp serverless mimari inşa edilmesini sağlar.

Çoklu dil desteği sağlar.

Diğer Azure servislerle entegre çalışır.(Bindingler sayesinde gerçekleşir)

NPM, Nuget gibi paket yöneticileri kullanılabilir.
 ## AZURE FUNCTİON BAĞLI OLDUĞU SERVİSLER

Azure function oluştuğumuz zaman azure storage da oluşturmak zorundayız. Azure function içerisindeki durum bilgileri azure storage içerisinde tutulur. Bir tane Azure storage oluşturup birden fazla Azure function a bağlayabiliriz.

Application Insights: İsteğe bağlı olarak gelir. Bizim canlıya aldığımız uygulamamızın davranışlarını izlemememize imkan veren bir monitoring(izleme) işlemidir. Default oluşturunca enable olarak gelir.

## AZURE FUNCTİON TRİGGER TİPLERİ

Bir function çalışabilmesi için mutlaka tetiklenmesi gerekir.

Http Trigger ve Timer Trigger haricindeki trigger çeşitleri diğer azure servislerine bağlıdır. Http Trigger ve Timer trigger herhangi azure servis kullanmaz. Dışarıdan vereceğimiz komutlarla bu ikisini tetikleyebiliriz.

<strong>HttpTrigger:</strong> Httptrigger ile bir function oluşturduğumuzda bize endpoint verir bu endpointe istek yaptığımızda tigger tetiklenir.

<strong>TimerTrigger:</strong> Belli aralıklarla çalışacak kodumuzda tercih ederiz.

<strong>QueueTrigger:</strong> Kuyruğa mesaj yazıldığında tetiklenir.

<strong>BlobTrigger:</strong>  Blob'a yeni blob düştüğünde tetiklenir.

<strong>host.json:</strong>  Çalışacak function'la ilgili runtime ile ilgili bilgiler tutulur.

<strong>localsettings.json:</strong>  Development esnasında localde bilgiler tutulur. Canlıya cloud ortama gitmez.
