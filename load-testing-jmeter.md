## Load Testing (JMeter)

Lalafo Elektronika kataqoriyasının load testi Apache JMeter vasitəsilə aparıldı.

### Test konfiqurasiyası
- Ramp-up period: 5 saniyə
- Loop count: 2

---

### Test 1 – 50 users
- Average response time: 953 ms
- Maximum: 1514 ms
- Error rate: 0%
- Throughput: 14.3 request/sec

---

### Test 2 – 100 users
- Average response time: 2987 ms
- Maximum: 4529 ms
- Error rate: 0%
- Throughput: 27.5 request/sec

---

### Test 3 – 200 users
- Average response time: 2851 ms
- Maximum: 7241 ms
- Error rate: 0%
- Throughput: 3.2 request/sec

---

### Analiz

50 istifadəçi yükündə sistem sürətli və stabil işləyir.  

100 istifadəçi zamanı sistem hələ stabil qalır, lakin response time əhəmiyyətli dərəcədə artır.  

200 istifadəçi zamanı isə sistemdə qeyri-sabit performans müşahidə olunur. Bəzi sorğular tez cavab versə də, maksimum gecikmə 7 saniyəyə qədər yüksəlir və throughput ciddi şəkildə azalır.  

---

### Yekun

Sistem aşağı yükdə yaxşı performans göstərir, lakin istifadəçi sayı artdıqca gecikmələr və performans problemləri ortaya çıxır. Yüksək yük altında sistemin optimallaşdırılması tələb olunur.
