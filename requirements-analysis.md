# Requirements Analysis

## 1. Qeydiyyat prosesi

Sistem namizədlərin mərkəzləşdirilmiş elektron qeydiyyat forması vasitəsilə müraciət etməsinə imkan verməlidir.

### Əsas tələblər

* Namizəd sistem üzərindən qeydiyyatdan keçə bilməlidir.
* Qeydiyyat prosesi sadə, aydın və istifadəçi üçün rahat olmalıdır.
* Qeydiyyat üçün tələb olunan məlumatlar lazımsız səhifə yönləndirmələri olmadan vahid proses daxilində toplanmalıdır.
* Uğurlu qeydiyyatdan sonra namizəd üçün profil yaradılmalıdır.
* Qeydiyyat məlumatları avtomatik olaraq backend database-ə ötürülməlidir.
* Qeydiyyat məlumatlarının göndərilməsi üçün əlavə manual təsdiq addımı tələb olunmamalıdır.

### QA qeydləri

Bu modul valid məlumatlar, invalid məlumatlar, boş required field-lər, təkrar qeydiyyat cəhdləri və fərqli altproqram seçimləri ilə test edilməlidir.

---

## 2. Təkrar qeydiyyatın qarşısının alınması

Sistem eyni namizədin eyni altproqrama bir neçə dəfə qeydiyyatdan keçməsinin qarşısını almalıdır.

### Əsas tələblər

* Hər namizəd üçün unikal profil yaradılmalıdır.
* Sistem eyni altproqrama təkrar qeydiyyata icazə verməməlidir.
* Namizəd uyğun olduğu halda bir neçə fərqli altproqrama müraciət edə bilməlidir.
* Təkrar qeydiyyat zamanı istifadəçiyə aydın xəbərdarlıq mesajı göstərilməlidir.

### QA qeydləri

Duplicate validation məntiqi dəqiqləşdirilməlidir. Təkrar qeydiyyatın hansı məlumat əsasında yoxlanıldığı aydın olmalıdır: unikal identifikator, email, telefon nömrəsi və ya bu məlumatların kombinasiyası.

---

## 3. Altproqram uyğunluğu

Sistem altproqramlar üzrə müəyyən edilmiş uyğunluq və məhdudiyyət qaydalarını tətbiq etməlidir.

### Əsas tələblər

* Bəzi altproqramlarda yaş məhdudiyyəti tətbiq olunmalıdır.
* Bəzi altproqramlarda yaş məhdudiyyəti olmaya bilər.
* Müəyyən altproqramlar arasında qarşılıqlı məhdudiyyət tətbiq oluna bilər.
* Namizəd bir altproqramda uğursuz olduqda digər uyğun altproqrama müraciət edə bilməlidir.

### QA qeydləri

Bu modul üçün boundary testing vacibdir. Minimum yaş, maksimum yaş, minimum yaşdan aşağı və maksimum yaşdan yuxarı hallar ayrıca test edilməlidir.

---

## 4. Namizəd profili

Namizədin qeydiyyat zamanı daxil etdiyi əsas məlumatlar profil ekranında görünməlidir.

### Əsas tələblər

* Namizədin əlaqə məlumatları profildə görünməlidir.
* Bacarıq və biliklərlə bağlı məlumatlar profildə görünməlidir.
* Ünvan və iş təcrübəsi məlumatları daxil edildiyi halda profildə əks olunmalıdır.
* Namizəd icazə verilən məlumatları şəxsi kabinet üzərindən yeniləyə bilməlidir.
* Yenilənən məlumatlar database-də də əks olunmalıdır.

### QA qeydləri

Profil yeniləmə funksiyası editable və non-editable field-lər üzrə yoxlanılmalıdır. Məlumatların yadda saxlanması, validation qaydaları və database update davranışı test edilməlidir.

---

## 5. Müraciətlərin izlənməsi

Namizəd bütün müraciətlərini vahid bölmə üzərindən izləyə bilməlidir.

### Əsas tələblər

* Bütün müraciətlər vahid müraciət izləmə bölməsində görünməlidir.
* Lazımsız və təkrar müraciət bölmələri sistemdən çıxarılmalıdır.
* Namizəd müraciətindən bir əməliyyatla imtina edə bilməlidir.
* İmtina əməliyyatı sistemdə avtomatik qeyd olunmalıdır.

### QA qeydləri

Müraciət statusunun dəyişməsi, imtina əməliyyatı, təsdiq mesajı və database-də statusun yenilənməsi test edilməlidir.

---

## 6. Admin və database idarəetməsi

Adminlər qeydiyyatdan keçmiş namizədlərin məlumatlarını idarə edə və qeydiyyatdan sonrakı mərhələlərdə əlavə məlumatlar daxil edə bilməlidir.

### Əsas tələblər

* Admin namizəd məlumatlarını görə bilməlidir.
* Admin qeydiyyatdan sonra əlavə məlumat daxil edə bilməlidir.
* Namizəd məlumatları üzrə axtarış və filtrasiya funksiyası olmalıdır.
* Köməkçi admin yalnız əsas admin tərəfindən icazə verilən sahələri görə və redaktə edə bilməlidir.
* Namizəd üzrə əlavə qeydlər üçün ayrıca qeyd sahəsi olmalıdır.

### QA qeydləri

Role-based access control ayrıca test edilməlidir. Əsas admin və köməkçi admin icazələri fərqli test ssenariləri ilə yoxlanılmalıdır.

---

## 7. Müsahibə və bal sistemi

Sistem müsahibə nəticələrinin daxil edilməsini və balların avtomatik hesablanmasını dəstəkləməlidir.

### Əsas tələblər

* Admin müsahibə ballarını daxil edə bilməlidir.
* Sistem ümumi və ya orta balı avtomatik hesablamalıdır.
* Bal nəticəsinə əsasən namizəd statusu avtomatik yenilənə bilməlidir.
* Lazım olduqda balı daxil edən şəxsin məlumatı görünməlidir.

### QA qeydləri

Bal hesablanması minimum, maksimum, valid, invalid və sərhəd dəyərləri ilə test edilməlidir.

---

## 8. Namizəd statuslarının idarə edilməsi

Sistem namizədin qeydiyyatdan sonrakı mərhələlərdə müxtəlif statuslarla izlənməsini təmin etməlidir.

### Əsas status nümunələri

* Müsahibə üçün gözləyir
* Əlaqə saxlanıla bilmədi
* Yenidən əlaqə
* Müsahibədə iştirak etmədi
* Ehtiyat namizəd
* Keçmədi
* İmtina etdi
* Donduruldu
* Cari könüllü
* Məzun könüllü

### QA qeydləri

Hər statusun seçilməsi, yadda saxlanması, ekranda görünməsi, filtrasiya olunması və bildiriş davranışı ayrıca test edilməlidir.

---

## 9. Bildiriş qaydaları

Sistem uyğun hallarda namizədlərə bildiriş göndərilməsini dəstəkləməlidir.

### Əsas tələblər

* Admin müsahibə ilə bağlı bildiriş göndərə bilməlidir.
* Bildiriş email və ya telefon nömrəsi vasitəsilə göndərilə bilər.
* Bəzi yekun statuslar üçün əvvəlcədən müəyyən edilmiş email bildirişləri ola bilər.
* Mail göndərilmə vəziyyəti sistemdə izlənməlidir.

### QA qeydləri

Email göndərilməsi, uğursuz göndərilmə halları, yanlış email statusu və statusa əsaslanan bildiriş qaydaları test edilməlidir.

---

## 10. Sənəd və CV yükləmə qaydaları

Sistem altproqram qaydalarına uyğun sənəd və CV yükləmə funksiyasını dəstəkləməlidir.

### Əsas tələblər

* Lazım olan hallarda sənəd yükləmə bölməsi mövcud olmalıdır.
* Bəzi altproqramlarda CV yükləmə məcburi ola bilər.
* Bəzi altproqramlarda sənəd yükləmə optional ola bilər.
* Sənəd yüklənmədikdə sistem qaydalara uyğun davranmalıdır.

### QA qeydləri

Mandatory və optional upload qaydaları ayrıca test edilməlidir. Fayl formatı, fayl ölçüsü, boş upload və invalid fayl yükləmə davranışı dəqiqləşdirilməli və test edilməlidir.
