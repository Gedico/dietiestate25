## DietiEstates25

 Piattaforma Full Stack per la gestione di inserzioni immobiliari, con ricerca avanzata, invio proposte e gestione delle proposte.
 Progetto per il corso di Ingegneria del Software
 –Università degli Studi di Napoli Federico II (A.A. 2024/2025).

## Team

- Gennaro Emanuele Di Costanzo
- Nives Cassese

## Docenti

- Sergio Di Martino
- Luigi Libero Lucio Starace


## Struttura del Progetto

DietiEstates25/
 ├── backend/
 │   ├── controller/
 │   ├── service/
 │   ├── repository/
 │   ├── model/
 │   ├── dto/
 │   ├── security/
 │   └── config/
 │
 └── frontend/
     ├── components/
     ├── pages/
     ├── services/
     ├── guards/
     ├── models/
     └── assets/

## Panoramica del progetto

DietiEstates25 è una web application che consente di:

- visualizzare e cercare inserzioni immobiliari tramite filtri;
- registrarsi ed effettuare login (anche tramite Google e Github);
- gestire profilo utente/agente;
- creare e gestire inserzioni (lato agente);
- inviare e gestire proposte lato utente e lato agente;
- ricevere email di supporto (es. reset password).

## Architettura

Il sistema è stato realizzato full stack, quindi prevede sia la costruzione del backend che del frontend.

- Il backend segue una classica **architettura a livelli**:
  - **Controller**: gestione delle API REST
  - **Service**: logica di business
  - **Repository**: accesso ai dati con Spring Data JPA
  - **Entity**: rappresentazione delle entità persistenti
  - **DTO e Mapper**: separazione tra il modello interno e i dati esposti
  - **Security**: configurazione dell'autenticazione e dell'autorizzazione
- Il frontend Angular è organizzato in componenti, pagine e servizi.

## Tecnologie principali

### Backend

- **Java 17**
- **Spring Boot 3.5.6**
- **Spring Web** (REST API)
- **Spring Data JPA + Hibernate**
- **Spring Security**
- **Spring Validation**
- **Spring Mail**
- **OAuth2 Client** (Login Google)
- **JWT** (gestione token)
- **PostgreSQL**
- **Google Cloud Storage** (gestione immagini / upload)
- **JUnit 5 + Mockito** (test)
- **Lombox**
- **Spring Boot Actuator** (monitoraggio)

### Frontend

- **Angular 20**
- **Angular Material**
- **Bootstrap**
- **TypeScript**
- **RxJS**
- **Leaflet e Google Maps**
- **Jasmine e Karma per testing**

## Prerequisiti

Per eseguire il progetto in locale:

- **JDK 17**
- **Maven 3.x**
- **Node.js + npm**
- **PostgreSQL**
- **Credenziali di accesso per test**:

## Avvio del progetto

### Backend (Spring Boot)

mvn clean install
mvn spring-boot:run

### Frontend

npm install
npm start

## Avvio dell'applicazione con Docker

Assicurarsi di trovarsi nella cartella dove è presente il file docker-compose.yml.

Per avviare tutti i servizi (frontend e backend) eseguire:

    docker-compose up -d

Questo comando costruirà e avvierà i container in background.  
Per fermarli:

    docker-compose down


Assicurarsi Di avere una connessione internet per potersi connettere al database.

## Credenziali 

Se si desidera testare le funzionalità, forniamo una serie di credenziali per i vari accessi:

Utente: utente@gmail.com, Password: 12345678
Agente: Agente@gmail.com, Password: 12345678
Admin: Admin@gmail.com,   Password: 12345678
