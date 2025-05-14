# Satış Məlumatları Analizi

Bu layihə satış məlumatlarını analiz edərək və vizuallaşdıraraq biznes qərarları üçün faydalı insaytlar əldə etməyə imkan verir. Mən bu kodu endirim effektivliyi, müştəri davranışı və satış tendensiyalarını başa düşmək üçün yaratdım.

## Bu layihə nə edir?

- Satış məlumatlarını oxuyur və təhlil edir
- Endirimlərin satışlara təsirini ölçür
- Həftənin və günün hansı vaxtlarında satışların daha yaxşı getdiyini göstərir
- Ən çox gəlir gətirən məhsul kateqoriyalarını müəyyənləşdirir
- VIP müştərilərin satışlardakı rolunu araşdırır
- Məhsul qaytarılmasının əsas səbəblərini aşkar edir
- Bütün bu analizləri gözəl qrafiklər və diaqramlarla göstərir

## Necə istifadə edə bilərəm?

1. Bu reponu öz kompüterinizə yükləyin
2. `satislar_data.csv` faylını `data` qovluğuna yerləşdirin (və ya öz CSV faylınızı eyni sütun adları ilə istifadə edin)
3. Python mühitinizdə lazımi paketləri yükləyin:
   ```
   pip install pandas numpy matplotlib seaborn
   ```
4. Analiz skriptini çalışdırın:
   ```
   python analyze_sales.py
   ```
   
Budur! İndi siz `results` qovluğunda bütün analiz hesabatlarını və qrafikləri görəcəksiniz.

## CSV faylımın necə görünməlidir?

CSV faylınızda bu sütunlar olmalıdır:
```
sale_id, date, customer_id, customer_name, customer_city, store_id, store_name, 
store_city, product_id, product_name, product_category, quantity, base_price, 
discount_pct, final_price, total_amount, payment_method, promotion_code, 
is_vip_customer, weekday, month, year, hour, is_returned, return_date, return_reason
```

## Əldə etdiyim nəticələr nə olacaq?

Bu layihə ilə siz aşağıdakı suallara cavab tapa biləcəksiniz:

- Hansı endirim səviyyəsi ən çox satış gətirir? (15% endirimlər daha effektivdir?)
- Həftənin hansı günü və günün hansı saatlarında satışlar pik səviyyəyə çatır?
- Hansı məhsul kateqoriyaları ən çox satılır və gəlir gətirir?
- VIP müştərilər biznes üçün nə qədər dəyərlidir?
- Müştərilər niyə məhsulları qaytarırlar və bunu necə azalda bilərik?

## Çıxış qrafiklərinə nümunələr

- Endirim səviyyələrinin satışlara təsiri
- Həftəlik və saatlıq satış tendensiyaları
- Məhsul kateqoriyalarının payı
- Ödəniş metodlarının populyarlığı
- Məhsul qiyməti və satış miqdarı arasındakı əlaqə

## Layihə üzərində necə işlədim

Mən Python dilində pandas, numpy, matplotlib və seaborn kitabxanalarından istifadə edərək bu proyekti hazırladım. İlk öncə satış məlumatlarını analiz etdim, sonra bu məlumatları vizual olaraq təqdim etmək üçün müxtəlif qrafik növlərindən istifadə etdim.

Başlanğıcda iki əsas problem ilə qarşılaşdım: qrafiklərin üst-üstə düşməsi və annotasiyaların (işarələmələrin) qarışması. Bu problemləri yaradıcı şəkildə həll etdim və nəticədə təmiz və anlaşılan vizuallaşdırmalar əldə etdim.

## Əlavə işlər

Bu layihəni genişləndirmək üçün aşağıdakı istiqamətlərdə işlər görməyi planlaşdırıram:

- Interaktiv vizuallaşdırmalar üçün Plotly və Dash əlavə etmək
- Satış proqnozları üçün sadə ML modeli qurmaq
- Həftəlik avtomatik hesabat göndərmək üçün script yazmaq

Əgər bu layihə xoşunuza gəlirsə və ya suallarınız varsa, əlaqə saxlamaqdan çəkinməyin!

## Lisenziya

Bu layihə MIT lisenziyası altında yayımlanır.
