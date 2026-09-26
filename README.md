# 🏡 DietiEstates25

Piattaforma Web Full-Stack per la ricerca, la pubblicazione e la gestione avanzata di inserzioni e proposte immobiliari.

> **Progetto accademico** per il corso di *Ingegneria del Software*  
> 🎓 **Università degli Studi di Napoli Federico II** (A.A. 2024/2025)

---

## 👥 Team & Crediti

| Ruolo | Nome / Riferimenti |
| :--- | :--- |
| **Sviluppatori** | Gennaro Emanuele Di Costanzo<br>Nives Cassese |
| **Docenti** | Prof. Sergio Di Martino<br>Prof. Luigi Libero Lucio Starace |

---

## 💡 Panoramica del Progetto

**DietiEstates25** è un'applicazione web completa progettata per semplificare l'interazione tra utenti, agenti immobiliari e amministratori di sistema.

### **Funzionalità Principali**
- 🔍 **Ricerca e Filtri:** Esplorazione e ricerca avanzata di inserzioni immobiliari basata su filtri specifici e mappe interattive.
- 🔐 **Autenticazione Sicura:** Registrazione e Login nativo con gestione JWT o tramite OAuth2 (Google e GitHub).
- 🏷️ **Gestione Inserzioni:** Creazione, modifica e pubblicazione di annunci con supporto all'upload di immagini.
- 🤝 **Gestione Proposte:** Invio, tracciamento e gestione delle proposte d'acquisto o affitto sia lato utente che lato agente.
- 👤 **Gestione Profilo & Supporto:** Gestione dei dati utente/agente e servizio di notifiche/reset password via e-mail.

---

## 🛠️ Tecnologie Utilizzate

### **Backend**
* **Linguaggio & Framework:** Java 17, Spring Boot 3.5.6
* **Sicurezza & Autenticazione:** Spring Security, OAuth2 Client, JWT (JSON Web Token)
* **Persistenza & Database:** Spring Data JPA, Hibernate, PostgreSQL
* **Utilities & Monitoraggio:** Spring Mail, Spring Validation, Spring Boot Actuator, Lombok
* **Cloud Storage:** Google Cloud Storage (gestione ed hosting e-media/immagini)
* **Testing:** JUnit 5, Mockito

### **Frontend**
* **Framework & Core:** Angular 20, TypeScript, RxJS
* **UI & Styling:** Angular Material, Bootstrap
* **Mappe & Geolocalizzazione:** Leaflet, Google Maps API
* **Testing:** Jasmine, Karma

---

## 📁 Struttura del Progetto

```text
DietiEstates25/
├── backend/
│   ├── controller/      # Endpoints e gestione API REST
│   ├── service/         # Logica di business
│   ├── repository/      # Interazione con il database (Spring Data JPA)
│   ├── model/           # Entità di dominio / persistenti
│   ├── dto/             # Data Transfer Objects e Mapper
│   ├── security/        # Filtri JWT, configurazioni di sicurezza e OAuth2
│   └── config/          # Configurazioni generali dell'applicazione
│
└── frontend/
    ├── components/      # Componenti UI riutilizzabili
    ├── pages/           # Viste e pagine principali della SPA
    ├── services/        # Servizi di comunicazione HTTP e stato
    ├── guards/          # Protezione delle rotte (Route Guards)
    ├── models/          # Interfacce e tipi TypeScript
    └── assets/          # Risorse statiche (immagini, stili, icone)
