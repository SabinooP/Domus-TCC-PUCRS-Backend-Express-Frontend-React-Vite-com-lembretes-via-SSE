# DOMUS — TCC PUCRS
Backend (Express) + Frontend (React/Vite) com lembretes via SSE.

## Como rodar
**Backend**
1. `cd backend`  
2. `npm install`  
3. `npm run dev` → http://localhost:3000

**Frontend**
1. `cd frontend-react`  
2. `npm install`  
3. (opcional) criar `.env` a partir de `.env.example` e ajustar `VITE_WATERMARK`  
4. `npm run dev` → http://localhost:5173

## API
`GET /tasks` · `GET /tasks/:id` · `POST /tasks` · `PATCH /tasks/:id` · `DELETE /tasks/:id`  
Tempo real (SSE): `GET /events` · Próximos: `GET /reminders/upcoming?minutes=N`

## Observações
- Acentuação preservada.  
- Lembretes dependem da **aba aberta** (MVP).  
- `backend/db.json` não é versionado; use `backend/db.example.json`.
