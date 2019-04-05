---
layout: post
title: Enova365 Informacja
excerpt: "Informacja dla Klientów, którzy sporządzili e-sprawozdania finansowe wersją 15.3 enova365."
comments: false
---
W wersji 15.3 ukazała się funkcjonalność wspierająca sporządzanie e-sprawozdań w formie zestawień oraz pliku XLML.

W wersji tej zostały stwierdzone następujące problemy:
<ul>
<li><b>Zestawienia księgowe.</b> Dla wyniku obliczonego zestawienia po kliknięciu na konkretną pozycję nie pokazywały się składowe, w oparciu o które ustalono wynik.</li>
<li><b>e-Sprawozdania.</b> W programie istniał niejasny opis pola "Istnieją okoliczności wskazujące na zagrożenie kontynuowania działalności”, który mógł spowodować wprowadzenie niepoprawnej wartości.</li>
</ul>
Powyższe problemy wyeliminowano w wersji 15.4 enova365 opublikowanej 12 marca 2019:
<ul>
<li>Obecnie w polu Informacja o wyrażeniu prezentowane jest wyrażenie, na podstawie którego została obliczona kwota w danej pozycji.</li>
<li>Skorygowano opis pola dotyczącego okoliczności zagrażających kontynuowaniu działalności, przez nadanie mu następującej treści: <b>"Wskazanie, czy nie istnieją okoliczności wskazujące na zagrożenie kontynuowania przez nią działalności".</b> W przypadku braku zagrożeń pole powinno mieć ustawioną wartość TAK. Zmianę w tym zakresie wprowadzono również na wydruku sprawozdania.</li>
</ul>

<b>Klientom, którzy nie zaktualizowali enova365 do wersji 15.4, a sporządzili e-sprawozdania i podpisali celem dalszego procedowania np. wysłania do KRS lub KAS, rekomendujemy sprawdzenie, czy plik XML został poprawnie wygenerowany.</b>

W szczególności należy zweryfikować, czy dla firm, które nie mają zagrożenia kontynuowania działalności, w pliku XML:
<ol>
<li>wartość w polu P_5B jest ustawiona na true, dla schem sprawozdań wg nazewnictwa w oprogramowaniu enova365: Jednostka inna (tys.), Jednostka inna (zł), Jednostka mała (tys.), Jednostka mała (zł), Jednostka mikro (tys.), Jednostka mikro (zł),</li>
<li>wartość w polu P_4B jest ustawiona na true, dla schem sprawozdań wg nazewnictwa w oprogramowaniu enova365: Jednostka OP (tys.), Jednostka OP (zł)</li>
</ol>

W razie stwierdzenia, że plik został wygenerowany niepoprawnie, należy dokonać korekty. W tym celu należy zapoznać się, w jaki sposób przygotować korektę e-sprawozdania. Stosowna instrukcja znajduje się w Bazie wiedzy (<a href="https://dok.enova365.pl/Topic/35094" target="_blank">tutaj</a>).
