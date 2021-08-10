## Bu sunum hakkında

- https://revealjs.com/
- Sunumun kaynak kodlarını şurada bulabilirsiniz: https://gitlab.piworks.net/ismailarilik/gitlab-ci-presentation


![](https://import.viva64.com/docx/blog/0710_DevOps_vs_DevSecOps/image2.png)


![](https://princepatni.com/wp-content/uploads/2020/12/princepatni.com-Devops.png)


## GitLab

1. 2011'de Dmytro Zaporozhets ve Valery Sizov isimli iki Ukraynalı geliştiri tarafından kuruldu.
1. Ruby on Rails ile yazıldı. Sonrasında bazı kısımları performans nedeniyle Go ile yeniden yazıldı. Frontend'de bir süredir Vue.js kullanılıyor.
1. 2015'te Y Combinator'a katılmasıyla büyümesi hızlandı.
1. Açık kaynak bir proje. Ücretli özellikleri de açık kaynak ancak lisansı farklı.
1. 67 ülkeden çalışanların tümü uzaktan çalışıyor.
1. Herkes [**kolayca**](https://gitlab.com/gitlab-org/gitlab/-/issues?scope=all&state=opened&label_name[]=Accepting%20merge%20requests&label_name[]=good%20for%20new%20contributors) katkıda bulunabilir.


## GitLab CI/CD

[ismailarilik/loading/.gitlab-ci.yml](https://gitlab.piworks.net/ismailarilik/loading/-/blob/master/.gitlab-ci.yml)


## Semantic Versioning

Sürüm: MAJOR.MINOR.PATCH
Örnek: 1.2.3

### Kurallar

- Önceki sürümler ile uyumlu olmayan nispeten büyük değişiklikler için MAJOR değiştirilir: 2.0.0
- Önceki sürümler ile uyumlu nispeten küçük değişiklikler için MINOR değiştirilir: 1.3.0
- Hata düzeltmeleri gibi küçük değişiklikler için PATCH değiştirilir: 1.2.4


## semantic-release

1. Koşulları doğrula
1. Son sürümü al
1. Commit'leri analiz et
1. Release'i doğrula
1. Notları oluştur
1. Git tag'lerini oluştur
1. Hazırla
1. Yayınla
1. Bildir

Note:

1. Koşulları doğrula: Ön kontrol; konfigürasyon doğru mu, authentication token doğru mu, vb.
1. Son sürümü al: Bir üst sürümü belirlemek için
1. Commit'leri analiz et: Sürümün tipini (major, minor ya da patch) belirlemek için
1. Release'i doğrula: Sürüm numarası, tipi, etiketi, vb. parametreleri doğrula
1. Notları oluştur: Sürüm notlarını oluşturur
1. Git tag'ini oluştur: Yeni sürüm için bir git tag'i oluşturur
1. Hazırla: Yeni sürümü hazırlamaktan sorumlu. Örneğin; package.json, [CHANGELOG dosyası](https://keepachangelog.com/), belgelendirme ve derlenmiş çıktıları günceller ya da oluşturur. Sonrasında bir commit push eder. 
1. Yayınla: Sürümü yayınlar.
1. Bildir: Yeni sürümü ya da yayınlama hatalarını bildirir.
