SDW2025 – Pipeline ETL Portifólio







📌 1. Introdução

Este projeto tem como objetivo construir um portfólio baseado em dados estruturados de usuários, utilizando arquivos locais, GitHub como fonte estática e integrações com APIs externas.

O trabalho surgiu da necessidade de contornar a indisponibilidade da API oficial da SDW2025, garantindo autonomia e continuidade no desenvolvimento.

🚀 2. Etapas do Desenvolvimento

2.1 Criação da Base de Dados

Devido ao desligamento temporário da API do curso, foi necessário criar uma estrutura própria de dados.

Foram criados os arquivos:

usuarios.json — contém todas as informações completas dos usuários.

SDW2025-userID.csv — arquivo auxiliar contendo apenas os IDs para uso direto no Google Colab.

📄 Conteúdo do arquivo SDW2025-userID.csv:

userID
4
5
6

Esse arquivo permitiu identificar os usuários e cruzar dados no processamento.

2.2 API Utilizada — GitHub

O GitHub foi utilizado como um servidor estático de dados. Os arquivos dados.json e SDW2025-userID.csv foram hospedados e servidos via URLs públicas, simulando endpoints de uma API tradicional.

Vantagens:

Alta disponibilidade

Zero custo

Fácil integração com Google Colab

Não requer backend ativo

2.3 Tratamento e Transformação dos Dados

No Google Colab, os dados foram carregados, estruturados e transformados utilizando Python e Pandas para compor as visualizações e análises desejadas.

2.4 Uso da API da OpenAI e Limitações Encontradas

Para algumas etapas de transformação e enriquecimento dos dados, foi configurada a API da OpenAI, com a geração de uma Secret Key (key).

No entanto, ao executar a etapa TRANSFORM, ocorreu o erro:

RateLimitError: Error code: 429 - {'error': {'message': 'You exceeded your current quota, please check your plan and billing details. For more information on this error, read the docs: https://platform.openai.com/docs/guides/error-codes/api-errors.', 'type': 'insufficient_quota', 'param': None, 'code': 'insufficient_quota'}}

Esse erro indica que o limite de uso da conta foi atingido, impossibilitando continuar usando a API naquele momento.

📁 3. Estrutura do Projeto

SDW2025_Projeto_Portifólio/

│

├── dados.json                # Base completa dos usuários

├── SDW2025-userID.csv        # Lista dos IDs

├── README.md                 # Documentação

└── exemplo_colab.ipynb       # Exemplo opcional para uso no Colab

🧾 4. Conclusão

Mesmo com limitações, especialmente relacionadas à cota da API da OpenAI, foi possível construir uma estrutura funcional, documentada e totalmente independente da API original.
Esse projeto demonstra domínio de manipulação de dados, criação de fontes alternativas e integração com Google Colab.



🙏 5. Agradecimentos

Este projeto também é um reflexo do impacto positivo da jornada proporcionada pela DIO (Digital Innovation One).A toda a equipe, meu sincero agradecimento pela dedicação, pelos conteúdos de qualidade e pela motivação constante em incentivar estudantes e profissionais a evoluírem na prática.

Obrigado por criarem um ambiente acessível, acolhedor e transformador. Cada módulo, desafio e mentoria contribuíram diretamente para minha evolução — e este portfólio é uma prova disso. 💙


