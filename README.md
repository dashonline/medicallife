# Dashboard de Tráfego — Dr. Luiz Araujo

Dashboard estática (GitHub Pages) da conta Meta **MEDICAL ANUNCIOS** (`act_885696692755554`).
Headline = **mensagens** (1ª resposta). Imposto ×1,1385 sobre todo gasto. CTR sempre de link.

- `build.ps1` lê a Meta Graph API (nível anúncio, por dia, desde 2026-01-01, todas as campanhas) e gera `data.js`.
- **Agendamentos**: lidos ao vivo da planilha da equipe `1PF2txGK4WJ3HWstG_OBSQtcBwV337GeUn2X7fhtWO_Q`
  (1 aba por mês, `Set/2026`...). Agendamentos = Vacinas Marcadas + Médico Parceiro + Consulta Alergista.
- `.github/workflows/build.yml` roda de hora em hora e publica no Pages. Token no secret `META_ACCESS_TOKEN`.

## Rodar local
```powershell
.uild.ps1 -Mode all
python -m http.server
```
