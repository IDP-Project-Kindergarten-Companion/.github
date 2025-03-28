# Little Steps

*Aplicatie de monitorizare pentru gradinita*  
Proiect IDP – Universitatea Politehnica Bucuresti  
Autori: Burnichi Alexandra (341C4), Preda Marius (344C1)  
Asistent coordonator: Radu Ciobanu

---

## Descriere

*Little Steps* este o aplicatie inteligenta dedicata parintilor care doresc sa fie permanent conectati cu activitatile zilnice ale copiilor lor aflati la gradinita. Aplicatia permite monitorizarea comportamentului, a alimentatiei si a somnului, precum si arhivarea desenelor realizate de copii intr-un spatiu digital accesibil oricand.

Parintii pot vizualiza progresul copilului printr-o interfata prietenoasa si intuitiva, in timp ce supraveghetorii pot adauga in timp real informatii legate de rutina zilnica a celor mici. Aplicatia sustine o comunicare eficienta intre familie si mediul educational.

---

## Functionalitati

- Autentificare si autorizare cu roluri (parinte / supraveghetor)
- Inregistrarea activitatilor zilnice (masa, somn, comportament)
- Upload si arhivare desene digitale
- Vizualizare profil copil si statistici zilnice/saptamanale
- Interfata web compatibila cu mobilul

---

## Arhitectura

Aplicatia este dezvoltata folosind o arhitectura bazata pe *microservicii* si orchestrata cu *Kubernetes. Comunicarea intre componente este realizata prin HTTP, rutele fiind gestionate de **Kong API Gateway*.

### Microservicii:

- Auth Service – Autentificare si gestionare roluri (Flask + MongoDB)
- Business Logic Service – Evaluari si logica aplicatiei (Flask)
- Database Interaction Service – Operatii CRUD pe datele copiilor (Flask + MongoDB)
- Frontend – Interfata React pentru utilizatori

### Componente auxiliare:

- MongoDB – Doua instante: una pentru auth, una pentru datele copiilor
- Mongo Express – Interfata web pentru administrarea MongoDB
- Kong – API Gateway pentru rutare si securitate
- Portainer – UI pentru gestionarea clusterului Kubernetes
- GitLab CI/CD – Automatizare build si deployment
- Prometheus + Grafana – Logging si monitorizare

---

## Tehnologii folosite

| Componenta                 | Tehnologie                |
|---------------------------|---------------------------|
| Frontend                  | React.js                  |
| Backend Microservices     | Flask (Python)            |
| Baze de date              | MongoDB                   |
| DB Management             | Mongo Express             |
| Gateway                   | Kong                      |
| Orchestrare               | Kubernetes + Docker       |
| CI/CD                     | GitLab Pipelines          |
| Monitorizare              | Prometheus + Grafana      |
| Cluster UI                | Portainer                 |

---

## Impartirea sarcinilor

*Alexandra Burnichi*
- Design si implementare interfata React
- Scriere si testare logica frontend
- Documentatie si UX flow

*Marius Preda*
- Arhitectura backend si microservicii
- Implementare backend + autentificare
- Configurare CI/CD si deployment in Kubernetes

---

## Repository-uri

- [Auth Service](https://github.com/littlesteps-org/auth-service)
- [Business Logic Service](https://github.com/littlesteps-org/business-logic-service)
- [Database Interaction Service](https://github.com/littlesteps-org/db-interaction-service)
- [Frontend](https://github.com/littlesteps-org/frontend)
- [Infrastructure & Deployment](https://github.com/littlesteps-org/infrastructure)

