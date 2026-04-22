# Dashboard Operacional VIP — Starian

Painel de gestão de relacionamento e SLAs dos clientes VIP da Starian, 
desenvolvido em HTML puro com Chart.js e PapaParse.

## Acesso

O dashboard está disponível em:
**[link do GitHub Pages aqui]**

---

## Como atualizar os dados

1. Exporte o relatório de tickets do Freshdesk
2. Renomeie o arquivo para **`dados.csv`**
3. Faça upload no repositório substituindo o arquivo anterior
4. Aguarde 2–5 minutos para o dashboard atualizar automaticamente

> Caso prefira, o botão **"Carregar dados.csv"** no dashboard permite 
> fazer upload manual direto no navegador.

---

## Funcionalidades

### Abas

| Aba | Descrição |
|-----|-----------|
| Resumo Executivo | KPIs, evolução mensal, MTTR e inteligência operacional |
| Radar Operacional | Tickets ativos com SLA violado, separados por status |
| Evolutivas & Melhorias | Backlog de produto sem SLA, ordenado por antiguidade |
| Análise de Gargalos | MTTR por grupo, top clientes e plano de ação |
| Insights Executivos | Visão consolidada para reuniões executivas |

### Motor de SLA

Cálculo baseado em **horas úteis reais**:
- Segunda a sexta-feira, das 08h às 18h (**10h/dia**)
- Feriados nacionais brasileiros excluídos automaticamente
- Cálculo de Páscoa, Carnaval e Corpus Christi por ano

| Tipo | Urgente | Alta | Média | Baixa |
|------|---------|------|-------|-------|
| Sistema Inoperante | 10h | — | — | — |
| Erro Relacionado | 40h | 140h | 180h | 300h |
| Erro do Sistema | 30h | 100h | 150h | 250h |
| Problema de Desempenho | 30h | 100h | 150h | 250h |
| Intervenção na Base | 60h | 100h | 150h | 180h |
| Dúvidas e Orientações | 15h | 15h | 15h | 15h |
| Consultoria de Sistema | — | — | 50h | — |
| Ativação API / Connectors | — | — | 50h | — |
| Criação de Base DC | — | — | 30h | — |
| Alterações / Melhorias | Sem SLA | | | |

### Filtros disponíveis

Período · Segmento VIP · Canal · CSM · Tipo · Status · 
Prioridade · Grupo Solucionador · Time de Desenvolvimento · Cliente

---

## Estrutura do repositório

---

## Tecnologias

- [Chart.js](https://www.chartjs.org/) — Gráficos
- [PapaParse](https://www.papaparse.com/) — Leitura de CSV
- [Tailwind CSS](https://tailwindcss.com/) — Estilização
- [chartjs-plugin-datalabels](https://chartjs-plugin-datalabels.netlify.app/) — Labels nos gráficos

---

## Acesso restrito

Este dashboard contém informações confidenciais de clientes VIP.  
Compartilhe o link apenas com pessoas autorizadas da Starian.

---

*Desenvolvido por Vanessa Luz — BackOffice Starian*
