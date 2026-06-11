# controle-financeiro-anual

App web para controle de gastos mensais, parcelas e cálculo de salário líquido.

## Funcionalidades

- Lançamento de gastos por categoria
- Controle de compras parceladas
- Cálculo de salário líquido (Com os Descontos em Folha)
- Sincronização via Supabase
- Modo offline com cache local

## Stack

- HTML/CSS/JS puro (sem framework)
- Supabase (PostgreSQL + REST API)

## Segurança

Este projeto utiliza a `publishable key` do Supabase exposta no frontend. 
Este comportamento é intencional e documentado pela própria plataforma para aplicações
client-side.

A proteção dos dados é feita via **Row Level Security (RLS)** diretamente no
banco de dados, com policies que isolam o acesso por `device_id` via request
header.
