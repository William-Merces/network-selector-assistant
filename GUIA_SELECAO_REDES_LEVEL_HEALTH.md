# 🗺️ GUIA DE SELEÇÃO DE REDES LEVEL HEALTH
## Referência Rápida para Escolha da Rede Correta

*Versão: Outubro 2025 - Baseado em Network Options.xlsx*

---

## 📋 ÍNDICE

1. [Como Usar Este Guia](#como-usar-este-guia)
2. [Árvore de Decisão Rápida](#árvore-de-decisão-rápida)
3. [Redes Standard (Nacionais)](#redes-standard-nacionais)
4. [Redes Local/Direct por Estado](#redes-localdirect-por-estado)
5. [Tabela de Referência Rápida por ZIP](#tabela-de-referência-rápida-por-zip)
6. [Mapeamento Portal Arlo → HubSpot](#mapeamento-portal-arlo--hubspot)
7. [Casos Especiais e Exceções](#casos-especiais-e-exceções)

---

## 🎯 COMO USAR ESTE GUIA

### Processo de 3 Passos:

**1. IDENTIFICAR LOCALIZAÇÃO**
- Analisar todos os ZIPs no census
- Determinar localização predominante
- Verificar se há múltiplas localizações significativas

**2. CONSULTAR ÁRVORE DE DECISÃO**
- Seguir a árvore de decisão por estado/região
- Identificar se área tem rede local disponível
- Verificar casos especiais (SSPINS, Q4, etc.)

**3. CONFIRMAR SELEÇÕES**
- Verificar opção correta no Portal Arlo
- Confirmar nomes exatos para HubSpot Primary/Secondary
- Documentar justificativa se houver múltiplas opções

---

## 🌳 ÁRVORE DE DECISÃO RÁPIDA

```
┌─ ANALISAR ZIP DO CENSUS
│
├─ MISSOURI? ────────────────────┐
│  ├─ Kansas City MSA ──────► Centrus + Healthlink
│  ├─ St. Louis area ──────► SSM + Healthlink
│  ├─ Jefferson City ─────► SSM + Healthlink
│  ├─ Cape/Poplar Bluff ──► St. Francis + Healthlink
│  ├─ Central MO ─────────► Mercy + Healthlink ou MO Coop (H2B)
│  ├─ Rolla ──────────────► Phelps Hospital (D2E) + Healthlink
│  ├─ Sikeston ───────────► Missouri Delta (D2E) + Healthlink
│  └─ Sem local específico ► Healthlink OA III (standard)
│
├─ KANSAS? ──────────────────────┐
│  └─ TODO O ESTADO ───────► Centrus + Healthlink ($0 Local)
│
├─ ARKANSAS/TENNESSEE/MS? ───────┐
│  └─ NE AR/West TN/MS ────► Baptist Memorial + Healthlink
│
├─ GEORGIA? ─────────────────────┐
│  ├─ Atlanta Metro [Q4] ──► DUPLA: Cigna PPO + Health Partners w/FH
│  ├─ NE Georgia [Q4] ─────► Health Partners + First Health
│  └─ Outras áreas ────────► Cigna PPO (verificar caso a caso)
│
├─ OHIO? ────────────────────────┐
│  ├─ Cincinnati ──────────► H2B Cincinnati + RBP
│  └─ North of Cincinnati ─► H2B Ohio + RBP
│
├─ KENTUCKY? ────────────────────┐
│  └─ Cincinnati area ──────► H2B Kentucky + [confirmar secondary]
│
├─ IDAHO? ───────────────────────┐
│  └─ Idaho Falls MSA ──────► H2B Idaho + First Choice Health
│
├─ OREGON? ──────────────────────┐
│  └─ Salem MSA ────────────► H2B Oregon + First Choice Health
│
├─ MICHIGAN? ────────────────────┐
│  └─ [região específica] ──► H2B Michigan + RBP
│
├─ SOUTH GEORGIA? ───────────────┐
│  └─ Coffee/Irwin Counties ► H2B South Georgia + RBP
│
├─ WY, WA, ID, OR, AK, MT, ─────┐
│  ND, SD, CO, NE? (<10 enrolled)
│  └─ Grupo < 10 enrolled ──► First Choice Health Network
│
└─ OUTRAS LOCALIZAÇÕES ──────────┐
   └─ Default nacional ───────► Cigna PPO
```

---

## 🌎 REDES STANDARD (NACIONAIS)

### 1. Cigna PPO
**Descrição**: Default National PPO  
**Quando usar**: Maioria dos casos fora de áreas de rede direta  
**Casos especiais**: SSPINS (Sterling Seacrest) usar Cigna PPO por padrão

**Portal Arlo**: "Level Health - Cigna"  
**HubSpot Primary**: "Cigna PPO"  
**HubSpot Secondary**: "N/A"

---

### 2. Healthlink OA III
**Descrição**: Regional PPO  
**Cobertura**: Missouri, Illinois, NE Arkansas, West TN  
**Quando usar**: Missouri sem rede local disponível

**Portal Arlo**: "Level Health - Healthlink"  
**HubSpot Primary**: "HealthLink OA III"  
**HubSpot Secondary**: "N/A"

---

### 3. EHN (Employer's Health Network)
**Descrição**: Rede EPO específica  
**Cobertura**: Ver detalhes na Seção 8 - Rede EHN Detalhada  
**Estados**: AZ, CO, DE, MD, FL, GA, IL, IN, KS, NC, TX, SC

**Portal Arlo**: "Level-Health - EHN EPO"  
**HubSpot Primary**: "Employer's Health Network"  
**HubSpot Secondary**: "N/A"

**⚠️ ATENÇÃO**: EHN é uma rede complexa com hospitais específicos em cada região. Consultar tab EHN para lista completa de hospitais por cidade.

---

### 4. First Choice Health Network
**Descrição**: Regional PPO para grupos pequenos  
**Cobertura**: WY, WA, ID, OR, AK, MT, ND, SD, CO, NE  
**Quando usar**: APENAS para grupos com **menos de 10 enrolled** nestas regiões

**Portal Arlo**: "Level Health - First Choice PPO"  
**HubSpot Primary**: "First Choice Health Network"  
**HubSpot Secondary**: "N/A"

---

## 🏥 REDES LOCAL/DIRECT POR ESTADO

### MISSOURI - Mapa de Referência

**Link do Mapa**: https://www.google.com/maps/d/edit?mid=1dkJSHwp2Z9n8UQPgFDcTPbbgrr1EcRs&usp=sharing

#### 1. Kansas City MSA
**Primary Network**: Centrus Network  
**Secondary Network**: Healthlink OA III (MO) / ProviDRs Care Network (KS)  
**Nota**: Ambas incluem Freedom Network Select

**Portal Arlo**: "$0 Local Contract"  
**HubSpot Primary**: "Centrus Network"  
**HubSpot Secondary**: "Healthlink OA III"

**Região Atendida**: Kansas City MSA, Cape Girardeau/Poplar Bluff, MO  
**Brokers Comuns**: Legacy Brokers, Coalter Insurance, Arnold Insurance, Sonus Benefits

**⚠️ REGRA ESPECIAL KANSAS**: Para QUALQUER empresa no Kansas (KS), mesmo fora da região de Kansas City, SEMPRE usar "$0 Local Contract" com Centrus + Healthlink

**[Q4 2025]**: Sem mudanças

---

#### 2. St. Louis Area / Jefferson City
**Primary Network**: SSM Health  
**Secondary Network**: Healthlink OA III

**Portal Arlo**: "$0 Local Contract"  
**HubSpot Primary**: "SSM Health"  
**HubSpot Secondary**: "Healthlink OA III"

**Região Atendida**: Jefferson City, MO / St. Louis area

**[Q4 2025] Jefferson City**: SSM > Mercy (exceção à regra geral)  
**[Q4 2025] St. Louis**: Sem mudanças

---

#### 3. Southeast Missouri - Cape Girardeau / Poplar Bluff
**Primary Network**: St. Francis Medical Centers  
**Secondary Network**: Healthlink OA III

**Portal Arlo**: "$0 Local Contract"  
**HubSpot Primary**: "St. Francis Medical Centers"  
**HubSpot Secondary**: "Healthlink OA III"

**Região Atendida**: Cape Girardeau região, Southeast Missouri  
**Brokers Comuns**: Coalter Insurance, Arnold Insurance, Sonus Benefits

**[Q4 2025]**: St. Francis > Mercy (prioridade Q4)

---

#### 4. Central Missouri (MID MO)
**Primary Network**: Mercy Health  
**Secondary Network**: Healthlink OA III

**Portal Arlo**: "$0 Local Contract"  
**HubSpot Primary**: "Mercy Health"  
**HubSpot Secondary**: "Healthlink OA III"

**Região Atendida**: Missouri, Northwest AR, Oklahoma City, OK

**[Q4 2025]**: Mercy > SSM em MAIORIA do Central Missouri (EXCETO Jefferson City)

**ALTERNATIVA - Health Cooperative of MO (H2B)**:
- **Portal Arlo**: "$0 Local Contract"
- **HubSpot Primary**: "Missouri Health Co-Op (H2B)"
- **HubSpot Secondary**: "Healthlink OA III"
- **Região**: MID MO
- **Brokers Comuns**: TIG
- **⚠️ EXCEÇÃO H2B**: Sempre adicionar Radion/Great American independente do tamanho

---

#### 5. Rolla, MO - Phelps Hospital (D2E)
**Primary Network**: Phelps Hospital  
**Secondary Network**: Healthlink OA III

**Portal Arlo**: [Aguardando confirmação]  
**HubSpot Primary**: "D2E"  
**HubSpot Secondary**: "Healthlink OA III"

**Região Atendida**: Rolla, MO  
**Brokers Comuns**: Mitchell Insurance

---

#### 6. Sikeston, MO - Missouri Delta (D2E)
**Primary Network**: Missouri Delta  
**Secondary Network**: Healthlink OA III

**Portal Arlo**: [Aguardando confirmação]  
**HubSpot Primary**: "D2E"  
**HubSpot Secondary**: "Healthlink OA III"

**Região Atendida**: Sikeston, MO  
**Brokers Comuns**: Mitchell Insurance

---

### KANSAS

#### TODO O ESTADO DO KANSAS
**Primary Network**: Centrus Network  
**Secondary Network**: Healthlink OA III (para MO) / ProviDRs Care Network (para KS)

**Portal Arlo**: "$0 Local Contract"  
**HubSpot Primary**: "Centrus Network"  
**HubSpot Secondary**: "Healthlink OA III"

**⚠️ REGRA CRÍTICA**: Para QUALQUER empresa no Kansas (KS), independente da região, SEMPRE usar "$0 Local Contract" com Centrus + Healthlink

---

### ARKANSAS / TENNESSEE / MISSISSIPPI

#### NE Arkansas / West TN / MS
**Primary Network**: Baptist Memorial Healthcare  
**Secondary Network**: Healthlink OA III

**Portal Arlo**: "$0 Local Contract"  
**HubSpot Primary**: "Baptist Memorial Health"  
**HubSpot Secondary**: "Healthlink OA III"

**Região Atendida**: NE Arkansas, West TN, MS  
**Localidades Específicas**: Jonesboro AR, Memphis TN

---

### GEORGIA

#### Atlanta Metro
**Primary Network**: 
- **[Q4 2025]**: DUPLA SUBMISSÃO OBRIGATÓRIA
  1. Level Health - Cigna PPO
  2. Health Partners Network + First Health
- **[PERMANENTE]**: Health Partners Network + First Health

**[Q4 2025] Portal Arlo**: 
- Submissão 1: "Level Health - Cigna"
- Submissão 2: "GA Health Partners w FH Wrap"

**[Q4 2025] HubSpot**:
- Submissão Cigna → Primary: "Cigna PPO" / Secondary: "N/A"
- Submissão Health Partners → Primary: "Northeast Georgia Health Partners" / Secondary: "First Health"

**[PERMANENTE] Portal Arlo**: "GA Health Partners w FH Wrap"  
**[PERMANENTE] HubSpot Primary**: "Northeast Georgia Health Partners"  
**[PERMANENTE] HubSpot Secondary**: "First Health"

**Brokers Comuns**: TWS, Sterling Seacrest

**⚠️ NOTA SSPINS**: Para MAIORIA dos casos SSPINS (Sterling Seacrest), usar Cigna PPO por padrão. Durante Q4, para Atlanta, fazer dupla submissão.

---

#### Northeast Georgia
**Primary Network**: Health Partners Network  
**Secondary Network**: First Health

**[Q4 2025] Portal Arlo**: "GA Health Partners w FH Wrap"  
**[Q4 2025] HubSpot Primary**: "Northeast Georgia Health Partners"  
**[Q4 2025] HubSpot Secondary**: "First Health"

**⚠️ [Q4 2025]**: APENAS Health Partners w/FH. NÃO usar $0 Local Contract durante Q4.

**[PERMANENTE] Portal Arlo**: "$0 Local Contract"  
**[PERMANENTE] HubSpot Primary**: "Northeast Georgia Health Partners"  
**[PERMANENTE] HubSpot Secondary**: "First Health"

**Brokers Comuns**: TWS, Sterling Seacrest

---

### OHIO

#### Cincinnati
**Primary Network**: H2B Cincinnati  
**Secondary Network**: RBP

**Portal Arlo**: "$0 Local Contract"  
**HubSpot Primary**: "H2B Cincinnati"  
**HubSpot Secondary**: "RBP"

**Região Atendida**: Cincinnati, Northern Kentucky  
**Brokers Comuns**: H2B

**⚠️ EXCEÇÃO H2B**: Sempre adicionar Radion/Great American independente do tamanho

---

#### North of Cincinnati
**Primary Network**: H2B Ohio  
**Secondary Network**: RBP

**Portal Arlo**: "$0 Local Contract"  
**HubSpot Primary**: "H2B Ohio"  
**HubSpot Secondary**: "RBP"

**Região Atendida**: North of Cincinnati  
**Brokers Comuns**: H2B

**⚠️ EXCEÇÃO H2B**: Sempre adicionar Radion/Great American independente do tamanho

---

### KENTUCKY

#### H2B Kentucky
**Primary Network**: H2B Kentucky  
**Secondary Network**: [Aguardando confirmação]

**Portal Arlo**: "$0 Local Contract"  
**HubSpot Primary**: "H2B Kentucky"  
**HubSpot Secondary**: [Confirmar]

**⚠️ EXCEÇÃO H2B**: Sempre adicionar Radion/Great American independente do tamanho

---

### IDAHO

#### Idaho Falls MSA
**Primary Network**: H2B Idaho  
**Secondary Network**: First Choice Health Network

**Portal Arlo**: "Level Health - H2B Idaho"  
**HubSpot Primary**: "H2B Idaho"  
**HubSpot Secondary**: "First Choice Health Network"

**Região Atendida**: Idaho Falls MSA  
**Brokers Comuns**: Baker Benefits

**⚠️ EXCEÇÃO H2B**: Sempre adicionar Radion/Great American independente do tamanho

---

### OREGON ⭐ NOVA

#### Salem, OR MSA
**Primary Network**: H2B Oregon  
**Secondary Network**: First Choice Health Network

**Portal Arlo**: "$0 Local Contract"  
**HubSpot Primary**: "H2B Oregon"  
**HubSpot Secondary**: "First Choice Health Network"

**Região Atendida**: Salem, OR MSA

**⚠️ EXCEÇÃO H2B**: Sempre adicionar Radion/Great American independente do tamanho

---

### MICHIGAN ⭐ NOVA

#### H2B Michigan
**Primary Network**: H2B Michigan  
**Secondary Network**: RBP

**Portal Arlo**: "$0 Local Contract"  
**HubSpot Primary**: "H2B Michigan"  
**HubSpot Secondary**: "RBP"

**Região Atendida**: [Confirmar localidades específicas]

**⚠️ EXCEÇÃO H2B**: Sempre adicionar Radion/Great American independente do tamanho

---

### SOUTH GEORGIA

#### Coffee County / Irwin County
**Primary Network**: H2B South Georgia  
**Secondary Network**: RBP

**Portal Arlo**: "$0 Local Contract"  
**HubSpot Primary**: "H2B South Georgia"  
**HubSpot Secondary**: "RBP"

**Região Atendida**: Coffee County, Irwin County  
**Brokers Comuns**: H2B

**⚠️ EXCEÇÃO H2B**: Sempre adicionar Radion/Great American independente do tamanho

---

## 📍 TABELA DE REFERÊNCIA RÁPIDA POR LOCALIZAÇÃO

### Missouri

| Localização | Primary Network | Secondary Network | Portal Arlo | Q4 Prioridade |
|---|---|---|---|---|
| Kansas City | Centrus | Healthlink OA III | $0 Local | Sem mudanças |
| St. Louis | SSM | Healthlink OA III | $0 Local | Sem mudanças |
| Jefferson City | SSM | Healthlink OA III | $0 Local | SSM > Mercy |
| Cape Girardeau/Poplar Bluff | St. Francis | Healthlink OA III | $0 Local | St. Francis > Mercy |
| Central MO (exceto Jeff City) | Mercy | Healthlink OA III | $0 Local | Mercy > SSM |
| Central MO (alternativa) | MO Coop (H2B) | Healthlink OA III | $0 Local | Alternativa |
| Rolla | Phelps (D2E) | Healthlink OA III | [Confirmar] | Nova opção |
| Sikeston | Missouri Delta (D2E) | Healthlink OA III | [Confirmar] | Nova opção |
| Oklahoma City, OK | Mercy | Healthlink OA III | $0 Local | Sem mudanças |
| Sem local específico | Healthlink OA III | N/A | Level Health - Healthlink | Standard |

---

### Kansas

| Localização | Primary Network | Secondary Network | Portal Arlo | Nota |
|---|---|---|---|---|
| TODO O ESTADO | Centrus | Healthlink OA III | $0 Local | Regra especial |

---

### Arkansas / Tennessee / Mississippi

| Localização | Primary Network | Secondary Network | Portal Arlo | Nota |
|---|---|---|---|---|
| NE Arkansas | Baptist Memorial | Healthlink OA III | $0 Local | Jonesboro AR |
| West Tennessee | Baptist Memorial | Healthlink OA III | $0 Local | Memphis TN |
| Mississippi | Baptist Memorial | Healthlink OA III | $0 Local | West TN/MS |

---

### Georgia

| Localização | Primary Network | Secondary Network | Portal Arlo | Q4 2025 |
|---|---|---|---|---|
| Atlanta Metro | Cigna PPO + Health Partners | N/A + First Health | Cigna + GA HP w FH | DUPLA submissão |
| Northeast Georgia | Health Partners | First Health | GA HP w FH Wrap | Apenas HP Q4 |

---

### Ohio / Kentucky

| Localização | Primary Network | Secondary Network | Portal Arlo | H2B Exception |
|---|---|---|---|---|
| Cincinnati | H2B Cincinnati | RBP | $0 Local | Sim |
| North of Cincinnati | H2B Ohio | RBP | $0 Local | Sim |
| Kentucky (Cincinnati area) | H2B Kentucky | [Confirmar] | $0 Local | Sim |

---

### Idaho / Oregon / Michigan

| Localização | Primary Network | Secondary Network | Portal Arlo | H2B Exception |
|---|---|---|---|---|
| Idaho Falls MSA | H2B Idaho | First Choice | Level Health - H2B Idaho | Sim |
| Salem, OR MSA | H2B Oregon | First Choice | $0 Local | Sim ⭐ |
| Michigan | H2B Michigan | RBP | $0 Local | Sim ⭐ |

---

### South Georgia

| Localização | Primary Network | Secondary Network | Portal Arlo | H2B Exception |
|---|---|---|---|---|
| Coffee/Irwin Counties | H2B South Georgia | RBP | $0 Local | Sim |

---

### Estados do Noroeste (<10 enrolled)

| Estados | Primary Network | Secondary Network | Portal Arlo | Condição |
|---|---|---|---|---|
| WY, WA, ID, OR, AK, MT, ND, SD, CO, NE | First Choice Health | N/A | Level Health - First Choice PPO | < 10 enrolled |

---

## 🔄 MAPEAMENTO PORTAL ARLO → HUBSPOT

### Redes Standard

| Portal Arlo | HubSpot Primary | HubSpot Secondary |
|---|---|---|
| Level Health - Cigna | Cigna PPO | N/A |
| Level Health - Healthlink | HealthLink OA III | N/A |
| Level-Health - EHN EPO | Employer's Health Network | N/A |
| Level Health - First Choice PPO | First Choice Health Network | N/A |

---

### Redes Local/Direct - $0 Local Contract

**⚠️ ATENÇÃO**: A opção "$0 Local Contract" no Portal Arlo pode representar DIFERENTES redes dependendo da região. Você deve determinar qual rede específica com base na localização do grupo.

| Região | Portal Arlo | HubSpot Primary | HubSpot Secondary |
|---|---|---|---|
| Kansas City / Kansas | $0 Local Contract | Centrus Network | Healthlink OA III |
| St. Louis / Jefferson City | $0 Local Contract | SSM Health | Healthlink OA III |
| Cape Girardeau/Poplar Bluff | $0 Local Contract | St. Francis Medical Centers | Healthlink OA III |
| Central Missouri | $0 Local Contract | Mercy Health | Healthlink OA III |
| Central Missouri (alt) | $0 Local Contract | Missouri Health Co-Op (H2B) | Healthlink OA III |
| NE AR / West TN / MS | $0 Local Contract | Baptist Memorial Health | Healthlink OA III |
| Cincinnati | $0 Local Contract | H2B Cincinnati | RBP |
| North of Cincinnati | $0 Local Contract | H2B Ohio | RBP |
| Kentucky | $0 Local Contract | H2B Kentucky | [Confirmar] |
| South Georgia | $0 Local Contract | H2B South Georgia | RBP |
| Salem, OR MSA | $0 Local Contract | H2B Oregon | First Choice Health Network |
| Michigan | $0 Local Contract | H2B Michigan | RBP |

---

### Redes Específicas com Opção Própria

| Portal Arlo | HubSpot Primary | HubSpot Secondary |
|---|---|---|
| Level Health - H2B Idaho | H2B Idaho | First Choice Health Network |
| GA Health Partners w FH Wrap | Northeast Georgia Health Partners | First Health |

---

### D2E (Rolla e Sikeston)

| Região | Portal Arlo | HubSpot Primary | HubSpot Secondary |
|---|---|---|---|
| Rolla, MO | [Aguardando confirmação] | D2E | Healthlink OA III |
| Sikeston, MO | [Aguardando confirmação] | D2E | Healthlink OA III |

---

## ⚠️ CASOS ESPECIAIS E EXCEÇÕES

### 1. Exceção H2B Networks (SEMPRE Radion/Great American)

**Lista Completa de Redes H2B (ATUALIZADA)**:
- Health Cooperative of MO (Missouri)
- H2B Cincinnati (Ohio)
- H2B Idaho
- H2B Ohio
- H2B Kentucky
- H2B South Georgia
- **H2B Oregon** (Salem, OR MSA) ⭐ NOVA
- **H2B Michigan** ⭐ NOVA

**Regra**: SEMPRE adicionar Radion/Great American independente do tamanho do grupo quando usar qualquer rede H2B.

---

### 2. SSPINS (Sterling Seacrest)

**Regra Geral [PERMANENTE]**: Para MAIORIA dos casos SSPINS (Sterling Seacrest), usar **Cigna PPO** por padrão, NÃO usar Health Partners + First Health automaticamente.

**[Q4 2025] Exceção**: 
- Atlanta: DUPLA submissão (Cigna + Health Partners)
- NE Georgia: Usar Health Partners w/FH mesmo se SSPINS

---

### 3. Kansas - Regra Especial TODO O ESTADO

**REGRA CRÍTICA**: Para QUALQUER empresa no Kansas (KS), independente da região:
- SEMPRE usar "$0 Local Contract"
- Primary: Centrus Network
- Secondary: Healthlink OA III

Isto se aplica a TODO o estado do Kansas, não apenas Kansas City.

---

### 4. Regras Q4 2025 (Outubro-Dezembro)

#### Atlanta Metro:
- DUPLA submissão obrigatória:
  1. Level Health - Cigna PPO
  2. GA Health Partners w FH Wrap
- NÃO usar $0 Local durante Q4

#### Northeast Georgia:
- Usar APENAS Health Partners w/FH Wrap
- NÃO usar $0 Local Contract durante Q4
- Sobrepõe regra SSPINS durante Q4

#### Missouri - Prioridades Q4:
- Cape Girardeau/Poplar Bluff: St. Francis > Mercy
- Central MO (exceto Jefferson City): Mercy > SSM
- Jefferson City: SSM > Mercy (exceção à regra geral)
- Consultar mapa: https://www.google.com/maps/d/edit?mid=1dkJSHwp2Z9n8UQPgFDcTPbbgrr1EcRs&usp=sharing

---

### 5. First Choice Health Network

**APENAS para grupos com < 10 enrolled** nos seguintes estados:
- WY, WA, ID, OR, AK, MT, ND, SD, CO, NE

**Se grupo ≥ 10 enrolled** nestas regiões: usar Cigna PPO (standard)

---

### 6. D2E (Direct to Employer)

**Duas redes usam designação D2E no HubSpot**:
- Phelps Hospital (Rolla, MO)
- Missouri Delta (Sikeston, MO)

**Ambas têm**:
- HubSpot Primary: "D2E"
- HubSpot Secondary: "Healthlink OA III"
- Portal Arlo: [Aguardando confirmação]

---

### 7. Restrições Arlo (Setembro 2025)

**Estados INDISPONÍVEIS no Arlo**:
- Washington (WA)
- Oklahoma (OK)
- District of Columbia (DC)
- New York (NY)

**Ação**: Se grupo estiver nestes estados, NÃO submeter para Arlo. Proceder apenas com outras MGUs aplicáveis.

---

## 🔍 PROCESSO DE VERIFICAÇÃO ANTES DE SUBMETER

### Checklist de Seleção de Rede:

- [ ] **1. Analisar TODOS os ZIPs no census**
- [ ] **2. Determinar localização predominante**
- [ ] **3. Verificar se há área de rede local disponível**
- [ ] **4. Consultar árvore de decisão por estado**
- [ ] **5. Verificar casos especiais**:
  - [ ] É SSPINS (Sterling Seacrest)? → Cigna PPO padrão (exceto Q4 Atlanta/NE GA)
  - [ ] É rede H2B? → Adicionar Radion/Great American
  - [ ] É Kansas? → SEMPRE $0 Local (todo o estado)
  - [ ] É Missouri? → Consultar mapa e prioridades Q4
  - [ ] É Atlanta? [Q4] → DUPLA submissão
  - [ ] É NE Georgia? [Q4] → Health Partners w/FH
  - [ ] É grupo < 10 em WY/WA/ID/OR/AK/MT/ND/SD/CO/NE? → First Choice
- [ ] **6. Confirmar opção correta no Portal Arlo**
- [ ] **7. Confirmar nomes exatos para HubSpot Primary/Secondary**
- [ ] **8. Documentar justificativa se múltiplas localizações**

---

## 📊 REDE EHN DETALHADA

### Employer's Health Network (EHN) - Por Estado e Região

**⚠️ ATENÇÃO**: EHN é uma rede EPO com hospitais específicos em cada região. Sempre verificar se a localização do grupo está próxima aos hospitais listados.

---

#### ARIZONA

**Phoenix:**
- Abrazo West Hospital
- Abrazo Central Hospital
- Abrazo Arrowhead Campus
- Abrazo Arizona Heart Hospital
- Abrazo Surprise Hospital
- Abrazo Scottsdale Campus
- Abrazo Buckeye Emergency Center
- Abrazo Mesa Hospital
- Abrazo Buckeye Peoria Center
- Chandler Regional Medical Center
- Cogent Healthcare of Arizona
- Dignity Health Arizona General Hospital (AGH Laveen)
- Dignity Health Arizona General Hospital (AGH Mesa)
- Dignity Health Cancer Institute at St Joseph's Hospital
- Mercy Gilbert Medical Center
- Phoenix Children's Hospital
- Phoenix Children's at Mercy Gilbert
- St. Joseph's Hospital and Medical Center
- St. Joseph's Westgate Medical Center
- Valleywise Health Medical Center - all locations

**Tucson/Nogales:**
- Carondelet St. Mary's Hospital
- Carondelet St. Joseph's Hospital
- Carondelet Holy Cross Hospital
- Carondelet Marana Micro Hospital
- Carondelet Foothills Surgery Center

---

#### COLORADO

**Canon City:**
- St Thomas More - Centura

**Pueblo:**
- St Mary Corwin Hospital - Centura

**Frisco:**
- St Anthony Summit Hospital - Centura

**Summit:**
- St Anthony North Hospital - Centura

**Lakewood:**
- St Anthony Hospital - Centura
- OrthoColorado Hospital - Centura

**Denver:**
- Porter Adventist Hospital - Centura

**Durango:**
- Mercy Hospital - Centura

**Longmont:**
- Longmont Hospital - Centura

**Littleton:**
- Littleton Adventist Hospital - Centura

**Castle Rock:**
- Castle Rock Adventist Hospital - Centura

**Louisville:**
- Avista Adventist Hospital - Centura

**Parker:**
- Parker Adventist Hospital - Centura

**Ulysses, KS:**
- Bob Wilson Hospital - Centura

---

#### DELAWARE / MARYLAND

**Lower DE, Maryland Eastern Shore:**
- DE - Beebe
- DE - Nanticoke
- DE - DuPont Children's
- MD Peninsula General/McCready
- MD - Atlantic General
- MD - Univ of Maryland

---

#### FLORIDA

**Jacksonville:**
- UF Health North Campus
- UF Health Jacksonville
- UF Health Gainesville
- Emerson Plaza
- Wolfson Children's Hospital
- UF Health Shands Hospital
- UF Health Shands Children's Hospital
- UF Health Shands Cancer Hospital
- UF Health Heart and Vascular Hospital
- UF Health Neuromedicine Hospital
- UF Health Rehab Hospital
- UF Health Psychiatric Hospital
- Nemours
- Care Spot Urgent Care Clinics

**Orlando:**
- Orlando Regional Medical Center
- Halifax Health
- Parrish Medical Center
- UF Health Leesburg
- Orlando Health Arnold Palmer Hospital for Children
- Orlando Health Winnie Palmer Hospital for Women
- Orlando Health - Health Central Hospital

---

#### GEORGIA

**Savannah:**
- St Josephs Hospital
- Candler Hospital
- Bluffton Campus
- Pooler Campus

---

#### ILLINOIS

**Mattoon:**
- Sara Bush Lincoln Health System

---

#### INDIANA

**Carmel:**
- Franciscan Health Carmel

**Crawfordsville:**
- Franciscan Health Crawfordsville

**Crown Point:**
- Franciscan Health Crown Point

**Dyer:**
- Franciscan Health Dyer

**Hammond:**
- Franciscan Health Hammond

**Indianapolis:**
- Franciscan Health Indianapolis

**Lafayette:**
- Franciscan Health Lafayette

**Michigan City:**
- Franciscan Health Michigan City

**Mooresville:**
- Franciscan Health Mooresville

**Munster:**
- Franciscan Health Munster

**Olympia Fields:**
- Franciscan Health Olympia Fields

**Rensselaer:**
- Franciscan Health Rensselaer

---

#### KANSAS

**Kansas City:**
- University of Kansas Medical Center
- University of Kansas Hospital
- University of Kansas Health System Marillac Campus
- University of Kansas Health System Strawberry Hill Campus
- Miami County Medical Center
- Olathe Medical Center
- Children's Mercy Kansas City
- Meritas Health North Kansas City Hospital
- Advent Health - Shawnee Mission
- Advent Health - Lenexa
- Advent Health - Overland Park
- AdventHealth Centra Care Olathe

**Topeka:**
- University of Kansas Health System - St Francis

---

#### NORTH CAROLINA

**Charlotte:**
- Atrium
- Piedmont - Rock Hill, SC
- MUSC Lancaster - Lancaster, SC

---

#### TEXAS

**Austin:**
- Seton Medical Center
- Dell Seton Medical Center
- Dell Children's
- Seton Northwest
- Seton Southwest
- Seton Medical Center Hays
- Seton Medical Center Williamson
- Seton Medical Center Harker Heights
- Cedar Park Regional Medical Center

**Rio Grande:**
- Valley Baptist Medical Center - Harlingen
- Valley Baptist Medical Center - Brownsville
- Valley Baptist Medical Center - Weslaco

**Dallas Fort Worth:**
- Baylor Scott & White All Saints Medical Center - Fort Worth
- Baylor Scott & White Heart and Vascular Hospital - Dallas
- Baylor Scott & White Medical Center - Centennial
- Baylor Scott & White Medical Center - Grapevine
- Baylor Scott & White Medical Center - Irving
- Baylor Scott & White Medical Center - Lake Pointe
- Baylor Scott & White Medical Center - McKinney
- Baylor Scott & White Medical Center - Plano
- Baylor Scott & White Medical Center at Waxahachie
- Baylor Scott & White The Heart Hospital - Denton
- Baylor Scott & White The Heart Hospital - Plano
- Baylor University Medical Center
- Baylor Scott & White McLane Children's Medical Center
- Baylor Scott & White Medical Center - Austin
- Baylor Scott & White Medical Center - Brenham
- Baylor Scott & White Medical Center - Buda
- Baylor Scott & White Medical Center - College Station
- Baylor Scott & White Medical Center - Hillcrest
- Baylor Scott & White Medical Center - Lakeway
- Baylor Scott & White Medical Center - Llano
- Baylor Scott & White Medical Center - Marble Falls
- Baylor Scott & White Medical Center - Pflugerville
- Baylor Scott & White Medical Center - Round Rock
- Baylor Scott & White Medical Center - Taylor
- Baylor Scott & White Medical Center - Temple
- Baylor Orthopedic and Spine Hospital at Arlington
- Baylor Scott & White Medical Center - Frisco
- Baylor Scott & White Medical Center - Sunnyvale
- Baylor Scott & White Medical Center - Trophy Club
- Baylor Scott & White Medical Center - Uptown
- Baylor Scott & White Surgical Hospital - Fort Worth
- Baylor Scott & White Surgical Hospital at Sherman
- Baylor Scott & White Texas Spine & Joint Hospital
- Baylor Surgical Hospital at Las Colinas
- North Central Surgical Center
- Baylor Scott & White Emergency Hospital
- Baylor Scott & White Emergency Hospital Burleson
- Baylor Scott & White Emergency Hospital Colleyville
- Baylor Scott & White Emergency Hospital Grand Prairie
- Baylor Scott & White Emergency Hospital Keller
- Baylor Scott & White Emergency Hospital Mansfield
- Baylor Scott & White Emergency Hospital Murphy
- Baylor Scott & White Emergency Hospital Rockwall

**El Paso:**
- The Hospitals of Providence Transmountain Campus
- The Hospitals of Providence Memorial Campus
- The Hospitals of Providence Sierra Campus
- The Hospitals of Providence East Campus

**Houston:**
- Memorial Hermann Southeast Hospital
- Memorial Hermann Cypress Hospital
- Memorial Hermann Southwest Hospital
- Memorial Hermann Heart & Vascular
- Memorial Hermann Hospital
- Children's Memorial Hermann Hospital
- Memorial Hermann Memorial City Medical Center
- Longpoint Medical Center
- Memorial Hermann Northeast Hospital
- Memorial Hermann Katy Hospital
- Memorial Hermann Specialty Hospital
- Memorial Hermann Pearland Hospital
- Memorial Hermann - The Woodlands Hospital
- Memorial Hermann Sugarland Hospital

**San Antonio:**
- St Luke's Baptist Hospital
- Baptist Medical Center
- Mission Trail Baptist Hospital
- Northeast Baptist Hospital
- North Central Baptist Hospital & Baptist Children's Hospital
- Resolute Health Hospital
- Baptist Neighborhood Hospital- Hausman
- Baptist Neighborhood Hospital– Shavano Park
- Baptist Neighborhood Hospital Zarzamora
- Baptist Neighborhood Hospital Kelly
- Baptist Neighborhood Hospital– Westover Hills
- Baptist Neighborhood Hospital Thousand Oaks
- Baptist Neighborhood Hospital Overlook
- Baptist Neighborhood Hospital Schertz

---

#### SOUTH CAROLINA

**Charleston:**
- Medical University of South Carolina
- Chester Medical Center
- Florence Medical Center
- Lancaster Medical Center
- Marion Medical Center
- University Medical Center

**Greenville/Spartanburg:**
- Spartanburg Reg Health System
- Spartanburg Medical Center
- Spartanburg Medical Center - Mary Black Campus
- Cherokee Medical Center
- Pelham Medical Center
- Union Medical Center

---

## 📈 H2B NETWORKS - DETALHAMENTO COMPLETO

### H2B Idaho

**Hospitais Incluídos**:
- St Luke's Regional Medical Center
- St Luke's McCall Hospital
- St Luke's Nampa Medical Center
- St Luke's Magic Valley Medical Center
- St Luke's Jerome Hospital
- St Luke's Wood River Medical Center
- St Luke's Children's Hospital
- St Luke's Elmore Medical Center
- St. Luke's Rehabilitation Hospital
- North Canyon Medical Center

**Contratos**:
- St Luke's Regional: Inpatient 2.3x, Outpatient 2.3x, Professional 2.0x
- North Canyon: Outpatient 1.8x, Professional 1.6x

**Segundo Grupo de Hospitais**:
- Bingham Memorial Healthcare: Inpatient 1.5x, Outpatient 1.65x, Professional 1.85x
- Grove Creek ASC: Outpatient 1.65x, Professional 1.85x
- Madison Memorial Hospital: Inpatient 1.6x, Outpatient 1.7x, Professional 1.6x
- Mountain View Hospital: Outpatient 2.0x, Professional 1.7x
- Idaho Community Hospital: Inpatient 2.0x, Outpatient 2.0x, Professional 1.7x

---

### H2B Oregon

**Hospitais Incluídos**:
- Legacy Emanuel Hospital & Health Center
- Legacy Good Samaritan Hospital & Medical Center
- Legacy Meridian Park Hospital
- Legacy Mount Hood Medical Center
- Legacy Salmon Creek Hospital
- Silverton Health

**Contratos**:
- Inpatient 2.3x
- Outpatient 3.0x
- Professional 1.7x

---

### H2B Missouri (Health Cooperative of MO)

**Hospitais Incluídos**:
- Boone Hospital Center
- Bothwell Regional Health Center
- Fitzgibbon Hospital
- Pershing Health System
- Scotland County Hospital
- Sullivan County Hospital

**Contratos**:
- Inpatient 1.65x
- Outpatient 1.75x
- Professional 1.4x

---

### H2B Kentucky

**Hospitais Incluídos**:
- St Elizabeth Edgewood
- St Elizabeth Florence
- St Elizabeth Ft. Thomas
- St Elizabeth Grant County
- St Elizabeth Covington
- Mercy Health – Lourdes Hospital

**Contratos**:
- St Elizabeth: Inpatient 2.27x, Outpatient 2.27x, Professional 1.45x
- Mercy Lourdes: Inpatient 1.9x, Outpatient 1.9x, Professional 1.4x

---

### H2B Cincinnati / Ohio

**Hospitais Incluídos**:
- Mercy Health - Anderson Hospital
- Mercy Health - Clermont Hospital
- Mercy Health Fairfield Hospital
- Mercy Health - West Hospital
- The Jewish Hospital
- Mercy Health - Urbana Hospital
- Mercy Health - Springfield Regional Medical Center
- Mercy Health – St. Vincent Medical Center
- Mercy Health – Perrysburg Hospital
- Mercy Health – St. Charles Hospital
- Mercy Health – St. Anne Hospital
- Mercy Health – Willard Hospital
- Mercy Health – Tiffin Hospital
- Mercy Health – Defiance Hospital
- Wilson Health
- Wayne Health

**Contratos**:
- Mercy Health: Inpatient 2.0x, Outpatient 2.0x, Professional 1.4x
- Wilson Health: Inpatient 1.8x, Outpatient 1.8x, Professional 1.4x
- Wayne Health: Inpatient 1.8x, Outpatient 1.8x, Professional 1.4x

---

### H2B Michigan

**Hospitais Incluídos**:
- McKenzie Health

**Contratos**:
- Inpatient 1.15x
- Outpatient 1.6x
- Professional 1.2x

---

### H2B South Georgia

**Hospitais Incluídos**:
- Coffee Regional Medical Center
- Irwin County Hospital

**Contratos**:
- Coffee Regional: Inpatient 2.75x, Outpatient 2.75x, Professional 1.35x
- Irwin County: Inpatient 2.0x, Professional 1.3x

---

### USPI (United Surgical Partners International)

**Descrição**: Rede nacional de ASCs (Ambulatory Surgery Centers)

**Hospitais**: 355 ASCs em todo o país

**Contratos**:
- Outpatient 2.65x

---

## 📝 NOTAS FINAIS E LEMBRETES

### Pontos Críticos:

1. **SEMPRE consultar o mapa de Missouri**: https://www.google.com/maps/d/edit?mid=1dkJSHwp2Z9n8UQPgFDcTPbbgrr1EcRs&usp=sharing

2. **H2B Networks = Exceção MGU**: Qualquer rede H2B sempre adiciona Radion/Great American independente do tamanho

3. **Kansas = TODO o estado $0 Local**: Não apenas Kansas City, mas TODO o estado do Kansas

4. **SSPINS = Cigna PPO padrão**: Exceto durante Q4 para Atlanta (dupla) e NE Georgia (Health Partners)

5. **First Choice = Apenas <10 enrolled**: Em WY, WA, ID, OR, AK, MT, ND, SD, CO, NE

6. **D2E no HubSpot**: Apenas para Phelps Hospital (Rolla) e Missouri Delta (Sikeston)

7. **EHN é EPO**: Verificar lista específica de hospitais por região antes de recomendar

8. **Portal Arlo "$0 Local Contract"**: Pode representar diferentes redes - determinar pela localização

9. **Q4 2025**: Regras temporárias para Atlanta (dupla), NE Georgia (apenas HP), e prioridades Missouri

10. **Restrições Arlo**: WA, OK, DC, NY indisponíveis

---

### Transição Q4 → 2026:

**Durante Q4 2025 (Outubro-Dezembro)**:
- Usar regras Q4 para Atlanta, NE Georgia e prioridades Missouri
- Manter todas as outras regras inalteradas

**A partir de Janeiro 2026**:
- Retornar às regras permanentes
- Atlanta: Apenas Health Partners (não mais dupla)
- NE Georgia: $0 Local Contract (não mais apenas HP)
- Missouri: Prioridades standard (sem prioridades Q4)

---

*Fim do Guia de Seleção de Redes Level Health*  
*Versão: Outubro 2025*  
*Baseado em: Network Options.xlsx + Guia Completo Consolidado*  
*Próxima atualização: Janeiro 2026*
