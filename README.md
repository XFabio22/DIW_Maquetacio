# Restaurant Els Coberts - Pràctica 11: Multimedia, Transitions & Animations

## Condicions d'entrega i compliment
- [cite_start]**Branca del projecte:** Desenvolupat a la branca 'multimedia'[cite: 14].
- [cite_start]**Sense JavaScript per a efectes visuals:** Totes les transicions i animacions s'han realitzat exclusivament amb CSS pur[cite: 16].
- [cite_start]**Comentaris en el codi:** S'han inclòs comentaris explícits tant en el fitxer HTML com en el CSS explicant cadascun dels canvis realitzats[cite: 17].
- [cite_start]**Propietats de classe:** Només s'han utilitzat les propietats i sintaxis vistes a classe i en els apunts[cite: 18].

---

## Localització de Transicions i Animacions

### Exercici 1: Transicions

#### 1.1 Transició a les imatges de la galeria
- **Localització:** `Index.css` (Secció de la galeria)
- [cite_start]**Descripció:** S'activa amb el `:hover` sobre la imatge[cite: 25]. [cite_start]Utilitza simultàniament les propietats `scale`, `rotate` i `grayscale`[cite: 26]. [cite_start]L'element pare té aplicat `overflow: hidden` perquè la imatge no surti del seu contingut[cite: 27].

#### 1.2 Transició personalitzada (Menú de navegació)
- **Localització:** `Index.css` (Secció de navegació)
- [cite_start]**Descripció:** Transició lliure aplicada als enllaços de la barra de navegació (`.nav-links a`) en fer `:hover`[cite: 28]. [cite_start]Modifica 3 propietats CSS: `color`, `text-shadow` i `transform`[cite: 28].

---

### Exercici 2: Animacions

#### 2.1 Animació del text inicial de la capçalera
- **Localització:** `Index.css` (`@keyframes heroTextFadeMove` i `.hero-text`)
- [cite_start]**Descripció:** Animació automàtica en carregar la pàgina que fa aparèixer el text a poc a poc (opacity), el mou cap amunt (transform) i canvia el color de taronja a blanc[cite: 36]. [cite_start]S'utilitza `animation-fill-mode: forwards` perquè es quedi permanentment en l'estat final[cite: 37, 50].

#### 2.2 Animació personalitzada (Botó d'enviament)
- **Localització:** `Index.css` (`@keyframes submitButtonPulse` i `.btn-submit:hover`)
- [cite_start]**Descripció:** Animació que s'activa amb el `:hover` utilitzant exactament 4 frames (0%, 33%, 66%, 100%) i canvia el valor de 3 propietats: `background-color`, `box-shadow` i `transform`[cite: 56].

---

### Exercici 3 i 4: Vídeo i Controls Multimèdia

#### 3.1 Inclusió del vídeo responsive
- [cite_start]**Localització:** `Index.html` (Després de la galeria de fotos) i `Index.css` [cite: 59]
- [cite_start]**Descripció:** Etiqueta `<video>` centrada i adaptada al tamany del navegador sense generar scroll horitzontal[cite: 64, 65]. [cite_start]Per defecte està parat, silenciat i sense els controls natius del navegador[cite: 66, 72].

#### 4.1 Controls personalitzats amb icones(el video no te so)
- **Localització:** `Index.html` (Estructura de controls i funcions JavaScript) i `Index.css`
- [cite_start]**Descripció:** Capa amb fons fosc i transparent que conté icones de Google Fonts (`play_circle`, `pause_circle`, `volume_up`, `volume_off`)[cite: 77, 90, 91]. [cite_start]Les icones apliquen un efecte de shadow en passar el ratolí per sobre[cite: 75]. [cite_start]S'utilitza JavaScript natiu per programar les accions de reproducció, pausa, activar volum i silenciar en fer clic[cite: 80, 81, 83, 85].

---

### Exercici 5: JavaScript amb Scroll

#### 5.1 Reducció del menú de navegació (Navbar Shrink)
- [cite_start]**Localització:** `Index.html` (Event `window.onscroll`) i `Index.css` [cite: 97]
- [cite_start]**Descripció:** S'aplica una transició mitjançant JavaScript que redueix el tamany del menú de navegació quan l'usuari fa scroll cap avall a la pàgina[cite: 97].

#### 5.2 Reproducció automàtica per proximitat
- **Localització:** `Index.html` (Dins de la funció d'scroll)
- [cite_start]**Descripció:** Control d'scroll que activa automàticament el `.play()` del vídeo quan aquest entra dins de l'àrea visible de l'usuari (viewport)[cite: 99].