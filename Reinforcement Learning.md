name: title
class: center, middle, title

# Reinforcement Learning
## and DeepMind

Piotr Januszewski

---

.left-column[
## DeepMind
### - Kto to?
]

.right-column[
# Londyn 2010
Firmę założyli Demis Hassabis, Shane Legg i Mustafa Suleyman w 2010 roku w Londynie.

> Solve intelligence.
> Use it to make the world a better place.

Ich celem jest "rozwiązać inteligencję" i tym samym stworzyć system, który będzie w stanie nauczyć się rozwiązywać dowolnie skomplikowany problem, bez potrzeby wskazania jak.
]

???

1. Hassabis i Legg poznali się na University College London.
2. Stworzenie sztucznej inteligencji, która będzie w stanie ogarnąć wiele problemów, nie potrzebując przy tym specyficznych zmian, aby to osiągnać.

---

.left-column[
## DeepMind
### - Kto to?
### - Debiut
]

.right-column[
### Playing Atari with Deep Reinforcement Learning![:super]
Komputer gra w 7 gier Atari 2600, w 6 z nich gra lepiej niż kiedykolwiek. W trzech z nich pokonuje człowieka na poziomie eksperta.
### Human-level control through deep reinforcement learning![:super]
49 gier Atari 2600. W 29 komputer gra na poziomie człowieka lub lepszym.
]

.footnote[
![:script][Volodymyr Mnih, Koray Kavukcuoglu & David Silver, *Playing Atari with Deep Reinforcement Learning*, Dec 2013](https://arxiv.org/abs/1312.5602)  
![:script][Volodymyr Mnih, Koray Kavukcuoglu & David Silver, *Human-level control through deep reinforcement learning*, "Nature" 518, Feb 2015](https://www.nature.com/nature/journal/v518/n7540/full/nature14236.html)
]

???

1. Zastosowanie jednej i tej samej techniki do każdej gry.
2. Przez te eksperymenty starają się dojść do swojego celu, jakim jest wszechstronna sztuczna inteligencja.
3. Po opublikowaniu pierwszej pracy, Google postanowiło ich kupić w styczniu 2014 roku za 500 mln dolarów.
4. Druga praca pojawiła się na łamach czasopisma "Nature"... (kolejny slajd).

---

.left-column[
## DeepMind
### - Kto to?
### - Debiut
### - Okładka Nature
]

.right-column[
.center[
![:scale 80%](./Reinforcement Learning.d/Nature.png)
]]

???

Powiedz co to za czasopismo.

---

.left-column[
## RL
### - Metoda
]

.right-column[
]

---

.left-column[
## RL
### - Metoda
### - Agent
]

.right-column[
]

---

.left-column[
## RL
### - Metoda
### - Agent
### - Nagroda
]

.right-column[
]

---

.left-column[
## RL
### - Metoda
### - Agent
### - Nagroda
### - Q-learning
]

.right-column[
]

---

.left-column[
## RL
### - Metoda
### - Agent
### - Nagroda
### - Q-learning
### - Deep Q-learning
]

.right-column[
]

---

.left-column[
## Przykłady
### - Seaquest
]

.right-column[
### "Wartość" przykładowych stanów
![:scale 100%](./Reinforcement Learning.d/Seaquest_1.png)
![:scale 100%](./Reinforcement Learning.d/Seaquest_2.png)
1. Kiedy przeciwnik pojawia się z lewej strony ekranu, funkcja wartosci zwraca większe wartości.
2. Zaraz przed uderzeniem torpedy w przeciwnika, funkcja wartości ma największą wartość.
3. Po zniszczeniu przeciwnika wartość spada.
]

???

Powiedz co przedstawiają obrazki.

---

.left-column[
## Przykłady
### - Seaquest
### - t-SNE
]

.right-column[
![:scale 100%](./Reinforcement Learning.d/t-SNE.png)
]

???

1. t-SNE to metoda reprezentowania wielowymiarowej przestrzeni w 2D. Stany "podobne" leżą bliżej siebie.
2. Obrazki są związane z konkretnymi stanami i ich wartościami (oczekiwaną nagrodą).
3. Górne lewe i środkowe oraz dolne prawe nie są podobne percepcyjnie, ale są podobne swoją wartoscią i dlatego leżą blisko siebie. Sieć potrafiła się tego nauczyć.

---

.left-column[
## Przykłady
### - Seaquest
### - t-SNE
### - Porównanie
]

.right-column[
![:scale 90%](./Reinforcement Learning.d/Comparison.png)
]

???

Co przedstawia wykres. Procenty to jak dobrze względem człowieka poradził sobie model (w uproszczeniu).

---

.left-column[
## Przykłady
### - Seaquest
### - t-SNE
### - Porównanie
]

.right-column[
## Montezuma's Revenge
![:scale 90%](./Reinforcement Learning.d/Montezuma's_Revenge.png)
Środowisko w tej grze jest bardzo złożone i różnorodne, a cele nie są trywialne.
]

???

Środowisko w tej grze jest bardzo złożone i różnorodne, a cele nie są trywialne.

---

.left-column[
## Przykłady
### - Seaquest
### - t-SNE
### - Porównanie
]

.right-column[
## Video Pinball
![:scale 90%](./Reinforcement Learning.d/video_pinball.png)
Proste środowisko i jasno zdefiniowane nagrody.
]

???

Proste środowisko i jasno zdefiniowane nagrody.

---

.left-column[
## Przykłady
### - Seaquest
### - t-SNE
### - Porównanie
### - Filmiki
]

.right-column[
## Przykładowe rozgrywki
[Film](https://www.youtube.com/watch?v=iqXKQf2BOSE) przedstawia dwie przykładowe rozgrywki w różnych stadiach rozwoju sieci. Gry to Breakout oraz Space Invaders.
]


---

# Podsumowanie

## Jeden model, wiele problemów
DeepMind przedstawiło model, który otrzymując "gołe" piksele oraz nagrody jako wejścia, z użyciem jednej i tej samej metody uczenia jest w stanie zrozumieć wiele zróżnicowanych środowisk.

## Neurobiologiczne poszlaki
Model ten musiał sam nauczyć się widzieć, a następnie zrozumieć co widzi. Zrobił to otrzymując jedynie nagrody za podjęte przez siebie akcje. Sugeruje to, że sygnały o nagrodach podczas rozwijania percepcji, mogą mieć również wpływ na rozwój kory wzrokowej.

???

1. Model i metody uczenia te same, ale różne środowiska
2. Powiązanie z rozwojem kory wzrokowej.

---

class: middle

# Źródła
https://www.nervanasys.com/demystifying-deep-reinforcement-learning/  
https://arxiv.org/abs/1312.5602  
https://www.nature.com/nature/journal/v518/n7540/full/nature14236.html
