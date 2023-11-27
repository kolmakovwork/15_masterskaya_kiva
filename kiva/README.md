# 15_masterskaya_kiva
 EDA краудфандинговой платформы kiva.org
 
Девиз Kiva: "loans that change lives" (кредиты, которые меняют жизнь)

**Контекст проекта**

Краудфандинговая платформа kiva.org ставит своей целью предоставление финансовых услуг наиболее нуждающимся и необеспеченным людям. Заёмщики оставляют заявку на сайте, доноры поддерживают её  финансово, на месте партнёр организации выдаёт кредит, который погашается из этих средств, которые донорам возвращаются уже заёмщиками через платформу.

Kiva основана в 2005 году в Сан-Франциско.

Представленный компанией датасет за 2014-2017гг. содержит информацию о займах на различные проекты в 85 разных странах.

**Цели исследования**

1. Выявить от каких показателей зависит скоростью набора средств на заявку (разница между временем, когда заявка опублирована на сайте и средства на неё собраны), мы исследуем, связана ли доля заёмщиков-женщин с основной религией страны.
2. Проанализировать активность Kiva и заявителей в разрезе стран, дать рекомендации о тех странах, на которые Kiva стоит обратить внимание.
3. Доп.: провести дополнительные исследования (проанализировать пол заемщиков, партнеров Kiva, их объем или другие пар-ры)

**Описание данных**
Датасет kiva.csv с исполненными заявками за 2014-2017гг.

- id —  идентификатор заявки-кредита;
- funded_amount - сумма сбора (выдается агенту, USD);
- loan_amount - сумма запрашиваемого займа (от агента заемщику, USD) (loan_amount=funded_amount)
- activity - подсектор применения
- sector - сектор применения
- use - назначение-описание использования
- country_code - ISO-код страны страны, в которой выдан кредит
- country - название страны, в которой выдан кредит
- region - регион в стране
- currency - местная валюта (не интересует)
- partner_id - номер партнера, выдающий кредит
- posted_time - время публикации заявки на сайте
- disbursed_time - время предоставления кредита
- funded_time - время когда собрали денежные средства (может быть раньше даты заявки)
- term_in_months - срок в месяцах, на который был выдан кредит
- lender_count -кол-во кредиторов
- tags - тэги по сайту
- borrower_genders - пол заемщика(ов)
- repayment_interval - регулярность выплат:
    * bullet - единовременное погашение
    * weekly - еженедельно
    * monthly -ежемесячно
    * irregular - нерегулярно
- date - дата (в формате гггг-мм-дд) (предположительно = posted_time)
- main_country_religion - главная религия страны:
    * Christians - христиане
    * Muslims - мусульмане
    * Buddhists - буддисты
    * Hindus - индусы
    * Folk Religions - народные религии
    * Jews - евреи
    * Unaffiliated -неаффилированные


 