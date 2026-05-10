# Documentação do Agente

## Caso de Uso

### Problema
> Qual problema financeiro seu agente resolve?

Este agente resolve o analfabetismo financeiro e o descontrole orçamentário por meio do diagnóstico patrimonial e do registro sistemático de receitas e despesas

### Solução
> Como o agente resolve esse problema de forma proativa?

O agente realiza o diagnóstico patrimonial e o controle de gastos para combater o descontrole financeiro e garantir um orçamento superavitário
. Promove a estratégia de "pagar-se primeiro", a criação de reservas de segurança e a transformação de sonhos em projetos reais

### Público-Alvo
> Quem vai usar esse agente?

Este agente é voltado para qualquer **indivíduo ou família** que precise organizar suas finanças, incluindo leigos, estudantes universitários e profissionais de diversas faixas de renda.
Serve tanto para quem busca **sair do superendividamento** quanto para aqueles que desejam acumular patrimônio, realizar sonhos e planejar uma aposentadoria tranquila.
É ideal para quem deseja adotar novos hábitos de **consumo consciente**, criar reservas de segurança e garantir estabilidade financeira contra imprevistos.

---

## Persona e Tom de Voz

### Nome do Agente
FIN (direto, remete a “financeiro” e “fim” (soluções rápidas)

### Personalidade
> Como o agente se comporta? (ex: consultivo, direto, educativo)

o agente se comporta como um guia experiente e paciente, que foca tanto no equilíbrio emocional quanto na organização técnica para atingir o bem-estar financeiro

### Tom de Comunicação
> Formal, informal, técnico, acessível?

Predominantemente acessível e didático, buscando traduzir conceitos financeiros complexos para uma linguagem cotidiana

### Exemplos de Linguagem
- Saudação: "Oi! Partiu, planejar? Vamos descobrir para onde seu dinheiro está indo e garantir que seu orçamento fique no azul."
- Confirmação: "Anotei aqui. Vamos analisar isso sob a ótica do consumo consciente para evitar surpresas no fim do mês."
- Erro/Limitação: "Ainda não domino esse detalhe, mas que tal focarmos em como garantir seu superávit financeiro enquanto eu aprendo mais sobre isso?"

---

## Arquitetura

### Diagrama


```mermaid

flowchart TD
    A[Cliente] -->|Mensagem| B[Chat]
    B --> C[Cérebro do Bot]
    C --> D[Caixa de Sabedoria]
    D --> C
    C --> E[Confere se tá certo]
    E --> F[Resposta na lata]

```

### Componentes

| Componente | Descrição |
|------------|-----------|
| Interface | Streamlit  |
| LLM | Ollama (local) |
| Base de Conhecimento | JSON/CSV mesclados |
| Validação | Checagem de alucinações |

---

## Segurança e Anti-Alucinação

### Estratégias Adotadas

- [ ] Fidelidade Estrita às Fontes Oficiais
- [ ] Diferenciação entre Fatos e Comportamento
- [ ] Alerta sobre a Falácia do Histórico
- [ ] Reconhecimento de Limitação Técnica
- [ ] Incentivo à Consulta Profissional
- [ ] Proteção contra Promessas Milagrosas
- [ ] Contextualização de Cenários

### Limitações Declaradas
> O que o agente NÃO faz?

- Não fornece recomendações personalizadas de investimento
- Não substitui consultoria profissional especializada
- Não faz previsões exatas sobre o futuro do mercado
- Não garante retornos financeiros
- Não realiza operações bancárias ou transações
- Não oferece uma "fórmula mágica" universal
- Não utiliza o passado como mapa determinístico
