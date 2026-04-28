## Load Testing (JMeter)

Lalafo.az saytının elektronika kateqoriyası Apache JMeter vasitəsilə yük altında test edildi.

### Test scope
Elektronika kateqoriyasının səhifələri müxtəlif istifadəçi yükü altında yoxlanıldı.

### Test konfiqurasiyası
- Threads (users): 50 / 100 / 200
- Ramp-up period: 5 saniyə
- Loop count: 2
- Alət: Apache JMeter

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

- 50 istifadəçi: Sistem sürətli və stabil işləyir  
- 100 istifadəçi: Sistem stabil qalır, lakin cavab müddəti artır  
- 200 istifadəçi: Gecikmələr artır, performans qeyri-sabit olur və throughput azalır  

---

### Yekun

Sistem aşağı yükdə yaxşı performans göstərir, lakin istifadəçi sayı artdıqca gecikmələr və performans problemləri müşahidə olunur. Yüksək yük altında sistemin optimallaşdırılması tələb olunur.


### 50 users
![50 users](screenshots/50-users.png)

### 100 users
![100 users](screenshots/100-users.png)

### 200 users
![200 users](screenshots/200-users.png)
