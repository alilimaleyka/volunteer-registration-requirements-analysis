# Volunteer Registration System Testing Checklist

## Registration

- [ ] Qeydiyyat forması açılır
- [ ] Required field-lər yoxlanılır
- [ ] Valid məlumatlarla qeydiyyat tamamlanır
- [ ] Invalid məlumatlarla validation mesajı göstərilir
- [ ] Qeydiyyat məlumatları sistemdə saxlanılır

## Duplicate Registration

- [ ] Eyni namizəd eyni altproqrama təkrar qeydiyyatdan keçə bilmir
- [ ] Təkrar qeydiyyat zamanı xəbərdarlıq mesajı göstərilir
- [ ] Namizəd uyğun olduğu halda fərqli altproqrama müraciət edə bilir

## Eligibility Rules

- [ ] Yaş məhdudiyyəti olan altproqramlar yoxlanılır
- [ ] Minimum yaş sərhədi yoxlanılır
- [ ] Maksimum yaş sərhədi yoxlanılır
- [ ] Uyğun olmayan yaşda qeydiyyat bloklanır

## Candidate Profile

- [ ] Namizəd profili yaradılır
- [ ] Əlaqə məlumatları profildə görünür
- [ ] Profil məlumatları yenilənə bilir
- [ ] Yenilənmiş məlumatlar sistemdə saxlanılır

## Admin Panel

- [ ] Admin namizəd məlumatlarını görə bilir
- [ ] Admin namizəd məlumatlarını axtara bilir
- [ ] Admin filter funksiyasından istifadə edə bilir
- [ ] Köməkçi admin yalnız icazəli sahələri görə bilir

## Notifications

- [ ] Email bildirişi göndərilir
- [ ] Yanlış email halı düzgün idarə olunur
- [ ] Mail statusu sistemdə yenilənir

## Document Upload

- [ ] Məcburi CV yükləmə yoxlanılır
- [ ] Optional sənəd yükləmə yoxlanılır
- [ ] Yanlış fayl formatı bloklanır
- [ ] Böyük həcmli fayl yükləmə yoxlanılır