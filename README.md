# Model za generisanje teksat na osnovu zadate teme ili upita
## Uvod
Jedan od najmoćnijih alata za generisnje teksta je GPT-2 model (Generative Pre-trained Transformer 2). GPT-2 je jezički model baziran na transformer arhitekturi, koji je razvio OpenAI. To je napredni model vještačke inteligencije obučen na ogromnom skupu tekstualnih podataka. GPT-2 je sposoban da generiše kvalitetan tekst na osnovu zadatog ulaza, bilo da su to rečenice, teksta ili pitanja. 

## Dokumentacija
1.	Instalacija biblioteka - Prije pokretanja koda, potrebno je instalirati neophodne biblioteke: 'transformers' i 'googletrans'. Ovo se može uraditi pomoću `pip` alata u komandnoj liniji.
2.	Importovanje neophodnih modula - Nakon instalacije, uvozimo potrebne module iz instaliranih biblioteka. Koristimo module iz `transformers` biblioteke za rad sa GPT-2 modelom, kao i Translator modul iz `'googletrans'` biblioteke za prevođenje teksta.
3.	Inicijalizacija GPT-2 modela i tokenizatora –Inicijalizujemo GPT-2 jezički model i tokenizator. Ova inicijalizacija omogućava rad sa GPT-2 modelom velikih dimenzija (`gpt2-large`).
4.	Definisanje tema/pitanja za generisanje teksta - Korak prije generisanja novog teksta je definisanje teme ili pitanja za generisanje. Korisnik unosi tekst koji se dalje procesira. Ako je tekst na jeziku koji nije engleski, prethodno se vrši prevod teksta na engleski jezik.
5.	Tokenizacija ulaznog teksta - Nakon definisanja ulaznog teksta, vrši se njegova tokenizacija. Tokenizacija predstavlja proces pretvaranja teksta u niz tokena koji je razumljiv modelu.
6.	Generisanje novog teksta - Generiše se novi tekst koristeći GPT-2 jezički model. Model prima tokenizovani ulaz i generiše odgovarajući izlaz.
7.	Dekodiranje generisanog izlaza - Generisani izlaz, koji je u obliku tokena, dekodira se nazad u tekstualni format koji je lako čitljiv.
8.	Prevođenje teksta (opcionalno) - Ukoliko je tekst preveden za generisanje, sada se vraća u početni jezik. Ovo omogućava da se rezultat prevedenog teksta prikaže korisniku na željenom jeziku.
9.	Ispisivanje generisanog teksta - Na kraju, generisani tekst se ispisuje. Ukoliko je tekst predugačak, može se podijeliti u manje dijelove radi lakšeg prikaza.
