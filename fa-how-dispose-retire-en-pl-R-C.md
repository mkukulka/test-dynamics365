---
title: Sprzedaż lub likwidacja ŚT | Opis programu Microsoft docs: W przypadki złomowania, sprzedaży lub likwidacji środka trwałego konieczne jest zaksięgowanie wartości sprzedaży/likwidacji. author: SorenGP

ms.service: dynamics365-business-central ms.topic: article ms.devlang: na ms.tgt\_pltfrm: na ms.workload: na ms.search.keywords: scrap ms.date: 10/01/2018 ms.author: sgroespe

---
# Sprzedaż lub likwidacja środków trwałych
W przypadku sprzedaży lub innej metody likwidacji środka trwałego, wartość sprzedaży/likwidacji powinna być zaksięgowana w celu obliczenia i zarejestrowania zysku lub straty.  Zapis sprzedaży/likwidacji powinien być ostatnim zapisem zaksięgowanym dla środka trwałego. W przypadku częściowo zlikwidowanych środków trwałych, można zaksięgować więcej niż jeden zapis sprzedaży/likwidacji. Suma wszystkich zaksięgowanych kwot musi być kwotą kredytu.  

> \[!UWAGA]  
>   W przypadku transakcji wymiany środka trwałego na inny należy zarejestrować zarówno sprzedaż poprzedniego środka (likwidację) oraz zakup nowego (nabycie). Więcej informacji zamieszczono w sekcji [Nabycie środków trwałych](fa-how-acquire.md).  

## Księgowanie zmniejszenia wartości z poziomu dziennika K/G środka trwałego
1. Wybierz ikonę ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Powiedz mi co chcesz zrobić"), wprowadź **Dzienniki ŚT K/G**, a następnie wybierz powiązane łącze.  
2. Utwórz początkowy wiersz dziennika i wypełnij odpowiednio pola.\[!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
3. W polu **Typ księgowania ŚT** wybierz **Alokacja**.  
4. Wybierz akcję **Wstaw konto przeciwst. ŚT**.  Tworzony jest wtedy drugi wiersz dziennika dla konta przeciwstawnego, jakie jest definiowanego dla księgowania likwidacji/sprzedaży.  

    > \[!UWAGA]  
    >   Krok 4 działa tylko w sytuacji, gdy wprowadzono następujące ustawienia: W oknie **Kartoteka gr. księgowej ŚT** dla grupy księgowej środka trwałego, pole **Konto sprzed./likw.** zawiera konto debet K/G, a pole **Konto przeciwst. sprzed./likw.xxx** zawiera konto księgi głównej, na którym mają być zaksięgowane zapisy przeciwstawne dla zwiększenia wartości.  Więcej szczegółowych informacji zamieszczono w sekcji „Konfiguracja grup księgowych środków trwałych” w [Ogólne ustawienia środków trwałych](fa-how-setup-general.md).  
5. Wybierz akcję **Księguj**.  

W przypadku sprzedaży lub likwidacji części środka trwałego, należy dokonać podziału środka przed zarejestrowaniem transakcji sprzedaży/likwidacji. Więcej szczegółowych informacji zamieszczono w sekcji [Przeniesienie, podział lub łączenie środków trwałych](fa-how-trans-split-combine.md).  

## Wyświetlanie zapisów księgi sprzedaży/likwidacji
Podczas sprzedaży likwidacji środka trwałego, wartość sprzedaży/likwidacji jest księgowana do księgi głównej, w której można wyświetlić wynik.   

1. Wybierz ikonę ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Powiedz mi co chcesz zrobić"), wprowadź **Środki trwałe**, a następnie wybierz powiązane łącze.  
2. Wybierz środek trwały, którego zapisy mają być wyświetlone, a następnie wybierz akcję **Księgi amortyzacji**.  
3. Wybierz księgę amortyzacji, której zapisy mają być wyświetlone, a następnie wybierz akcję **Zapisy księgi**.  
4. Wybierz wiersz z opcją **Sprzed./likw.** w polu **Kategoria księgowania ŚT**, a następnie wybierz akcję **Nawiguj**.  
5. W oknie **Nawigacja**, wybierz wiersz zapisu księgi głównej, a następnie wybierz akcję **Pokaż**.  

Zostanie wtedy otwarte okno **Zapisy księgi głównej** zawierające zapisy, które zostały utworzone podczas księgowania sprzedaży/likwidacji.  

## Zobacz też
[Środki trwałe](fa-manage.md)  
[Konfigurowanie środków trwałych](fa-setup.md)  
[Finanse](finance.md)  
[Wprowadzenie](product-get-started.md)  
\[Working with \[!INCLUDE[d365fin](includes/d365fin_md.md)]\](ui-work-product.md)
