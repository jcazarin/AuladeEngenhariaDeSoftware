🎓 Engenharia de Software - ADS | IFMT Campo VerdeEste repositório é o espaço oficial para as atividades práticas e colaborativas da disciplina de Engenharia de Software, ministrada para a turma de Tecnologia em Análise e Desenvolvimento de Sistemas (ADS) do IFMT Campus Campo Verde.O objetivo central deste projeto é integrar os conceitos teóricos de engenharia, modelagem de sistemas e processos de desenvolvimento com o uso de ferramentas reais da indústria, como Git e GitHub.🚀 Objetivos da DisciplinaNeste ambiente, exploraremos as seguintes competências:Gerenciamento de Configuração: Uso profissional de controle de versão, branches e fluxos de trabalho (Git Flow).Documentação Dinâmica: Escrita técnica e modelagem utilizando Markdown e Mermaid.Desenvolvimento Colaborativo: Prática de Code Review, abertura de Issues e submissão de Pull Requests.Qualidade de Software: Aplicação de padrões de projeto e testes para garantir a integridade das soluções.📊 Exemplo de Modelagem: Fluxo de PedidoComo parte das atividades de documentação, utilizamos o Mermaid para representar processos. Abaixo está o diagrama de atividades para o recebimento de pedidos:graph TD
    Start(( )) --> Receber[Receber Pedido]

    %% Barra de Fork (Paralelismo)
    Receber --> Fork_Bar[ ]
    style Fork_Bar fill:#000,stroke:#000,stroke-width:4px

    %% Fluxo de Entrega
    Fork_Bar --> Preencher[Preencher Pedido]
    Preencher --> Entrega[Realizar Entrega]

    %% Fluxo de Faturamento
    Fork_Bar --> Fatura[Enviar Fatura]
    Fatura --> Pagamento[Receber Pagamento]

    %% Barra de Join (Sincronização)
    Entrega --> Join_Bar[ ]
    Pagamento --> Join_Bar[ ]
    style Join_Bar fill:#000,stroke:#000,stroke-width:4px

    %% Finalização
    Join_Bar --> Fechar[Fechar Pedido]
    Fechar --> End((( )))

    classDef box rx:15,ry:15,fill:#f9f9f9,stroke:#333,stroke-width:1px
    class Receber,Preencher,Entrega,Fatura,Pagamento,Fechar box
🤝 Instruções para a TurmaPara participar das atividades e contribuir com o repositório, siga as diretrizes estabelecidas em aula:Acompanhamento: Verifique regularmente a aba de Issues para novas tarefas e desafios.Contribuição: Utilize o fluxo de Fork e Pull Request para submeter suas implementações ou correções de documentação.Padrões: Mantenha as mensagens de commit claras e siga a estrutura de pastas proposta.✨ Contribuidores (Hall of Fame)Neste projeto, valorizamos cada contribuição! Utilizamos o sistema All Contributors para reconhecer quem ajuda a construir este conhecimento.<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section --><!-- O Bot All-Contributors irá gerar a lista aqui automaticamente após ser configurado --><img src="https://github.com/identicons/prof-bruna.png" width="100px;"/><br /><sub><b>Bruna Patricia</b></sub><br />📖 💡<img src="https://github.com/identicons/aluno-ads.png" width="100px;"/><br /><sub><b>Aluno ADS</b></sub><br />💻 🎨<!-- ALL-CONTRIBUTORS-LIST:END -->🏛️ Instituição e ContatoCurso: Tecnologia em Análise e Desenvolvimento de Sistemas (ADS)Campus: IFMT Campo Verde - MTProfessor(a): Bruna Patricia CoutinhoDúvidas sobre o conteúdo ou sobre o uso do repositório? Abra uma Issue ou entre em contato pelos canais oficiais da disciplina.
