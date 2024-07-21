Ten projekt jest podsumowaniem etapu mojej nauki HTML oraz CSS - jest to kopia layoutu strony Onet.pl w czterech widokach: na komputery stacjonarne, tablety w wariancie horyzontalnym i wertykalnym oraz mobilnym. 

![desktop](https://github.com/user-attachments/assets/dac6da48-70bc-406f-a36b-03df0a093782)

![tablet horizontal](https://github.com/user-attachments/assets/441af189-86c3-47f0-8c10-63725f2df7bc)

![tablet vertical](https://github.com/user-attachments/assets/ce12a4ab-9b65-4fd1-aeb9-642695e1b30d)

![mobile](https://github.com/user-attachments/assets/1b826f32-2fb3-4ebd-9e62-f8295e628077)


By jak najlepiej oddać ducha zawodowych warunków, sama nałożyłam sobie deadline oraz sama wyznaczyłam sobie cele do osiągnięcia. Były one następujące:

1) statyczna strona-kopia strony Onetu - do kilku pierwszych sekcji;
2) RWD - wersje na desktopy, tablety oraz telefony;
3) rozwijane menu w kilku miejscach.

Opcjonalne:
1) co najmniej jeden osadzony film wideo;
2) widżet pokazujący aktualną pogodę;
3) jedna transformacja - pasek menu ma przyklejać się do góry strony podczas przewijania.

Aby oswoić się z githubem oraz - znowu - działać trochę tak, jak bym działała w pracy zawodowej, wrzucałam kolejne fragmenty kodu na githuba, a znajomy Frontend Developer (pracujący na stanowisku seniora) robił mi code review. 

Co się udało? 
Udało się skończyć projekt w wyznaczonym terminie, choć ostatni miesiąc "crunchowałam". Zrobiłam osobne wersje na desktopy, tablety (w orientacji pionowej i poziomej) oraz na telefony. Zrobiłam również rozwijane menu w kilku miejsach. Umieściłam filmik wideo (z prywatnych zbiorów), bo choć planowałam osadzić jakiś filmik z yt, to jednak prawa autorskie oraz przeszkody techniczne mi na to nie pozwoliły. Pasek menu elegancko przykleja się do góry strony podczas scrollowania. W wersji mobilnej jest kilka menu przewijanych w poziomie (jak w mobilnej wersji onetu). 

Nie udało mi się dodać widżeta pogodowego - zamiast niego jest statyczny obrazek wraz z ikonkami i tekstem. 

Czego mnie nauczył ten projekt?
1) estymowania czasu, a właściwie tego, że ciężko jest ten czas na wykonanie jakiejś części projektu wyestymować. Małe rzeczy, które wedle mojej opinii powinny mi zająć kilkanaście minut, niejednokrotnie zajmowały mi pół nocy, bo np. gdzieś się wkradła literówka albo nowa funkcjonalność działała, ale jednocześnie psuła wcześniej zrobione rzeczy. Więc samo napisanie kodu zajmowało faktycznie kilka minut, ale reperowanie skutków to już była kwestia znacznie większego nakładu czasu;
2) RWD to potężne i skomplikowane zagadnienie;
3) dobrze napisany HTML jest najlepszym fundamentem do dalszej pracy nad stroną. Odpowiednie nazewnictwo klas (jakaś z góry przyjęta zasada tworzenia nazw klas bardzo pomaga), odpowiednia struktrura dokumentu - to wszystko jest niezwykle ważne zwłaszcza w kontekście RWD;
4) że mam w swoich zbiorach absurdalnie dużo zdjęć moich kotów;
5) dowiedziałam się, jaki mam styl pracy i jak podchodzę do zadań.  

Co bym *teraz* zrobiła lepiej?
1) zupełnie inaczej podeszłabym do samej struktury pliku - kod nie byłby w jednym pliku html, ale raczej podzieliłabym go w ten sposób:
- osobny kod HTML dla wersji mobilnej, gdzie elementy często były w innej kolejności niż w innych szerokościach ekranu (przy jednym htmlu często musiałam uciekać się do takich sposobów jak "ukrywanie" kodu dla poszczególnych szerokości - np. przewijane w poziomie menu miało klasę, która była ukryta w szerokościach innych niż mobilna);
- arkusz stylów byłby osobnym plikiem, a właściwie - osobnymi plikami. Dla każdej części strony (menu główne, menu kolejne, sekcja pierwsza, belka poczna etc.) stworzyłabym osobny plik .css i tam napisałabym kod, który jest wspólny dla wszystkich urządzeń, a później dodałabym media query, by wycyzelować wersje na kolejne szerokości - wtedy zmiana jakiegoś elementu w tym samym menu dla każdej szerokości byłaby dużo prostsza niż praca w jednym  kodzie wrzuconym w <style> w pliku .html. Dzięki temu właściwości jakiegoś elementu, które są wspólne dla wszystkich urządzeń, byłyby w jednym miejscu, napisane tylko raz (a nie 50 razy, jak mi wytknął mój znajomy frontendowiec).
2) zaprzyjaźniłabym się z css variables lub preprocesorem Sass, by zoptymalizować pracę i nie pisać w kilkudziesięciu miejscach tego samego koloru w RGB/HSL lub tego samego rozmiaru fontu.  
3) nie porywałabym się na RWD ;) tak zupełnie serio - gdybym miała przygotować wersję tylko na desktopy, spokojnie wyrobiłabym się bez crunchowania. Jednocześnie to właśnie praca nad RWD przyniosła mi najwięcej satysfkacji i frajdy (choć to już było raczej pod koniec ;)) oraz to dzięki pracy nad wersjami mobilną oraz tabletową nauczyłam się chyba najwięcej. 
