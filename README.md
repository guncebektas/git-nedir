# Git ve GitHub nedir? 

## Git nedir ve neden kullanılır?
  
Git, bir sürüm kontrol sistemi (Version Control System - VCS) olarak bilinen ve yazılım geliştirme süreçlerinde dosya değişikliklerini izlemek, yönetmek ve işbirliği yapmak için kullanılan bir yazılımdır. Git, yazılım geliştirme süreçlerini daha organize, güvenilir ve etkili bir hale getirmek için kullanılır. İşte Git'in ne olduğu ve neden kullanıldığına dair bazı önemli noktalar:

1. **Değişiklik İzleme:** Git, bir projenin tüm dosyalarındaki değişiklikleri sürekli olarak izler. Her bir değişiklik, bir "commit" adı verilen birimler halinde kaydedilir. Bu, geçmişteki her değişikliğe geri dönme ve belirli bir sürümü kurtarma imkanı sağlar.

2. **İşbirliği ve Ekip Çalışması:** Git, birçok geliştiricinin aynı projada birlikte çalışmasını kolaylaştırır. Farklı geliştiriciler aynı projada değişiklikler yapabilir, bu değişiklikleri paylaşabilir ve diğerlerinin de bu değişikliklere katkıda bulunmasına olanak tanır. İşbirliği yaparken çakışmaları önlemek için de birçok araç ve iş akışı sunar.

3. **Geliştirme Süreçlerinin İyileştirilmesi:** Git, geliştirme süreçlerini daha düzenli hale getirir. Farklı iş akışlarına (branch'ler) izin verir, bu da yeni özelliklerin geliştirilmesi veya hata düzeltilmesi gibi görevlerin izolasyonunu kolaylaştırır. Ayrıca, değişikliklerin doğrulanması (code review) ve otomatik entegrasyon (continuous integration) gibi süreçlere de destek sağlar.

4. **Hızlı ve Dağıtık Yapı:** Git, hızlı ve dağıtık bir sürüm kontrol sistemi olarak çalışır. Bu, internet bağlantısı olmadan bile çalışabilir ve farklı cihazlar arasında değişiklikleri senkronize edebilir.

5. **Açık Kaynak ve Ücretsiz:** Git, açık kaynaklı bir yazılımdır ve ücretsiz olarak kullanılabilir. Bu, herhangi bir projenin Git'i kullanarak verimli bir şekilde yönetmesini sağlar.

6. **Güvenilirlik ve Yedekleme:** Git, değişikliklerin güvenli bir şekilde saklanmasını sağlar. Bu, veri kaybını önler ve hatalı değişikliklerin geri alınabilmesini sağlar.

7. **Çeşitli Hizmet Sağlayıcılarla Entegrasyon:** Git, popüler bir bulut tabanlı hizmet olan GitHub, GitLab, Bitbucket ve daha birçok hizmetle entegre olabilir. Bu, projelerin bulut sunucularında depolanmasını, işbirliği yapılmasını ve güvenli bir şekilde paylaşılmasını sağlar.

Git, yazılım geliştirme projeleri için temel bir araç haline gelmiştir ve aynı zamanda belgelendirme, veri analizi ve daha birçok uygulama alanında da kullanılmaktadır. Öğrenilmesi ve kullanılması, geliştiriciler için büyük bir avantajdır ve projelerin daha iyi yönetilmesine yardımcı olur.

> Git'i Linus Torvalds adlı Linux işletim sistemini de yapan yazılımcı geliştirmiştir.

## Git'in çalışma mantığı: commit, branch, merge, ve rebase.

Mantığını temel kavramlarla açıklarsak:

1. **Repository(Depo):** Git projelerini yönetmek için kullanılan temel yapıdır. Bir depo, projenin tüm dosyalarını, tarihçesini ve değişikliklerini içerir. Projenin tüm bilgileri burada saklanır.

2. **Commit (Taahhüt):** Değişikliklerin depoda kaydedildiği bağımsız birimlerdir. Her commit, bir dizi değişikliği içerir ve bir açıklama ile etiketlenir. Bu, projenin geçmişini oluşturur.

3. **Branch (Dal):** Git, projenin farklı dallarını kullanma yeteneği sağlar. Her dal, projenin farklı bir iş akışını veya sürümünü temsil eder. Ana dal genellikle "master" veya "main" olarak adlandırılır.

4. **Değişiklik Takibi:** Git, projedeki her dosyanın tüm değişikliklerini kaydeder. Bu, her dosyanın her committeki değişiklikleri saklamasını ve geçmişe erişilebilmesini sağlar.

5. **İşbirliği ve İletişim:** Git, birden fazla geliştiricinin aynı projada birlikte çalışmasını kolaylaştırır. Değişiklikler uzak depolarda saklanabilir ve geliştiriciler arasında paylaşılabilir. Bu, işbirliği senaryolarını destekler.

6. **Merge (Birleştir) ve Rebase(Yeniden Temel Al):** Farklı dallardaki değişikliklerin ana dal ile birleştirilmesi veya yeniden temel alınması Git'in temel işlemlerindendir. Bu, farklı geliştiricilerin veya iş akışlarının sonuçlarını birleştirmek için kullanılır.

7. **Distributed (Dağıtık Yapı):** Git, her geliştiriciye kendi kopyasını alabilme ve bağımsız olarak çalışabilme yeteneği sunar. Sonradan bu değişiklikler merkezi bir sunucuda birleştirilir.

Bu çalışma mantığı, Git'in projelerin sürüm kontrolünü, işbirliğini ve değişikliklerin takip edilmesini yönetmek için kullanıldığı temel prensiplerdir. Git, yazılım geliştirme, belge yönetimi ve diğer birçok alan için yaygın olarak kullanılan güçlü bir araçtır.

- Temel Git komutları: git init, git clone, git add, git commit, git push, git pull, git branch, git merge, vb. 

1. **`git init` (Depo Oluştur):** Bir Git "repository"i oluşturmak için kullanılır. Bu komut, mevcut bir klasörü Git depo haline getirir.

   ```bash
   git init
   ```

2. **`git clone` (Klonla):** Uzak bir Git "repository"sine yerel makinenize kopyalamak için kullanılır.

   ```bash
   git clone https://github.com/guncebektas/git-nedir.git
   ```

3. **`git add` (Ekle):** Değişiklikleri bir sonraki "commit"e eklemek için kullanılır. Değişiklik yapılan dosyaları izler.

   ```bash
   git add dosya.txt
   ```

4. **`git commit` (Taahhüt Et):** Staged (eklenmiş) değişiklikleri "repository"e kaydetmek için kullanılır. Her "commit" bir açıklama mesajı ile birlikte gelir.

   ```bash
   git commit -m "İlk commit: Projeye hoş geldiniz!"
   ```

5. **`git push` (Gönder):** Yerelde yapılan "commit"i uzak Git sunucusuna göndermek için kullanılır.

   ```bash
   git push origin master
   ```

6. **`git pull` (Çek):** Uzak sunucudan yerel makineye değişiklikleri çekmek için kullanılır.

   ```bash
   git pull origin master
   ```

7. **`git branch` (Dal):** Projede mevcut "branch"leri listelemek veya yeni bir branch oluşturmak için kullanılır.

   ```bash
   git branch
   git branch new-branch
   ```

8. **`git merge` (Birleştir):** Farklı "branch"lerdeki değişiklikleri birleştirmek için kullanılır.

   ```bash
   git merge hotfix
   ```

Bu komutlar, Git'i temelde nasıl kullanacağınızı gösteren önemli işlemleri içerir. Her bir komut, projelerin sürüm kontrolünü, işbirliğini ve değişikliklerin takibini sağlar. Örnekler, bu komutların nasıl kullanılacağını daha iyi anlamanıza yardımcı olacaktır.

## Temel Git İş Akışı:

### Bir Git "repository"si oluşturma ve klonlama.

Temel Git iş akışı, Git'i kullanarak bir projeyi sürüm kontrolü altına almak, değişiklikleri takip etmek ve işbirliği yapmak için izlenen adımları içerir. İşte temel Git iş akışının ana hatları:

1. **Repository Oluşturma:**
    - Projeyi Git "repository"si haline getirmek için yerel bir klasörde `git init` komutunu kullanarak bir "repository" oluşturun.

2. **Değişiklikleri İzleme (Staging):**
    - Projede yapılan değişiklikleri Git'e izlettirmek için `git add` komutunu kullanın. Bu, değişiklikleri "sahneye" koymak anlamına gelir, yani bir sonraki "commit"e dahil edilmesi gereken değişiklikleri belirler.

3. **Taahhüt (Commit) Oluşturma:**
    - İzlenen (staged) değişiklikleri yerel "repository"e kaydetmek için `git commit` komutunu kullanın. Her "commit" bir açıklama ile birlikte gelmelidir, böylece bu "commit"ler anlamlı hale gelir.

4. **Uzak Depoya Taşıma (Push):**
    - Yerelde yapılan taahhütleri uzak bir Git sunucusuna göndermek için `git push` komutunu kullanın. Bu, işbirliği yaparken diğer geliştiricilerin değişikliklerinizi görmelerini sağlar.

5. **Değişiklikleri Alma (Pull):**
    - Diğer geliştiricilerin yaptığı değişiklikleri almak için `git pull` komutunu kullanın. Bu, uzak sunucudan yerel makinenize değişiklikleri çeker.

6. **Yeni Dallar Oluşturma:**
    - Projede farklı iş akışlarını veya özellikleri izlemek için yeni "branch"ler oluşturabilirsiniz. `git branch` komutu ile mevcut "branch"leri ve `git checkout -b new-branch` ile yeni bir "branch" oluşturabilirsiniz.

7. **Dalları Birleştirme (Merge) veya Temel Üzerine Alma (Rebase):**
    - Farklı dallardaki değişiklikleri ana dala "merge" etmek veya "rebase" etmek için `git merge` veya `git rebase` komutlarını kullanabilirsiniz.

### Farklı branch'lerde çalışma ve değişiklikleri birleştirme (merge ve rebase).

Çalışmanız tamamlandığında ve değişikliklerinizi ana "branch"a eklemek istediğinizde, bu adımları izleyebilirsiniz:

Master "branch"a geçiş yapmak için:

```bash
git checkout master
```

Master ile farklı "branch"ı birleştirmek için:

```bash
git merge hotfix
```

> "Cherry-pick," Git ile çalışırken belirli bir taahhüdü (commit) istediginiz bir "branch"e uygulamanızı sağlayan işlemdir. Bu, belirli bir taahhüdün değişikliklerini kopyalamak istediğinizde ve tüm bir dalı birleştirmek yerine sadece belirli değişiklikleri almak istediğinizde kullanışlıdır.

Veya "hotfix"i master üzerine kopyalamak için:

```bash
git rebase hotfix
```

> Not: Rebase işlemi, değişikliklerinizi yeni dalın en son haline getirir ve daha temiz bir geçmiş oluşturur. Ancak rebase işlemi sıkça kullanıldığında projenizin tarihçesi karmaşık hale gelebilir.

"rebase" işlemi yanlış kullanıldığında veya dikkatsizce uygulandığında, bazı riskler ve olumsuz sonuçlar doğurabilir. İşte rebase yapmanın zararları ve dikkat edilmesi gereken noktalar:

Geçmişi Değiştirebilir: Rebase işlemi, geçmişteki taahhütleri değiştirebilir veya yeniden düzenleyebilir. Bu, projenin tarihçesini karmaşık hale getirebilir ve başkalarının geçmiş taahhütleri üzerinde çalışmasını zorlaştırabilir.

Çakışma Sorunları: Eğer rebase sırasında çakışma (conflict) oluşursa, bu çakışmaları çözmek gerekecektir. Çözülen çakışmalar hatalı olabilir ve projenin işleyişini etkileyebilir.

İnceleme ve İzleme Sorunları: Proje tarihçesini değiştirmek, geçmiş taahhütleri üzerinde yapılan incelemeleri ve izlemeyi etkileyebilir. Bu, geçmişte neyin neden değiştirildiğini anlamayı zorlaştırabilir.

İşbirliği Sorunları: Ekip üyeleri, rebase işlemi sırasında taahhütlerini yeniden düzenlediğinde, diğer ekip üyelerinin çalışmaları üzerinde olumsuz etkiler yaratabilir.

Kod Kaybı: Rebase sırasında hatalı bir işlem veya yanlış taahhüt seçimi, kodun kaybolmasına neden olabilir.

Bu nedenlerle, rebase işlemini dikkatli bir şekilde ve projenin gereksinimlerine uygun olarak yapmalısınız. Projenizin ana dalı üzerinde rebase yapmadan önce, projenin diğer katılımcılarıyla iyi bir iletişim içinde olmalı ve rebase işleminin potansiyel risklerini ve sonuçlarını anlamalısınız. Eğer projenizin sürekli rebase yapılmasına veya geçmişin sürekli değiştirilmesine ihtiyacı yoksa, diğer dal birleştirme (merge) stratejilerini düşünmelisiniz.

4. Çakışma Çözümleme (Eğer Gerekiyorsa):

Eğer yeni dalınız ile ana dalınız arasında çakışma (conflict) varsa, bu çakışmaları elle çözmelisiniz. Git size çakışmaları belirten dosyaları gösterecektir. Çakışmaları çözdükten sonra değişiklikleri git add ve git commit ile kaydedebilirsiniz.

5. Uzak Sunucuya Taşıma (Push):

Değişikliklerinizi uzak sunucuya (örneğin GitHub) taşımak için:

```bash
git push origin master
```

Bu işlem, değişikliklerinizi diğer geliştiricilerle paylaşmanızı sağlar.

Bu adımları takip ederek farklı dallar üzerinde çalışabilir ve değişiklikleri ana dala birleştirebilirsiniz. Bu sayede farklı iş akışları ve özellik geliştirmelerini yönetmek daha düzenli ve etkili bir hale gelir.

## İşbirliği ve Pull Requestler:

### İşbirliği yaparken fork, clone, ve pull requestlerin nasıl kullanılacağı.

İşbirliği yaparken "fork", "clone" ve "pull request" terimleri Git tabanlı iş akışlarında oldukça yaygın kullanılır. Bu terimleri ve nasıl kullanılacaklarını aşağıda açıklıyorum:

**1. Fork (Çatal):**
- "Fork" işlemi, başka bir geliştiricinin projesini kendi GitHub hesabınıza kopyalamak anlamına gelir. Bu, projenin bir kopyasını almanızı sağlar ve bu kopyayı kendi hesabınızda yönetebilirsiniz.
- Fork işlemi için projenin GitHub sayfasında sağ üst köşede bulunan "Fork" düğmesini tıklamanız yeterlidir.

**2. Clone (Klonla):**
- "Clone" işlemi, bir projenin kopyasını yerel makinenize indirmenizi sağlar. Bu, projeyi düzenleyip yerelde çalışmanız için gerekli bir adımdır.
- Kopyalamak istediğiniz projenin GitHub sayfasında "Code" düğmesini tıklayın ve oradaki URL'yi kullanarak aşağıdaki komutu çalıştırın:

   ```bash
   git clone https://github.com/kullanici/proje.git
   ```

**3. Pull Request (Çekme İsteği):**
- "Pull Request" (kısaca PR), projenizin değişikliklerini başka bir projenin ana dalına entegre etmek için kullanılır. Bu, projeye katkıda bulunmak istediğinizde kullanılır.
- Kendi forkladığınız projenizdeki değişiklikleri yapın ve bunları taahhüt (commit) edin. Ardından, değişikliklerinizi ana projeye eklemek için "Pull Request" oluşturun.
- Projenin GitHub sayfasında "Pull Request" düğmesine tıklayarak yeni bir istek başlatabilirsiniz. Değişiklikleriniz incelenir ve ana projeye eklenir veya reddedilir.

Bu işlemler, açık kaynak projelere katkıda bulunurken veya işbirliği yaparken sık sık kullanılır. Projelerin sahipleri, katkıda bulunanların değişikliklerini inceleyebilir ve bu sayede projelerin daha iyi ve güncel tutulmasına yardımcı olabilir.

### İşbirliği için iş akışları ve roller (örneğin, katkıda bulunan, inceleyici).

İşbirliği için Git tabanlı iş akışları ve roller, projelerin düzgün bir şekilde yönetilmesini ve geliştiricilerin etkili bir şekilde bir arada çalışmasını sağlamak için çok önemlidir. İşte bu iş akışlarının temelini oluşturan bazı roller ve iş akışları:

**1. Katkıda Bulunan (Contributor):**
- Katkıda bulunanlar, projeye kod, dokümantasyon veya diğer kaynaklarla katkıda bulunan geliştiricilerdir.
- Katkıda bulunanlar, projeyi çatallayabilir, yerel makinelerinde klonlayabilir, değişiklikler yapabilir, bu değişiklikleri kendi "fork"larında saklayabilir ve sonrasında "pull request" oluşturarak değişikliklerini ana projeye ekleyebilirler.

> "İşbirliği yaparken, katkıda bulunanlar (contributors) için Katkı Lisans Anlaşması (CLA) oldukça önemlidir ve bazı projeler CLA'ları gereksinim olarak koymaktadır. CLA, projeye katkıda bulunanların ve projenin sahibi veya yöneticisi arasında belirli hükümleri ve taahhütleri tanımlayan bir anlaşmadır. Katkıda bulunanlar, projeye katkıda bulunmaya başlamadan önce CLA'yı kabul etmelidir. Bu genellikle bir çevrimiçi formun doldurulması veya bir dosyanın elektronik imzalanması ile gerçekleştirilir. CLA'nın amacı, projeye katkıda bulunanların katkılarının kullanımı, lisansı ve hakları hakkında net ve standart bir anlayış sağlamaktır. Bu, projenin sahibi veya yöneticisi ile katkıda bulunanlar arasında açık bir iletişim ve anlayışın korunmasına yardımcı olur. Projelerin kullanıcıların katkılarını daha iyi yönetebilmeleri ve telif hakkı, patent hakları ve diğer hukuki konuları ele almaları için CLA kullanmaları oldukça yaygındır. CLA, hem projeye katkıda bulunanların hem de projenin kendisinin korunmasına yardımcı olur."

**2. İnceleyici (Reviewer):**
- İnceleyiciler, projeye gönderilen "pull request"leri gözden geçiren ve değişiklikleri onaylayan veya geri gönderen kişilerdir.
- İnceleyiciler, kod incelemesi yaparlar, çakışmaları çözerler ve değişikliklerin kod kalitesine ve proje gereksinimlerine uygun olup olmadığını değerlendirirler.

**3. Proje Sahibi (Project Owner):**
- Proje sahipleri, projenin ana yöneticileridir ve projenin son karar vericileridir.
- Projeyi sahiplenir, proje gereksinimlerini tanımlar, katkıda bulunanları ve inceleyicileri yönlendirir ve projenin gelişimini denetler.

**4. İş Akışları:**

a. **Merkezi İş Akışı (Centralized Workflow):**
- Bu iş akışında, projenin ana dalı korunur ve sadece incelemeler sonrası onaylanmış değişiklikler ana dala entegre edilir.
- Katkıda bulunanlar, her bir değişiklik için yeni bir dal oluşturur, değişikliklerini bu dalda yapar, ardından "pull request" açarlar.
- İncelemeler ve onaylar sonrası değişiklikler ana dala "merge" edilir.

b. **Dal İş Akışı (Feature Branch Workflow):**
- Bu iş akışında, her yeni özellik veya değişiklik kendi dalında geliştirilir.
- Katkıda bulunanlar, yeni bir özellik eklemek istediklerinde yeni bir dal oluşturur, bu dalda çalışır ve sonra ana dala geri birleştirme yapar.
- Her özellik veya değişiklik kendi dalında geliştirildiğinden, çakışmalar daha az olur.

c. **Fork İş Akışı (Forking Workflow):**
- Bu iş akışı, katkıda bulunanların projeyi kendi hesaplarına çatalamalarına dayanır. Her katkıda bulunan kendi çatalı üzerinde değişiklik yapar ve sonra bir "pull request" ile ana projeye katkıda bulunur.

İşbirliği iş akışları ve roller, projenin boyutuna, karmaşıklığına ve ihtiyaçlarına bağlı olarak değişebilir. Hangi iş akışının ve rollerin projeniz için en uygun olduğunu seçerken, projenizin hedeflerini ve gereksinimlerini dikkate almalısınız.

### Pull Requestlerin (PR) incelenme süreçleri.

Proje sahipleri veya inceleyiciler tarafından pull requestler incelendikten sonra aşağıdaki süreçlerden biri izlenir:

İnceleme: Pull request inceleyicileri (reviewer), değişiklikleri inceler ve gerektiğinde önerilerde bulunur. İncelemeler, kod kalitesi, güvenlik, performans ve uyumluluk gibi çeşitli faktörleri içerebilir.

Gerektiğinde Değişiklikler: İncelemeler sonucunda değişiklikler yapılması gerekebilir. Katkıda bulunan bu değişiklikleri yapar ve taahhüt eder.

Onay: İncelemeler tamamlandığında ve değişiklikler kabul edildiğinde, bir inceleyici veya proje sahibi pull request'i onaylar ve projeye entegre eder. Bu işlem "merge" olarak adlandırılır.

Geri İade: İncelemeler sonucunda değişikliklerin kabul edilmediği durumlarda, inceleyici veya proje sahibi pull request'i reddedebilir. Katkıda bulunan bu durumda değişiklikleri yapar ve tekrar bir pull request oluşturur.

Pull requestler, açık kaynak projelerde ve işbirliği içinde çalışan geliştiriciler arasında yaygın bir iş akışıdır. Bu süreç, değişikliklerin açıkça incelenmesine ve projeye kontrollü bir şekilde entegre edilmesine yardımcı olur.

### Git Sorun Giderme: (PR açın)

Hataları tanımlama ve çözme (örneğin, çakışmalar).
Git log ve git reflog komutlarını kullanarak geçmişi inceleme.
Git reset ve git revert komutlarıyla geri alma işlemleri. 

## GitHub Actions

GitHub Actions, GitHub tarafından sunulan entegre sürekli entegrasyon (CI) ve sürekli dağıtım (CD) hizmetidir. GitHub Actions, GitHub repositorileri ile entegre bir şekilde çalışır ve otomatikleştirilmiş iş akışları oluşturmanıza, testleri çalıştırmanıza, uygulamaları dağıtmanıza ve diğer yazılım geliştirme işlemlerini otomatize etmenize olanak tanır. GitHub Actions, projelerinizi daha hızlı ve güvenilir bir şekilde geliştirmenize yardımcı olur.

GitHub Actions'ın bazı temel özellikleri şunlardır:

1. **Otomatik İş Akışları:** GitHub Actions ile, belirli bir olay (örneğin, taahhüt yapıldığında veya yeni bir çekme isteği açıldığında) gerçekleştiğinde otomatik iş akışları çalıştırabilirsiniz.

2. **Çoklu Platform Desteği:** GitHub Actions, Linux, macOS ve Windows gibi farklı işletim sistemleri üzerinde işlem yapabilen iş akışları oluşturmanıza olanak tanır.

3. **İşlem Hızı:** GitHub Actions, hızlı ve ölçeklenebilir bir altyapı üzerinde çalışır, bu da iş akışlarınızın hızlı bir şekilde tamamlanmasını sağlar.

4. **Dil ve Çerçeve Desteği:** Birden fazla programlama dili ve test çerçevesini destekler, bu nedenle çeşitli projelerde kullanılabilir.

5. **Güvenlik ve Erişim Kontrolleri:** İş akışları, erişim kontrolü ve güvenlik önlemleri ile güvence altına alınabilir.

GitHub Actions, yazılım geliştirme süreçlerini daha düzenli ve güvenilir hale getirir. Projelerinizin otomatik olarak derlenmesi, test edilmesi ve dağıtılması gibi işlemler, hataların daha hızlı tespit edilmesini ve kod kalitesinin artırılmasını sağlar. Ayrıca, bu süreçlerin otomatize edilmesi, geliştiricilerin daha fazla zamanlarını yazılım geliştirmeye ve inovasyona odaklanmalarına yardımcı olur.

> GitHub Actions kullanırken sınırlamalar daha fazladır. Genellikle aylık 2000 dakika ücretsiz çalışma süresi sunulur ve aynı zamanda 2 eşzamanlı çalışma sınırlaması bulunur.

## Anlamlı commit mesajları yazmak
Anlamlı commit mesajları yazmak, kod tabanınızın geçmişini, değişikliklerin nedenini ve ne zaman yapıldığını daha iyi anlamanıza ve işbirliği yapmanıza yardımcı olur. İşte anlamlı commit mesajları yazmanıza yardımcı olacak bazı en iyi uygulamalar:

1. **Başlık ve Açıklama:** Commit mesajlarını iki bölüme ayırın: başlık (title) ve açıklama (description). Başlık, değişikliğin özetini içermeli ve bir cümlenin sonunda nokta ile bitmelidir. Açıklama ise değişikliğin ayrıntılarını içermelidir.

2. **Özgün ve Öznel Olun:** Commit mesajlarınız, değişikliğin ne yaptığını ve neden yapıldığını açıklamalıdır. Özgün olun ve sadece neyi değil, nedeni de açıklayın.

3. **İş Akışı Bağlamı:** Commit, hangi iş akışı veya sorunu düzelttiğini belirtmelidir. Özellikle büyük projelerde bu, işbirliği yapmayı kolaylaştırır.

4. **Referanslar:** Commit mesajlarına, ilgili sorun takip numarası, bağlantı veya referanslar ekleyin. Bu, değişikliklerin hangi sorunları giderdiğini izlemeyi kolaylaştırır.

5. **Özlü ve Açık Olun:** Commit mesajlarınız özgün ve açık olmalıdır, ancak gereksiz uzun olmamalıdır. Gereksiz ayrıntılara girmeden özlü bir şekilde ifade edilmelidir.

6. **Fiil Kullanımı:** Commit başlığı fiil içermelidir ve bu fiil, neyin değiştirildiğini belirtmelidir. Örneğin, "Ekle", "Düzelt", "Güncelle" gibi fiiller kullanılabilir.

7. **Dil ve Yazım Kuralları:** Commit mesajlarınızı dilbilgisi ve yazım kurallarına uygun bir şekilde yazmaya özen gösterin. Dikkatsizce yazılmış mesajlar karmaşıklığa neden olabilir.

8. **Daha Fazla Taahhüt Yapın:** Büyük değişiklikleri küçük ve bağımsız taahhütlere bölmek, her taahhüdün daha açık ve anlamlı olmasını sağlar.

İşte bir örnek anlamlı commit mesajı:

```
Başlık: "README.md dosyasına projenin başlığı eklendi"

Açıklama: "README.md dosyasına projenin başlığı eklendi. Bu, projenin daha açık ve anlaşılır olmasını sağlar ve belgelerin kullanıcılar tarafından daha kolay bulunmasını sağlar."
```

Anlamlı commit mesajları, projenizin geçmişini anlamak ve işbirliği yapmak için önemlidir. Bu, projenizin uzun vadeli sürdürülebilirliğine katkıda bulunur ve gelecekteki geliştiricilere rehberlik eder.

### Standart Commit Ön Ekleri:
Commit mesajlarınızı daha tutarlı ve anlamlı hale getirmek için standart commit ön ekleri kullanılabilir. Standart bir ön ek seti, commit mesajının başlığında yer alır ve değişikliğin ne tür bir işlevi veya değişikliği temsil ettiğini belirtir. İşte bazı yaygın kullanılan commit ön ekleri:

feat: Yeni bir özellik (feature) eklemek için kullanılır. Örneğin: "feat: Kullanıcı kaydı ekleme özelliği"

fix: Bir hata veya sorunu düzeltmek için kullanılır. Örneğin: "fix: Veri tabanı bağlantı hatası giderildi"

docs: Dokümantasyonu güncellemek için kullanılır. Örneğin: "docs: Kullanım kılavuzu güncellendi"

style: Kod stilini düzeltmek veya geliştirmek için kullanılır. Örneğin: "style: İmla hataları düzeltildi"

refactor: Kodu yeniden düzenlemek veya optimize etmek için kullanılır. Örneğin: "refactor: Veritabanı erişim kodu yeniden düzenlendi"

test: Testleri eklemek veya güncellemek için kullanılır. Örneğin: "test: Kullanıcı girişi testleri eklendi"

chore: Rutin işler veya işlem dışı değişiklikler için kullanılır. Örneğin: "chore: Bağımlılıkları güncelleme"

Bu ön ekler, commit mesajlarına daha fazla anlam eklemenize ve bir projenin geçmişini daha iyi izlemenize yardımcı olabilir. Ayrıca, bazı CI/CD araçları veya otomatik sürümleme araçları, bu ön ekleri kullanarak otomatik işlemleri tetikleyebilir veya bir sürüm notu oluşturabilir.

### Husky Kullanımı
Husky, Git taahhütlerinizin kalitesini ve tutarlılığını artırmak için kullanabileceğiniz bir ön taahhüt (pre-commit) ve ön taahhüt sonrası (pre-commit) kancaları yönetme aracıdır. Bu, taahhütlerinizi göndermeden önce belirli kurallara ve işlemlere uymayı zorunlu kılar. Örneğin, kod denetimlerini otomatize edebilir, testleri çalıştırabilir veya commit mesajlarına belirli bir formatı zorlayabilirsiniz.

## .gitignore dosyası oluşturma.

.gitignore dosyası, Git deposunda izlenmemesi gereken dosyaları ve klasörleri tanımlamanıza yardımcı olan bir dosyadır. Bu dosya, özellikle proje klasörünüzdeki geçici veya üretilen dosyaları ve özel yerel yapılandırmaları dışarıda bırakmanız gerektiğinde oldukça faydalıdır. İşte bir .gitignore dosyası oluşturma adımları:

1. Proje Dizininde .gitignore Dosyası Oluşturun:
    - Projenizin ana dizinine gidin.
    - Burada bir `.gitignore` adında yeni bir dosya oluşturun.

2. Düzenleyici veya Metin Düzenleyici Kullanarak .gitignore Dosyasını Düzenleyin:
    - `.gitignore` dosyasını açın ve izlenmemesi gereken dosyaları ve klasörleri tanımlamak için kurallar ekleyin.
    - Her satırda bir kural ekleyin ve kural, izlenmeyecek dosyanın veya klasörün adını veya kalıbını içermelidir.

Örnek bir `.gitignore` dosyası:

```gitignore
# Bu, yorum satırıdır ve .gitignore dosyasını açıklar.

# Belirli bir dosya veya klasörü izlememek için:
dosya.txt
veriler/

# Belirli uzantılara sahip dosyaları izlememek için:
*.log
*.tmp

# Belirli klasör yapısını izlememek için:
node_modules/
build/
```

- `#` işareti ile başlayan satırlar yorum satırlarıdır ve açıklamalar eklemek için kullanılır.
- Dosya veya klasör adları, doğrudan belirtilen adlara sahip dosyaları veya klasörleri izlememek için kullanılır.
- Yıldız (*) işareti ile başlayan kural, belirli bir uzantıya sahip tüm dosyaları temsil eder.
- Klasör adları eğer sonunda / işareti ile bitiyorsa, o klasörün içindeki tüm dosyaları ve alt klasörleri temsil eder.

3. .gitignore Dosyasını Depoya Ekleyin ve Taahhüt Edin:
    - `.gitignore` dosyasını proje deposuna eklemek için aşağıdaki komutları kullanabilirsiniz:

      ```bash
      git add .gitignore
      git commit -m "Git ignore dosyası eklendi"
      ```

4. .gitignore Dosyasını Depoya Taahhüt Edin:
    - .gitignore dosyasını taahhüt ettikten sonra, depoya göndermek için `git push` komutunu kullanabilirsiniz.

Bu adımları takip ederek, Git depolarınızda izlenmemesi gereken dosyaları ve klasörleri belirtmek için .gitignore dosyası oluşturabilir ve yönetebilirsiniz.

## Lisanslama ve Etik Sorunlar

Yazılım geliştirme ve paylaşma süreçlerinde lisanslama ve etik konular önemlidir. İşte bu konularda dikkate almanız gereken bazı önemli konular:

### Lisanslama:
Lisanslar, yazılımın kullanım, paylaşım ve değiştirilme koşullarını belirler. Yazılım geliştiricileri ve kullanıcıları için açık ve net bir yol haritası sağlarlar. İşte bazı yaygın yazılım lisansları:

1. **GPL (GNU Genel Kamu Lisansı):** Bu lisans, açık kaynak yazılımın özgürce kullanılmasını ve değiştirilmesini teşvik eder. Ancak, değişikliklerin kaynak kodunu da paylaşma zorunluluğu vardır.

2. **MIT Lisansı:** Bu lisans, yazılımın özgürce kullanılmasını ve değiştirilmesini sağlar. Kaynak kodunun paylaşılma zorunluluğu yoktur.

3. **Apache Lisansı:** Bu lisans, açık kaynak yazılımı ticari projelerde kullanmaya izin verir. Değişikliklerin kaynak kodunu paylaşma gerekliliği vardır.

4. **Creative Commons Lisansları:** Bu lisanslar, özellikle içerik oluşturucular için tasarlanmıştır ve içeriklerin paylaşılma ve kullanılma koşullarını belirler.

5. **Unlicense:** Unlicense, yazılımı kamuya mal etmek için kullanılan bir lisans türüdür. Kaynak kodunun serbestçe kullanılmasını ve değiştirilmesini sağlar.

### Etik Sorunlar:
Yazılım geliştiricileri ve kullanıcıları aşağıdaki etik sorunlara dikkat etmelidir:

1. **Telif Hakkı ve Lisanslar:** Başka bir kişinin veya projenin telif hakkına, lisans koşullarına ve kullanım haklarına saygı göstermek önemlidir.

2. **Kullanıcı Verileri ve Gizlilik:** Kullanıcıların verilerini korumak ve gizliliğini sağlamak etik bir sorumluluktur. Veri toplama ve işleme işlemleri yasal ve dürüst olmalıdır.

3. **Açık Kaynak Katkıları:** Açık kaynak projelere katkı yaparken, topluluğun kurallarına ve standartlarına uymak gerekir.

4. **İşbirliği ve Saygı:** Yazılım geliştirme süreçlerinde işbirliği yaparken diğer geliştiricilere saygı göstermek ve çatışmaları olumlu bir şekilde çözmek etik bir yaklaşımdır.

5. **Sosyal Sorumluluk:** Yazılımın toplumsal ve çevresel etkilerini düşünmek, sürdürülebilir ve toplum için faydalı projelere katkıda bulunmak etik bir yaklaşımdır.

6. **Ayrımcılık Karşıtlığı:** Kullanıcılar ve geliştiriciler arasında ayrımcılığa ve ayrımcılığa yol açabilecek davranışlardan kaçınmak önemlidir.

Lisanslama ve etik konular, yazılım geliştirme süreçlerinde sorumluluk ve saygıyı teşvik eder. Projelerinizde doğru lisansı seçmek ve etik kurallara uymak, hem topluluğa hem de gelecekteki kullanıcılara fayda sağlar.


