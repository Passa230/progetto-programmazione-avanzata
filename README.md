# 📦 Inventory Manager

**Inventory Manager** è un sistema software completo per la gestione della logistica e delle scorte multi-magazzino. 
Il progetto è suddiviso in due componenti principali: un **Backend RESTful** ad alte prestazioni e un **Client Desktop** con interfaccia grafica reattiva.

## 🚀 Caratteristiche Principali
* **Gestione Multi-Magazzino**: Creazione, modifica ed eliminazione di magazzini fisici o virtuali.
* **Gestione Prodotti**: Monitoraggio delle giacenze, dei prezzi e delle descrizioni dei prodotti in ogni magazzino.
* **Sistema di Autenticazione**: Login sicuro con hashing delle password (Spring Security).
* **Interfaccia Reattiva (Asincrona)**: Il client desktop utilizza chiamate HTTP asincrone (`CompletableFuture`) per garantire una UI fluida e non bloccante.

---

## 🛠️ Tecnologie Utilizzate

### Backend (Server)
* **Java 21**
* **Spring Boot** (Web, Data JPA, Validation)
* **Spring Security** (Autenticazione e Autorizzazione)
* **MySQL** (Database relazionale)
* **Flyway** (Gestione automatizzata delle migrazioni e dello schema DB)
* **Lombok** (Riduzione del codice boilerplate)
* **JUnit 5, Mockito & MockMvc** (Test Unitari e di Integrazione)

### Frontend (Client)
* **Java 21**
* **JavaFX** (Interfaccia Grafica)
* **Java `HttpClient`** (Comunicazione REST asincrona con il backend)
* **CSS** (Styling dell'interfaccia)
* **Jackson / Gson** (Serializzazione e deserializzazione JSON)

---

## 📋 Prerequisiti

Per eseguire questo progetto sul tuo computer, devi avere installato:
1. **Java Development Kit (JDK) 21** (o superiore).
2. **Apache Maven** (per la gestione delle dipendenze e la build).
3. **MySQL Server** in esecuzione (di default sulla porta `3306`).

---

## ⚙️ Installazione e Avvio

Il progetto è composto da due cartelle separate: il backend (server) e il frontend (client). **È fondamentale avviare prima il server e poi il client.**

### 1. Configurazione del Database
Il progetto utilizza **Flyway**. Non devi creare manualmente le tabelle, ti basta creare un database vuoto:
1. Apri MySQL (es. tramite MySQL Workbench o terminale).
2. Esegui il seguente comando:
   ```sql
   CREATE DATABASE 672567;
