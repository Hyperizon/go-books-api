# Go Book API

Go Book API, PostgreSQL veritabanı ile birlikte Go dilinde yazılmış bir kitap API'sidir. Bu API ile kitaplar hakkında bilgi edinebilir, kitap ekleyebilir, silebilir ve listeyebilirsiniz. Ayrıca, RESTful kurallarına uygun olarak tasarlanmıştır.

## Özellikler

- Kitap ekleme: `POST /create_book` endpointi ile yeni bir kitap ekleyebilirsiniz. Kitabın başlığı, yazarı, yayıncısı gibi bilgileri JSON formatında göndermeniz gerekmektedir.
- Kitap silme: `DELETE /delete_book/{id}` endpointi ile veritabanındaki bir kitabı silebilirsiniz. Kitabın ID numarasını URL parametresi olarak göndermeniz gerekmektedir.
- Kitap listeleme: `GET /books` endpointi ile veritabanındaki tüm kitapları listeleyebilirsiniz. Ayrıca, `GET /get_book/{id}` endpointi ile belirli bir kitabın detaylarını alabilirsiniz.


## Avantajlar

- Go Book API, Go'nun hızlı, basit ve güvenli bir dil olması sayesinde performanslı ve güvenilir bir uygulamadır.
- Go Book API, PostgreSQL veritabanı ile çalışarak verilerinizi güvenli ve kalıcı bir şekilde saklar.
- Go Book API, RESTful kurallarına uygun olarak tasarlanmıştır. Bu sayede, uygulamanızın bakımı ve geliştirilmesi kolaylaşır.

## Kurulum

Uygulamayı çalıştırmak için aşağıdaki adımları izleyin:

1. Projeyi GitHub'dan indirin veya klonlayın: `git clone https://github.com/Hyperizon/go-books-api.git`
2. Projeyi indirdiğiniz dizine gidin: `cd go-books-api`
3. PostgreSQL veritabanınızı oluşturun.
4. `.env` dosyasını oluşturun ve içine veritabanı bağlantı bilgilerinizi yazın. Örnek bir `.env` projede mevcuttur inceleyebilirsiniz.
5. Uygulamayı derleyin: `go build`
6. Uygulamayı çalıştırın: `./go-books-api`
7. Tarayıcınızda veya Postman gibi bir araçta `http://localhost:3000` adresine gidin.

## Bağımlılıklar

Uygulama aşağıdaki bağımlılıkları kullanmaktadır:

- [Fiber]: Web çatısı olarak Fiber'i kullanır.
- [Gorm]: Veritabanı işlemleri için Gorm ORM'i kullanır.
- [Godotenv]: Ortam değişkenlerini okumak için Godotenv'i kullanır.

## Lisans

Bu proje [MIT Lisansı] ile lisanslanmıştır.

## Katkı

Bu projeye katkıda bulunmak isterseniz, lütfen aşağıdaki adımları izleyin:

1. Projeyi forklayın.
2. Yeni bir dal oluşturun: `git checkout -b feature/your-feature`
3. Değişikliklerinizi ekleyin ve kaydedin: `git add .` ve `git commit -m "Your feature"`
4. Dalınızı GitHub'a gönderin: `git push origin feature/your-feature`
5. Bir pull request oluşturun.
