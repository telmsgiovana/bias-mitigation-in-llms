# Mitigação de viés de confirmação em LLMs
Pesquisa desenvolvida durante estágio de verão no INESCTEC. 

A pesquisa consistiu em realizar 52 perguntas enviesadas na área da saúde (validadas por equipe técnica da área), e aplicar 9 medidas de mitigação para viéses de confirmação em LLMs, 
analisando o comportamento diante da pergunta enviesada x medida de mitigação.
As medidas foram divididas em 3 categorias:
1-Base de Dados:
Disponibilizamos uma base de dados com afirmações verdadeiras validadas por equipe da área da saúde, e em seguida fazemos a pergunta enviesada;
Disponibilizamos uma base de dados informando que as informações das perguntas enviesadas são falsas, e em seguida fazemos a pergunta enviesada;

2-Engenharia de Prompt:
Realizamos a pergunta de forma não-enviesada, ou seja neutra, e avaliamos o comportamento;
Antes de fazer a pergunta enviesada, colocamos o prompt one-shot;
Antes de fazer a pergunta enviesada, colocamos o prompt few-shot;


3-Fine-Tuning:
Antes de realizar a pergunta, colocamos um Fine-Tuning para conscientização de viés;
Antes de realizar a pergunta, colocamos um Fine-Tuning para autocrítica simulada;
Antes de realizar a pergunta, colocamos um Fine-Tuning para consulta de múltiplas fontes;
Antes de realizar a pergunta, colocamos um Fine-Tuning de protocolo de verificação de viés;


---

## Como usar

Para conseguir rodar os códigos, é necessário antes  criar a sua chave de API em openrouter.ai e substituir nos locais indicados no código.
As bases de dados utilizadas nos códigos estão na pasta bases-dados. 
Para o código dos testes de Bases de Dados, utilizamos as planilhas: perguntas_enviesada, base-afirmações-corretas e base-afirmações-incorretas.
Para o código dos testes de Engenharia de Prompt, utizamos apenas a planilha: eng_prompt
Para o código dos teste de Fine-Tuning, utilizamos apenas a planilha perguntas_enviesadas

---
