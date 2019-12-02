---
title: Ubezpieczenie środków trwałych | Opis Microsoft Docs: Środek trwały można przypisać do polisy ubezpieczeniowej, której odzwierciedleniem jest  kartoteka ubezpieczenia.services: project-madeira documentationcenter: '' author: SorenGP

ms.service: dynamics365-business-central ms.topic: article ms.devlang: na ms.tgt\_pltfrm: na ms.workload: na ms.search.keywords: policy, coverage ms.date: 10/01/2018 ms.author: sgroespe

---
# Ubezpieczenie środków trwałych
Polisy ubezpieczeniowe środków trwałych są zawarte w kartotece ubezpieczenia. Możliwe jest przypisanie jednego środka trwałego do jednej polisy ubezpieczeniowej lub wielu środków trwałych do jednej polisy.

Można przypisać środek trwały do polisy ubezpieczeniowej poprzez zaksięgowanie go w księdze pokrycia ubezpieczenia z okna **Dziennik ubezpieczenia**.

Dodatkowo, można przypisać środek trwały do polisy ubezpieczeniowej, a następnie utworzyć zapisy księgi pokrycia po zaksięgowaniu kosztu nabycia. W tym celu należy zaksięgować koszt nabycia z dziennika środka trwałego w polu **Nr ubezpieczenia**. Pole wyboru **Automat. księgow. ubezpiecz.** w oknie **Ustawienia ŚT** powinno być zaznaczone. Więcej szczegółowych informacji zamieszczono w sekcji „Ręczne księgowanie nabycia środka trwałego przy pomocy dziennika K/G środków trwałych” w [Nabycie środków trwałych](fa-how-acquire.md).

Jeśli zaznaczono pole wyboru w **Automat. księgow. ubezpiecz.** w oknie **Ustawienia ŚT**, w wyniku księgowania nabycia z dziennika środków trwałych zostaną utworzone wiersze  w oknie **Dziennik ubezpieczenia**, który należy następnie zaksięgować ręcznie.

> \[!WARNING]  
>   Jeśli pole wyboru **Automat. księgow. ubezpiecz.** w oknie **Ustawienia  ŚT**, dziennik ubezpieczeń powinien opierać się na szablonie dziennika bez serii numeracji. Wynika to z tego, że numery dokumentów  wstawione z wiersza dziennika środka trwałego będą w przeciwnym razie niezgodne z serią numeracji dziennika ubezpieczenia. Więcej informacji na temat szablonów dzienników i instancji zamieszczono w **Ogólne ustawienia środków trwałych**.

Po przypisaniu środka trwałego do polisy ubezpieczeniowej, pole wyboru **Ubezpieczone** zostanie zaznaczone na kartotece środka trwałego. Po sprzedaży środka trwałego, pole wyboru zostanie automatycznie wyłączone.

## Tworzenie lub modyfikowanie kartoteki ubezpieczeń
Polisy ubezpieczeniowe środków trwałych powinny być odzwierciedlone w kartotece ubezpieczenia.

Po otrzymaniu informacji dotyczących zamian w kwocie pokrycia, należy wprowadzić nowe informacje w oknie **Kartoteka ubezpieczenia**, aby zagwarantować poprawne przeanalizowanie pokrycia polisy ubezpieczeniowej.  

1. Wybierz ikonę ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Powiedz mi co chcesz zrobić"), wprowadź **Ubezpieczenie**, a następnie wybierz powiązane łącze.
2. Wybierz akcję **Nowy**, aby utworzyć nową kartę dla polisy ubezpieczeniowej.\[!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. Alternatywnie, wybierz polisę ubezpieczeniową, której dotyczą zmiany, a następnie wybierz akcję **Edycja**.

## Przypisanie środka trwałego do polisy ubezpieczeniowej poprzez zaksięgowanie go z dziennika ubezpieczenia.
Środek trwały można przypisać do polisy ubezpieczeniowej poprzez zaksięgowanie go w księdze pokrycia ubezpieczenia.  

Poniższa procedura objaśnia sposób ręcznego tworzenia wiersza dziennika ubezpieczenia. Jeśli pole wyboru**Automat. księgow. ubezpiecz.** zostało zaznaczone w oknie **Ustawienia ŚT**, wiersze dziennika ubezpieczenia są automatycznie tworzone podczas księgowania kosztów nabycia. W takim przypadku, należy tylko zaksięgować dziennik.  

1. Wybierz ikonę ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Powiedz mi co chcesz zrobić"), wprowadź **Dzienniki ubezpieczeń**, a następnie wybierz powiązane łącze.  
2. Otwórz odpowiedni dziennik, a następnie wypełnij odpowiednio wiersze dziennika.  
3. W celu przypisania wielu środków trwałych do jednej polisy ubezpieczeniowej, utwórz wiersze dziennika z tą samą wartością w polu **Nr ubezpieczenia** i różnymi wartościami w polu **Nr  ŚT**.  
4. Wybierz akcję **Księguj**.  

    > \[!UWAGA]  
    >   Zapisy z dziennika ubezpieczenia są księgowane tylko do księgi pokrycia ubezpieczenia.  

## Aktualizacja wartości ubezpieczenia środka trwałego
Aktualizację wartości środków trwałych objętych ubezpieczeniem można przeprowadzić przy pomocy zadania wsadowego **Indeksowanie ubezpieczenia**.  

1. Wybierz ikonę ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Powiedz mi co chcesz zrobić"), wprowadź **Indeksowanie ubezpieczenia**, a następnie wybierz powiązane łącze.
2. Wypełnij odpowiednio pola.

    > \[!UWAGA]  
    >   W polu **Współczynnik indeksowania** zmniejszenie o np. 5% wprowadza się jako 95, a zwiększenie o %2 jako 102.  
3. Kliknij przycisk **OK**.  

   Zadanie wsadowe oblicza nową kwotę jako procent całkowitej wartości ubezpieczenia określonej w oknie **Statystyka ubezpieczenia**, a następnie tworzy wiersz w dzienniku ubezpieczeń.  
4. Wybierz ikonę ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Powiedz mi co chcesz zrobić"), wprowadź **Dzienniki ubezpieczeń**, a następnie wybierz powiązane łącze.  
5. Otwórz odpowiedni dziennik ubezpieczeń, przejrzyj utworzone wartości, a następnie zaksięguj je w księdze pokrycia ubezpieczenia.  

## Monitorowanie pokrycia ubezpieczenia
\[!INCLUDE[d365fin](includes/d365fin_md.md)] zawiera specjalne raporty i okna statystyk wykorzystywane w analizie polis ubezpieczeniowych oraz tego, czy zawarto je na odpowiednią wartość dla poszczególnych środków trwałych.  

### Zestawienie polis ubezpieczeniowych
W celu przejrzenia zestawienia polis ubezpieczeniowych, wyświetl lub wydrukuj raport **Ubezpieczenia - Lista**.xxx Raport zawiera wszystkie polisy i najważniejsze pola z kartotek ubezpieczeniowych.  

### Pokrycie ubezpieczenia
 Aby sprawdzić, które polisy ubezpieczeniowe obejmują każdy składnik aktywów i w jakiej kwocie, można wyświetlić podgląd raportu **Ubezpieczenie - ubezpieczona wartość razem** lub go wydrukować.  

### Ubezp. powyżej/poniżej wart.
Istnieją następujące sposoby sprawdzenia, czy środki trwałe są nadmiernie lub niewystarczająco ubezpieczone:  

* Okno **Statystyka ubezpieczenia**. Kwota dodatnia w polu **Ubezp. powyżej/poniżej wart.** oznacza, że środek trwały jest nadmiernie ubezpieczony. Kwota ujemna oznacza, że jest niedoubezpieczony.  
* Okno **Statystyka środka trwałego**. Wybierz pole **Ubezpieczona wartość razem** w celu wyświetlenia okna  **Zapisy księgi pokrycia**.  
* Raport **Ubezp. powyżej/poniżej wart.**.  
* Raport **Analiza ubezpieczenia**.  

### Nieubezpieczone środki trwałe
Aby sprawdzić, czy nie zapomniałeś przypisać środka trwałego do polisy ubezpieczeniowej, możesz wydrukować lub wyświetlić podgląd raportu o **Ubezpieczenie - nieubezp. ŚT**. Ten raport wyświetla środki trwałe, których kwoty nie zostały zaksięgowane do księgi pokrycia ubezpieczenia.  

## Wyświetlanie zapisów księgi pokrycia ubezpieczenia
Możliwe jest wyświetlenie zapisów wprowadzonych w księdze pokrycia ubezpieczenia.  

1. Wybierz ikonę ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Powiedz mi co chcesz zrobić"), wprowadź **Ubezpieczenie**, a następnie wybierz powiązane łącze.  
2. Wybierz odpowiednią polisę ubezpieczeniową, a następnie wybierz akcję **Zapisy księgi pokrycia**.  

## Wyświetlanie wartości ubezpieczenia środków trwałych
Dedykowane okno macierzy pokazuje wartości ubezpieczenia, które są zarejestrowane dla każdej polisy ubezpieczeniowej dla każdego środka trwałego w wyniku zaksięgowanych kwot związanych z ubezpieczeniem.  

1. Wybierz ikonę ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Powiedz mi co chcesz zrobić"), wprowadź **Ubezpieczenie**, a następnie wybierz powiązane łącze.  
2. Wybierz odpowiednią polisę ubezpieczeniową, a następnie wybierz akcję **Całkowita wartość ubezpieczenia wg ŚT**.  
3. Wypełnij odpowiednio pola.  
4. Wybierz akcję **Pokaż macierz**.  
5. Aby wyświetlić podstawowe zapisy księgi pokrycia ubezpieczenia, wybierz wartość w macierzy.  

## Korygowanie zapisów księgi pokrycia ubezpieczenia
Jeśli środek trwały został załączony do niewłaściwej polisy ubezpieczeniowej, można go skorygować poprzez tworzenie dwóch zapisów podziału z dziennika ubezpieczenia.  

1. Wybierz ikonę ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Powiedz mi co chcesz zrobić"), wprowadź **Dzienniki ubezpieczeń**, a następnie wybierz powiązane łącze.  
2. Utwórz jeden wiersz dziennika dla środka trwałego i skoryguj polisę ubezpieczeniową, w przypadku której wartość w polu **Kwota** jest dodatnia.  
3. Utwórz inny wiersz dziennika dla środka trwałego i niepoprawnej polisy ubezpieczeniowej, w przypadku której wartość w polu **Kwota** jest ujemna.  
4. Wybierz akcję **Księguj**.  

Środek trwały zostanie odłączony od niepoprawnej polisy ubezpieczeniowej, w drugim wierszu, i dołączony do właściwej polisy ubezpieczeniowej, w pierwszym wierszu.  

## Zobacz też
[Środki trwałe](fa-manage.md)  
[Konfigurowanie środków trwałych](fa-setup.md)  
[Finanse](finance.md)  
\[Working with \[!INCLUDE[d365fin](includes/d365fin_md.md)]\](ui-work-product.md)  
