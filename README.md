# 🔐 Password Leak Checker con Have I Been Pwned API

Questo è un semplice script Python che ti permette di controllare se una o più password sono state compromesse (cioè trovate in un data breach) utilizzando l'API pubblica del sito [Have I Been Pwned](https://haveibeenpwned.com/).

## 📚 Progetto realizzato durante un corso su Udemy

Questo script è stato sviluppato seguendo una lezione del corso **"How to become a Python 3 Developer and get hired! Build 12+ projects, learn Web Development, Machine Learning + more!"** su [Udemy](https://www.udemy.com/course/complete-python-developer-zero-to-mastery), per imparare a:

- Lavorare con le API pubbliche
- Usare `requests` per fare chiamate HTTP
- Manipolare hash SHA-1 con la libreria `hashlib`
- Gestire input da terminale con `sys.argv`

---

## 🛠️ Come funziona

1. Inserisci una o più password da controllare.
2. Lo script calcola l'hash SHA-1 della password.
3. Invia **solo i primi 5 caratteri** dell'hash all'API di Have I Been Pwned.
4. Confronta la risposta dell'API per vedere se il resto dell'hash è presente.
5. Ti dice quante volte quella password è stata trovata nei database hackerati.

---

## ▶️ Come usarlo

Una volta clonato il progetto e installato le dipendenze, da riga di comando digitare:

- `python check_my_pass.py password123`
- `python check_my_pass.py ciao1234`
