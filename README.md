# 🚀 EASY SWAP – Ecommerce Solutions

Sistema Web de Gestão de Trocas e Logística Reversa para E-commerce.

---

## Sobre o Projeto

O **EASY SWAP** é uma solução web desenvolvida para simplificar e automatizar o processo de trocas e devoluções em lojas virtuais.

A plataforma permite que o cliente registre solicitações de troca por meio de um formulário acessado via QR Code, enviando informações e fotos do produto.  
Essas solicitações são transformadas em tickets, que podem ser analisados por um atendente em um painel administrativo.

O sistema organiza a logística reversa, reduz retrabalho e melhora a experiência pós-venda no e-commerce.

---

## Objetivo

- Automatizar solicitações de trocas e devoluções  
- Organizar tickets de atendimento  
- Permitir aprovação ou recusa de solicitações  
- Gerar código de postagem automático (simulado)  
- Disponibilizar dashboard com indicadores operacionais  

---

## Tipo de Sistema

Sistema Web Responsivo  

---

## Público-Alvo

- Pequenos e médios e-commerces  
- Lojas virtuais que utilizam plataformas como Shopify  
- Operadores de e-commerce que desejam organizar o pós-venda  
- Marcas digitais que buscam melhorar a experiência do cliente  

---

## Tecnologias Utilizadas

**Frontend:**  
- Next.js

**Backend e Banco de Dados:**  
- Supabase (PostgreSQL)

**Armazenamento de Imagens:**  
- Supabase Storage  

**Gráficos e Indicadores:**  
- Chart.js  

**Deploy:**  
- Vercel  

---

## Fluxo do Sistema

### Cliente

1. Escaneia QR Code ou acessa link
2. Preenche formulário com:
   - Número do pedido
   - Email  
   - CPF
   - Motivo da troca
   - Descrição do problema
   - Upload de até 3 fotos
   - Escolha entre devolução automática ou apenas abertura de ticket
3. Envia solicitação
4. Sistema gera ticket no banco de dados

---

### Atendente

1. Acessa painel administrativo (/admin)
2. Visualiza lista de tickets
3. Analisa informações e imagens
4. Pode:
   - Aprovar
   - Recusar
   - Solicitar mais informações
5. Se aprovado:
   - Sistema gera código de postagem automático (simulado)
   - Status do ticket é atualizado

---

## Dashboard (Indicadores)

- Total de tickets
- Tickets por status
- Tickets por motivo
- Taxa de aprovação
- Volume mensal de solicitações

---

## Estrutura do Projeto


## Modelagem do Banco (Principais Tabelas)

**tickets**
- id
- numero_pedido
- email_cpf
- motivo
- descricao
- status
- codigo_postagem
- data_criacao

**fotos_ticket**
- id
- ticket_id
- url_imagem

**usuarios**
- id
- email
- senha
- tipo (admin)

---

## Deploy

O sistema é publicado na Vercel, conectado ao Supabase.

Fluxo de deploy:

1. Configurar variáveis de ambiente
2. Conectar projeto ao repositório Git
3. Publicar aplicação
4. Gerar QR Code apontando para /troca

---

## Planejamento de Execução

Tempo total estimado: 60 horas

- 20h Documentação
- 35h Desenvolvimento
- 5h Deploy e testes

---

## Diferencial da Solução

- Automatização de trocas para pequenos e médios e-commerces
- Redução de atendimento manual via WhatsApp e e-mail
- Organização da logística reversa
- Dashboard estratégico para tomada de decisão

---

## Status do Projeto

Em desenvolvimento.

---

## Desenvolvido por Elen Vieira

Projeto acadêmico / portfólio com foco em soluções para e-commerce.
