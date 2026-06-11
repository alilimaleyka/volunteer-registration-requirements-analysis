# Test Scenarios

## TS-001: Namizədin qeydiyyatdan keçməsi

**Module:** Registration
**Description:** Namizəd könüllü qeydiyyat sistemi üzərindən müraciət edə bilməlidir.

**Test Scope:**

* Qeydiyyat formasının açılması
* Required field-lərin yoxlanılması
* Valid məlumatlarla qeydiyyat
* Invalid məlumatlarla qeydiyyat
* Qeydiyyat məlumatlarının sistemə ötürülməsi

---

## TS-002: Təkrar qeydiyyatın qarşısının alınması

**Module:** Duplicate Registration Prevention
**Description:** Eyni namizəd eyni altproqrama təkrar qeydiyyatdan keçə bilməməlidir.

**Test Scope:**

* Eyni unikal məlumatlarla təkrar qeydiyyat cəhdi
* Eyni altproqrama ikinci dəfə müraciət
* Fərqli altproqrama uyğunluq əsasında müraciət
* Təkrar qeydiyyat zamanı xəbərdarlıq mesajının göstərilməsi

---

## TS-003: Altproqram seçimi və uyğunluq qaydaları

**Module:** Subprogram Eligibility
**Description:** Sistem namizədin yaşına və uyğunluq qaydalarına əsasən altproqramlara müraciəti idarə etməlidir.

**Test Scope:**

* Yaş məhdudiyyəti olan altproqramlar
* Yaş məhdudiyyəti olmayan altproqramlar
* Minimum yaş sərhədi
* Maksimum yaş sərhədi
* Uyğun olmayan yaşla müraciət
* Uyğun olan namizədin bir neçə altproqrama müraciəti

---

## TS-004: Altproqramlararası məhdudiyyətlərin yoxlanılması

**Module:** Cross-Program Restriction
**Description:** Müəyyən altproqramlar arasında qarşılıqlı məhdudiyyət qaydaları tətbiq olunmalıdır.

**Test Scope:**

* Bir altproqramda könüllü olmuş namizədin məhdudlaşdırılmış digər altproqrama müraciəti
* Uğursuz namizədin digər altproqrama müraciət imkanı
* Sistem mesajlarının düzgün göstərilməsi
* Müraciət statusunun düzgün saxlanılması

---

## TS-005: Namizəd profil məlumatlarının göstərilməsi

**Module:** Candidate Profile
**Description:** Namizədin qeydiyyat zamanı daxil etdiyi əsas məlumatlar profil ekranında görünməlidir.

**Test Scope:**

* Əlaqə məlumatlarının görünməsi
* Ünvan məlumatlarının görünməsi
* Bacarıq və bilik məlumatlarının görünməsi
* İş təcrübəsi məlumatlarının görünməsi
* Şəxsi kabinetdə məlumatların yenilənməsi
* Yenilənmiş məlumatların sistemdə saxlanılması

---

## TS-006: Müraciətlərin izlənməsi

**Module:** Application Tracking
**Description:** Namizəd bütün müraciətlərini vahid bölmə üzərindən izləyə bilməlidir.

**Test Scope:**

* Bütün müraciətlərin siyahıda görünməsi
* Müraciət statuslarının göstərilməsi
* Müraciətdən imtina funksiyası
* İmtina statusunun sistemdə saxlanılması
* Lazımsız müraciət bölmələrinin görünməməsi

---

## TS-007: Admin paneldə namizəd məlumatlarının idarə edilməsi

**Module:** Admin / Database Management
**Description:** Admin namizəd məlumatlarını görə, redaktə edə və qeydiyyatdan sonrakı məlumatları əlavə edə bilməlidir.

**Test Scope:**

* Adminin namizəd siyahısını görməsi
* Namizəd məlumatlarının axtarışı
* Namizəd məlumatlarının filtrasiya edilməsi
* Əlavə məlumatların daxil edilməsi
* Qeyd sahəsinin istifadəsi
* Dəyişikliklərin sistemdə saxlanılması

---

## TS-008: Köməkçi admin icazələrinin yoxlanılması

**Module:** Role-Based Access Control
**Description:** Köməkçi admin yalnız icazə verilən sahələri görə və redaktə edə bilməlidir.

**Test Scope:**

* Köməkçi adminin görə bildiyi sahələr
* Köməkçi adminin redaktə edə bildiyi sahələr
* İcazəsiz sahələrə girişin məhdudlaşdırılması
* Əsas admin və köməkçi admin fərqlərinin yoxlanılması

---

## TS-009: Müsahibə ballarının daxil edilməsi və hesablanması

**Module:** Interview Scoring
**Description:** Admin müsahibə ballarını daxil etdikdə sistem ümumi və ya orta balı avtomatik hesablamalıdır.

**Test Scope:**

* Valid bal daxil edilməsi
* Minimum bal dəyərləri
* Maksimum bal dəyərləri
* Invalid bal daxil edilməsi
* Ümumi/orta balın avtomatik hesablanması
* Balı daxil edən şəxsin məlumatının görünməsi

---

## TS-010: Namizəd statuslarının idarə edilməsi

**Module:** Candidate Status Management
**Description:** Namizədin müraciət və müsahibə nəticəsinə əsasən statusu sistemdə idarə olunmalıdır.

**Test Scope:**

* Statusun manual seçilməsi
* Statusun avtomatik dəyişməsi
* Statusun yadda saxlanılması
* Status üzrə filtrasiya
* Status dəyişdikdə bildiriş davranışı

---

## TS-011: Email və SMS bildirişlərinin yoxlanılması

**Module:** Notifications
**Description:** Sistem uyğun hallarda namizədə email və ya SMS bildirişi göndərə bilməlidir.

**Test Scope:**

* Müsahibə bildirişinin göndərilməsi
* Yekun nəticə bildirişinin göndərilməsi
* Yanlış email halının idarə edilməsi
* Mail vəziyyətinin dəyişməsi
* Bildirişin uyğun statusa əsasən göndərilməsi

---

## TS-012: Sənəd və CV yükləmə qaydalarının yoxlanılması

**Module:** Document Upload
**Description:** Sistem altproqram qaydalarına əsasən sənəd və CV yükləmə tələblərini tətbiq etməlidir.

**Test Scope:**

* Məcburi CV yükləmə
* Optional sənəd yükləmə
* Sənəd yükləmədən qeydiyyat cəhdi
* Yanlış fayl formatı
* Böyük həcmli fayl
* Uğurlu fayl yükləmə

