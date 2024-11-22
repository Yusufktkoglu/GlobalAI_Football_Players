# GlobalAI_Football_Players
![image](https://raw.githubusercontent.com/Yusufktkoglu/GlobalAI_Football_Players/main/cr7.jpg)

Futbol oyuncuları birçok oyuncunun uzunluğu kilosu yaşı bitiriciliği gibi 50'ye yakın özelliği içeren bir veri setidir. Veri setinin linkini aşağıdan bulabilirsiniz.

*Football Players Data: https://www.kaggle.com/datasets/maso0dahmed/football-players-data

*Projenin Kaggle Linki: https://www.kaggle.com/code/yusufktkolu/globalai-fifa-players

#### Değişkenler

* **name:** Oyuncunun adı.  
* **full_name:** Oyuncunun tam adı.  
* **birth_date:** Oyuncunun doğum tarihi.  
* **age:** Oyuncunun yaşı.  
* **height_cm:** Oyuncunun boyu (santimetre cinsinden).  
* **weight_kgs:** Oyuncunun ağırlığı (kilogram cinsinden).  
* **positions:** Oyuncunun oynadığı pozisyonlar.  
* **nationality:** Oyuncunun milliyeti.  
* **overall_rating:** Oyuncunun genel değerlendirme puanı.  
* **potential:** Oyuncunun ulaşabileceği maksimum potansiyel puanı.  
* **value_euro:** Oyuncunun piyasa değeri (Euro cinsinden).  
* **wage_euro:** Oyuncunun haftalık maaşı (Euro cinsinden).  
* **preferred_foot:** Oyuncunun tercih ettiği ayak (sağ/sol).  
* **international_reputation(1-5):** Oyuncunun uluslararası itibarı (1-5 arası).  
* **weak_foot(1-5):** Oyuncunun zayıf ayağının değerlendirmesi (1-5 arası).  
* **skill_moves(1-5):** Oyuncunun yetenek hareketleri değerlendirmesi (1-5 arası).   
* **release_clause_euro:** Oyuncunun serbest kalma bedeli (Euro cinsinden).  
* **national_team:** Oyuncunun milli takımda oynayıp oynamadığı.  
* **national_rating:** Oyuncunun milli takım performans puanı.  
* **national_team_position:** Oyuncunun milli takım pozisyonu.  
* **national_jersey_number:** Oyuncunun milli takım forma numarası.  
* **crossing:** Oyuncunun orta yapma becerisi.  
* **finishing:** Oyuncunun bitiricilik becerisi.  
* **heading_accuracy:** Oyuncunun kafa vuruşu isabetliliği.  
* **short_passing:** Oyuncunun kısa pas becerisi.  
* **volleys:** Oyuncunun vole vurma becerisi.  
* **dribbling:** Oyuncunun çalım atma becerisi.  
* **curve:** Oyuncunun falso verme becerisi.  
* **freekick_accuracy:** Oyuncunun frikik isabetliliği.  
* **long_passing:** Oyuncunun uzun pas becerisi.  
* **ball_control:** Oyuncunun top kontrol becerisi.  
* **acceleration:** Oyuncunun hızlanma becerisi.  
* **sprint_speed:** Oyuncunun sprint hızı.  
* **agility:** Oyuncunun çevikliği.  
* **reactions:** Oyuncunun reaksiyon süresi.  
* **balance:** Oyuncunun dengesini koruma becerisi.  
* **shot_power:** Oyuncunun şut gücü.  
* **jumping:** Oyuncunun sıçrama kabiliyeti.  
* **stamina:** Oyuncunun dayanıklılığı.  
* **strength:** Oyuncunun fiziksel gücü.  
* **long_shots:** Oyuncunun uzaktan şut çekme becerisi.  
* **aggression:** Oyuncunun agresifliği.  
* **interceptions:** Oyuncunun pas kesme becerisi.  
* **positioning:** Oyuncunun saha içi pozisyon alma becerisi.  
* **vision:** Oyuncunun oyun görüşü.  
* **penalties:** Oyuncunun penaltı atışı becerisi.  
* **composure:** Oyuncunun baskı altındaki soğukkanlılığı.  
* **marking:** Oyuncunun adam markajı becerisi.  
* **standing_tackle:** Oyuncunun ayakta müdahale becerisi.  
* **sliding_tackle:** Oyuncunun kayarak müdahale becerisi.

## Varılan Sonuçlar.

* Verimizde kendi eklediğimiz kayıp verilerin yanı sıra oyuncuların milli takım özelliklerinde eksiklikler vardı bunun sebebi daha önce o oyuncuların milli takımda oynamamış olması.
*  Verimiz 51 sütundan ve 2032 satıdan oluşuyor.
*  Verimizin çoğu numerik değişken olmak üzere pozisyon gibi bazı değerler kategorik hale getirilmiştir.
*  Verimizden forma numarası gibi analizimiz için gereksiz olabilecek sütunları veri setimizden sildik.
*  Veri setimizde en çok stoper ardından santrafor ve orta saha geliyor.
*  Pozisyonlar arasında ortalama en çok değere sahip olan pozisyon Merkez Forver ardından sağ ve sol kanat geliyor.
*  Reytingi en yüksek oyuncular sırasıyla Ronaldo(94), Messi(94) ve Neymar(92) olarak devam ediyor.
*  Korelasyon analizinde çok fazla özelliğimiz olduğu için özelliklerimizi defansif, orta saha, hücumcu ve fiziksel özellikler olarak 4'e ayırdık.
*  Defansif özelliklerde olan korelasyon ısı haritasında marking'in standin_tackle,siliding_tackle ve interceptions ile güçlü pozitif ilişkisi olduğu ve agression ile pozitif ilişkisi olduğunu görüyoruz aslında bu dört özellik kendi aralarında güçlü pozitif ilişkiye sahip olduğunu, kilo ve güç arasında'da pozitif bir ilişki olduğunu gördük.
*  Orta saha özelliklerinde ise buradada yine kendi aralarında güçlü ilişkiler olan özellikler gördük. Short_passing, dribbling ve ball_control kendi aralarında güçlü pozitif ilişki olduğunu görebiliriz. Aynı zamanda bu üç özelliğin vision, composure ve agility arasındada pozitif bir ilişki var. Skill_moves özelliğinin ise dribbling ile arasında güçlü bir ilişki varken ball_control, vşsşon, agility gibi özelliklerlede arasında pozitif ilişki var.
*  Hücumcu özelliklerinde ise finishing özelliğinin positioning, volleys ve dribbling arasında arasında güçlü, shot_power, penalties ve skill_moves ile ise pozitif ilişkide olduğunu görebiliriz. Yine bu özellikler kendi aralarında pozitif ilişkiye sahip.
*  Fiziksel özelliklerin reytinge ve potansiyele herhangi bir etkisi olmadığını gördük.
*  Yaş ve potansiyel arasındaki ilişkide ise yaş ilerledikçe reytingin arttığını fakat doğal olarak potansiyelin genellikle genç yaşlarda yüksek seviyede olduğunu gördük.
*  Dikkat çekici potansiyeli yüksek olan 21 yaş altında olan oyuncular arasında ise sırasıyla Mbappe(95), Donnaruma(94) ve de Ligt(92) olduğunu gördük.


* **ÖNERİ**: Buradan sonra istenirse potansiyel ve overall reytinge göre oyuncular S+, S, A+, A gibi bir segmentasyon yapılabilir. Makine öğrenmesi kullanarak en az maaliyetli ve en verimli oyuncular bulunabilir ve optimal en iyi 11 kurulabilir.
