# 🐞 BugBash Guide

O **BugBash** é uma prática colaborativa de testes manuais intensivos que já implementei nos times das empresas por onde passei, como **QuintoAndar**, **SoftExpert** e **Pitang**. Ele tem como objetivo principal encontrar falhas que poderiam passar despercebidas em testes convencionais, promovendo uma entrega mais segura e com melhor experiência para o usuário. Além disso, também funciona como um momento estratégico de **passagem de conhecimento entre membros do time**, fortalecendo a cultura de qualidade.

O BugBash normalmente ocorre **antes da entrega da feature**, mas pode ser adaptado para acontecer logo após, dependendo do contexto da equipe. Trata-se de uma iniciativa em que todo o time — incluindo pessoas de desenvolvimento (back e front), QA, produto e design — participa testando a funcionalidade como se fossem usuários finais. Essa diversidade de olhares traz múltiplas perspectivas e aumenta a chance de detectar problemas reais.

Para organizar um BugBash, a pessoa responsável por QA (ou alguém de qualidade/design/desenvolvimento, dependendo da estrutura do time) deve criar uma **tarefa principal no board**, com o título padronizado:

```bash
[Bugbash] Nome da Feature
```

Essa tarefa conterá uma descrição explicando a funcionalidade que será testada, os objetivos da sessão e os caminhos principais ou alternativos previstos. Caso a equipe não utilize ferramentas específicas como o **X-Ray** ou **Zephyr**, essa estrutura pode ser feita diretamente no Jira, utilizando **épicos e subépicos**, onde o BugBash se torna o épico e os bugs encontrados viram subtarefas ou itens vinculados a ele. 

Antes da sessão, a pessoa responsável alinha com o time os objetivos da feature e garante que o ambiente esteja pronto, com dados pré-cadastrados se necessário. A preparação também pode incluir sugestões de cenários e instruções para quem não conhece a feature a fundo.

Durante o BugBash, cada pessoa explora a funcionalidade livremente, testando a interface como um usuário comum — inclusive forçando cenários alternativos, inputs errados e caminhos que não seriam cobertos pelos testes convencionais. Todos os problemas encontrados devem ser documentados com print, passo a passo e classificação.

Os bugs devem ser classificados por criticidade:

- 🚫 **Block**: Impede a entrega da feature e precisa ser resolvido antes do deploy.
- ⚠️ **Produção**: Já ocorre em produção, precisa ser documentado, mas não bloqueia a entrega atual.
- 🔻 **Minor**: Problema leve, pode ser resolvido se houver tempo disponível.
- 🚀 **Melhoria**: Algo que não estava previsto no escopo, mas que pode ser convertido em débito técnico ou backlog.

Ao final do BugBash, a pessoa responsável comunica o time com um resumo da sessão. Essa comunicação pode ser feita por canais como Teams ou Slack, e deve conter:

- Status geral da entrega: Pronto para deploy, bugs leves encontrados, bloqueios, etc.
- Lista dos principais problemas encontrados
- Previsão de nova entrega, se houver necessidade de correção

O BugBash também permite a geração de métricas importantes para o time, como:

- Quantidade de bugs por funcionalidade
- Classificação média dos erros (criticidade)
- Volume de melhorias identificadas
- Nível de confiabilidade das entregas por squad

Essas métricas ajudam a entender se o time está testando bem, se os testes automatizados estão cobrindo os principais riscos e quais áreas precisam de mais atenção nas próximas entregas.

Caso sua equipe utilize ferramentas como o **X-Ray** ou **Zephyr**, é possível documentar todo o processo diretamente nelas. Mas, se não for o caso, uma boa prática é usar o próprio Jira, Notion, Trello ou até planilhas para organizar os dados.

Recomenda-se que o BugBash tenha uma **frequência consistente** dentro dos ciclos de desenvolvimento. Pode ser semanal, quinzenal ou até sob demanda, mas o importante é manter esse ritual como parte da cultura do time.

> Um bug encontrado no BugBash é um bug que **não** chega na mão do cliente. É um ato de prevenção e excelência coletiva. ✨

Se quiser trocar ideias sobre como adaptar o BugBash à sua realidade, me chama no [LinkedIn](https://www.linkedin.com/in/andrelineflira) ou no [Instagram](https://www.instagram.com/rotaesabor) 💜
