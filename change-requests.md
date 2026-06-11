# Change Requests / Improvement Notes

## CR-001: Qeydiyyat başlığının daha aydın adlandırılması

**Module:** Registration Page
**Type:** Content Improvement
**Priority:** Medium

**Current Behavior:**
Qeydiyyat bölməsində istifadə olunan başlıq istifadəçi üçün tam aydın olmaya bilər.

**Requested Change:**
Qeydiyyata açıq olan altproqramlar hissəsinin adı daha qısa və aydın formada təqdim edilməlidir.

**Expected Benefit:**
İstifadəçi hansı altproqramların qeydiyyata açıq olduğunu daha rahat başa düşəcək.

---

## CR-002: Əlavə altproqram seçimlərinin qeydiyyata əlavə edilməsi

**Module:** Subprogram Selection
**Type:** Functional Improvement
**Priority:** High

**Current Behavior:**
Qeydiyyat zamanı bütün tələb olunan altproqram seçimləri görünməyə bilər.

**Requested Change:**
Qeydiyyata açıq olan bütün uyğun altproqramlar seçim siyahısına əlavə edilməlidir.

**Expected Benefit:**
Namizəd uyğun olduğu altproqramı sistem üzərindən birbaşa seçə biləcək.

---

## CR-003: Təkrar qeydiyyatın avtomatik bloklanması

**Module:** Duplicate Registration Prevention
**Type:** Business Rule
**Priority:** High

**Current Behavior:**
Eyni namizədin eyni altproqrama təkrar qeydiyyat etməsinin qarşısı sistem tərəfindən avtomatik alınmaya bilər.

**Requested Change:**
Sistem eyni namizədin eyni altproqrama təkrar müraciət etməsini avtomatik bloklamalıdır.

**Expected Benefit:**
Database-də təkrar məlumatların yaranmasının qarşısı alınacaq və müraciətlərin idarə edilməsi daha səliqəli olacaq.

---

## CR-004: Qeydiyyat məlumatlarının vahid səhifədə toplanması

**Module:** Registration Flow
**Type:** UX Improvement
**Priority:** Medium

**Current Behavior:**
Qeydiyyat zamanı istifadəçinin müxtəlif səhifələrə yönləndirilməsi çaşqınlıq yarada bilər.

**Requested Change:**
Qeydiyyat üçün tələb olunan məlumatlar vahid proses daxilində, mərhələli və ya bloklar üzrə təqdim edilməlidir.

**Expected Benefit:**
İstifadəçi qeydiyyatı daha rahat və fasiləsiz şəkildə tamamlayacaq.

---

## CR-005: “İcrada olan müraciətlər” bölməsinin ləğv edilməsi

**Module:** Application Tracking
**Type:** Navigation Improvement
**Priority:** Medium

**Current Behavior:**
Müraciətlərin ayrı-ayrı bölmələrdə göstərilməsi istifadəçi üçün qarışıqlıq yarada bilər.

**Requested Change:**
Bütün müraciətlər vahid “Bütün müraciətlər” bölməsi üzərindən izlənməlidir.

**Expected Benefit:**
Namizəd bütün müraciətlərini bir yerdə görə və izləyə biləcək.

---

## CR-006: Müraciətdən bir kliklə imtina funksiyasının əlavə edilməsi

**Module:** Application Tracking
**Type:** Functional Improvement
**Priority:** High

**Current Behavior:**
Namizədin müraciətdən imtina prosesi sadə və birbaşa olmaya bilər.

**Requested Change:**
Namizədə müraciətindən bir kliklə imtina etmək imkanı verilməlidir.

**Expected Benefit:**
İmtina prosesi daha sürətli olacaq və sistemdə avtomatik qeydə alınacaq.

---

## CR-007: Müsahibə linki üçün ayrıca sahənin əlavə edilməsi

**Module:** Interview Management
**Type:** Functional Improvement
**Priority:** Medium

**Current Behavior:**
Onlayn müsahibə linkinin yerləşdirilməsi üçün ayrıca strukturlaşdırılmış sahə olmaya bilər.

**Requested Change:**
Admin paneldə onlayn müsahibə linki üçün ayrıca sahə əlavə edilməlidir.

**Expected Benefit:**
Namizədə onlayn müsahibə məlumatı daha düzgün və sistemli şəkildə təqdim ediləcək.

---

## CR-008: “Yenidən əlaqə” funksiyasının əlavə edilməsi

**Module:** Candidate Status Management
**Type:** Functional Improvement
**Priority:** Medium

**Current Behavior:**
Əlaqə saxlanıla bilməyən və ya müsahibədə iştirak etməyən namizədlərlə yenidən əlaqə prosesi ayrıca izlənməyə bilər.

**Requested Change:**
Müvafiq statuslarda namizədə sistem üzərindən yenidən əlaqə müraciəti göndərmək imkanı yaradılmalıdır.

**Expected Benefit:**
Namizədin statusu və yenidən əlaqə prosesi daha rahat izlənəcək.

---

## CR-009: CV yükləmə qaydasının altproqramlara görə tətbiqi

**Module:** Document Upload
**Type:** Validation Rule
**Priority:** High

**Current Behavior:**
CV və sənəd yükləmə tələbləri bütün altproqramlar üçün eyni tətbiq oluna bilər.

**Requested Change:**
CV yükləmə bəzi altproqramlar üçün məcburi, bəziləri üçün optional olmalıdır.

**Expected Benefit:**
Qeydiyyat prosesi altproqram tələblərinə uyğun işləyəcək.

---

## CR-010: Köməkçi admin icazələrinin məhdudlaşdırılması

**Module:** Role-Based Access Control
**Type:** Security / Permission Requirement
**Priority:** High

**Current Behavior:**
Köməkçi adminlərin bütün məlumatları görməsi və redaktə etməsi təhlükəsizlik və idarəetmə baxımından uyğun olmaya bilər.

**Requested Change:**
Köməkçi adminlər yalnız əsas admin tərəfindən icazə verilən sahələri görə və redaktə edə bilməlidir.

**Expected Benefit:**
Məlumatların təhlükəsizliyi və rol əsaslı idarəetmə təmin ediləcək.
