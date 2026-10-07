# Fișă de lucru — Tema 8: Rescrierea documentelor administrative în limbaj clar

**Proiect IAOFU · 2026-2027 · Reper săptămâna 2 (Echipe și alegere)**
**Domeniu delimitat:** regulamente și instrucțiuni de **burse studențești** dintr-o universitate publică
**Echipă:** _(nume membri)_ · **Data:** 2026-10-07

---

## 1. Utilizator și sarcină

**Cine folosește aplicația?** Un student care trebuie să înțeleagă dacă și cum poate obține o bursă
(socială, de merit, de performanță), ce acte depune și până la ce dată — fără să citească integral un
regulament scris în limbaj administrativ.

**Sarcina precisă:** Studentul lipește un fragment din regulamentul oficial de burse. Aplicația îl
**reformulează în limbaj clar, în română**, păstrând termenii și condițiile importante (cuantumuri,
praguri de medie, venit, termene) și afișează **alături fraza originală**. Studentul poate reveni oricând
la textul oficial.

## 2. Ce decide / corectează utilizatorul (nu acceptă automat)

- Comută între **„limbaj clar"** și **textul oficial** pentru orice frază.
- Fiecare reformulare **incertă este marcată explicit** (semnal vizual) — utilizatorul este invitat să verifice în original.
- Studentul poate **respinge sau corecta** o reformulare; decizia finală („sunt eligibil / ce depun")
  rămâne la persoană, nu la sistem.
- Sistemul **nu dă sfaturi juridice** și nu garantează eligibilitatea — doar clarifică textul.

## 3. Flux minim pentru demonstrația din săptămânile 8-9

1. Utilizatorul lipește / selectează un fragment din regulament (1–3 paragrafe).
2. Sistemul produce versiunea în limbaj clar, **propoziție cu propoziție, aliniată la original**.
3. Interfață în două coloane: **original ↔ reformulat**; fiecare segment are buton „vezi originalul" și
   marcaj „reformulare incertă" când e cazul.
4. Un rezumat scurt al **condițiilor și termenelor** extrase (listă: ce trebuie, până când).

## 4. Date: existente, drept de utilizare, de adnotat

- **Sursă:** 15–25 pagini din regulamente/instrucțiuni de burse **publice** (site-uri de universitate),
  domeniu bine delimitat; se citează proveniența și dreptul de folosire.
- **De adnotat de echipă:** **30 de enunțuri** reformulate manual ca referință (gold), cu
  **verificarea manuală a condițiilor și termenelor** păstrate.
- Set de **test separat** de exemplele pe care se reglează sistemul (cerință comună).

## 5. Variantă de comparație (referință) și măsuri

**Referință simplă:** reformulare prin reguli/liste de substituții lexicale (dicționar birocratic→comun)
**fără model de limbaj**, sau un prompt minimal fără aliniere la original și fără marcarea incertitudinii.

**Măsuri că IA ajută:**
- **Păstrarea sensului** — câte condiții/termene din original rămân corecte (verificare manuală).
- **Lizibilitate** — scădere a dificultății (ex. lungime frază, scor de lizibilitate RO) *fără* pierdere de sens.
- **Identificarea corectă a pașilor** — test cu **4–6 persoane**: găsesc corect ce acte și termene au?
- **Timp până la înțelegere** vs. citirea textului oficial.

## 6. Riscul principal (eroare care induce în eroare) și cum se observă

**Risc principal:** reformularea **schimbă subtil o condiție** (ex. „media ≥ 8" devine „media peste 8",
sau omite un termen) — studentul ia o decizie greșită crezând textul clar.

**Cum se observă la testare:**
- La fiecare enunț din setul de test se bifează dacă **toate condițiile și termenele** sunt păstrate corect;
  se raportează explicit rata de **distorsiuni de sens**.
- Reformulările incerte **marcate** vs. nemarcate — se măsoară câte erori scapă nemarcate (cel mai periculos caz).
- În testul cu utilizatori: întrebări de control („până când depui?", „ce medie îți trebuie?") pentru a
  detecta când textul clar i-a indus în eroare.

---

### Legătura cu cerințele comune
- ✔ Flux complet de lucru, prima versiune delimitată.
- ✔ Componentă IA evaluabilă + variantă de referință simplă.
- ✔ Set de test separat; raportare performanță tehnică **și** erori observate.
- ✔ Test cu utilizatori (4–6) pe lângă evaluarea automată.
- ✔ Proveniența și dreptul datelor, costul estimat al apelurilor, mod de corectare/anulare a unui rezultat.

### De completat până în săptămâna 3
- [ ] Alegerea universității/regulamentului concret și verificarea dreptului de folosire.
- [ ] Colectarea celor 15–25 de pagini + împărțire train/test.
- [ ] Redactarea celor 30 de enunțuri de referință adnotate.
- [ ] Estimarea costului apelurilor la model.
