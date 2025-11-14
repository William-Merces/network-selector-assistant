# 🧭 ADDENDUM Q4 2025 — SMALL GROUP NETWORK RULES (REV. NOV 2025)
**Autoridade:** Jake Page & Adriana Pastor  
**Status:** Substitui o Addendum original “Small Group Fallback Networks” (Out 2025)  
**Versão:** v2.0 — Novembro 2025  
**Aplicação:** Todos os grupos **com menos de 10 vidas** (Q4 2025)  
**Prioridade:** Sobrepõe qualquer fallback anterior (inclusive Healthlink)

---

## 1️⃣ CONTEXTO
Durante o Q4, o Arlo ainda bloqueia cotações na **Cigna PPO** para grupos com **menos de 10 vidas**, exibindo:
> “Quote Submission Error: We are unable to accommodate quoting this group on the PPO network selected due to not meeting the minimum requirement with our network vendor.”

O antigo “fallback padrão” (Healthlink) **não deve mais ser usado automaticamente.**  
A escolha da rede de substituição agora depende **da localização geográfica** e segue diretrizes diretas da liderança (Jake & Adriana).

---

## 2️⃣ NOVAS REGRAS DE REDE PARA GRUPOS <10 LIVES

| Região / Estado | Rede padrão a tentar primeiro | Rede alternativa (após erro de mínimo) | Observações |
|------------------|-------------------------------|----------------------------------------|-------------|
| **Northeast Georgia / North Atlanta** | Level Health – Cigna | **GA Health Partners w FH Wrap** | Health Partners é **exclusiva** do nordeste e norte de Atlanta. |
| **Resto da Geórgia (Macon, Columbus, Savannah, etc.)** | Level Health – Cigna | **Level-Health – EHN EPO** | EHN substitui Healthlink fora do NE GA. |
| **Tennessee (fora de Memphis), Alabama, Carolinas, Flórida** | Level Health – Cigna | **Level-Health – EHN EPO** | EHN agora cobre essas regiões pequenas quando <10 vidas. |
| **Memphis, TN / West TN** | Level Health – Cigna | **$0 Local Contract (Baptist Memorial)** | Mantém regra de rede local. |
| **Estados sem rede EHN (NV, AZ, NM)** | Level Health – Cigna | **Level Health – First Choice PPO** | Fallback técnico (mesmo da versão anterior). |
| **Menos de 5 vidas (qualquer estado)** | — | **DTQ (Declined to Quote)** | Arlo não permite submissão abaixo de 5. |

---

## 3️⃣ PROCEDIMENTO ATUALIZADO (ARLO)

1. Tentar **Cigna PPO** como rede padrão.  
2. Se aparecer o erro de “minimum requirement”:  
   - Determinar a **região real do grupo** (ZIP/cidade principal).  
   - Aplicar a rede alternativa da tabela acima.  
3. Reenviar a cotação **com a rede alternativa correta**.  
4. Registrar no HubSpot a nota padrão de ressubmissão (ver seção 5).

---

## 4️⃣ EXEMPLOS PRÁTICOS

| Empresa | Localização | Enrolled | Resultado esperado |
|----------|--------------|-----------|--------------------|
| **Edmondson Telford Center for Children** | Gainesville, GA (NE GA) | 5 | Health Partners w FH Wrap ✅ |
| **ABC Electric Co.** | Macon, GA | 8 | EHN ✅ |
| **Sunrise Dental Group** | Jacksonville, FL | 7 | EHN ✅ |
| **Henderson Auto Repair** | Nashville, TN | 6 | EHN ✅ |
| **Switch Care** | Denton, TX | 7 | Healthlink ✅ *(Texas ainda usa Healthlink fallback técnico)* |
| **Mini Manufacturing LLC** | Kansas City, MO | 9 | $0 Local Contract (Centrus) ✅ |
| **West Valley Builders** | Las Vegas, NV | 8 | First Choice PPO ✅ |

---

## 5️⃣ NOTA PADRÃO DE DOCUMENTAÇÃO (HUBSPOT)
Use este modelo sempre que ocorrer reenvio por erro de rede mínima:

```
Submitted to Arlo per updated small group network guidance (Jake/Adriana).
Initial submission on Cigna PPO returned minimum requirement error (<10 enrolled).
Resubmitted using [Network Name] as per regional rules.
Level Health Standard quote with:
- Tier 1: [Network]
- Tier 2: [Secondary or N/A]
```

---

## 6️⃣ MAPA RÁPIDO — REDES <10 VIDAS

| Região | Tier 1 | Tier 2 |
|---------|--------|--------|
| NE Georgia / N Atlanta | Northeast Georgia Health Partners | First Health |
| Restante da Geórgia | Employer’s Health Network (EHN) | N/A |
| Tennessee / Alabama / Carolinas / Flórida | Employer’s Health Network (EHN) | N/A |
| Memphis / West TN | Baptist Memorial Health | Healthlink OA III |
| Texas / Midwest | Healthlink OA III | N/A |
| Oeste (NV, AZ, NM) | First Choice Health Network | N/A |

---

## 7️⃣ IMPACTO NO PROCESSO

- Este documento **substitui completamente** o antigo fallback “Healthlink para <10 vidas”.  
- **EHN passa a ser a rede padrão alternativa fora do NE Georgia.**  
- O Addendum original (Healthlink fallback) deve ser mantido apenas como referência técnica, **não operacional**.  
- **Jake Page e Adriana Pastor** são a autoridade final para exceções.

---

## 8️⃣ REFERÊNCIAS CRUZADAS

- Substitui seções 3–6 do “Addendum Q4 2025 – Small Group Fallback Networks”.  
- Compatível com *INSTRUÇÕES_FIXAS_ASSISTENTE_DE_COTACAO_LEVELHEALTH_SIMPARA.md*.  
- Vinculado ao *LevelHealth_Full_Guide.md* (versão Outubro 2025) – Seção 4.2 e 8.1.  
- Aprovado por: Jake Page (Head of Growth) e Adriana Pastor (Underwriting Ops).  
- Última atualização: **10 de novembro de 2025.**
