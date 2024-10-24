# Amazon Bedrock Refeição por Ocasiao
Desafio de Código: Aplicação com AWS Step Functions e Amazon Bedrock
Este repositório contém a solução para o desafio do bootcamp "Nexa - Engenharia de Prompts na AWS com Claude" realizado na DIO. O desafio consistiu em criar uma aplicação utilizando AWS Step Functions e Amazon Bedrock para fornecer recomendações personalizadas de alimentação com base nas preferências e necessidades dos usuários.

Objetivo do Desafio
O objetivo do desafio era desenvolver uma aplicação interativa capaz de recomendar opções de alimentação em três cenários:

Faça você mesmo: Sugestão de lista de compras, locais para adquirir os ingredientes, receitas, empratamento e opções de pratos complementares.
Restaurante: Informações sobre o restaurante, avaliações de clientes, disponibilidade de reservas, pratos que combinam com a refeição escolhida e sugestões de traje.
Delivery: Como realizar o pedido, avaliações do estabelecimento, tempo de entrega e instruções para recriar o prato em casa.
Tecnologias Utilizadas
AWS Step Functions: Para orquestrar o fluxo da aplicação, gerenciando as diferentes etapas e opções.
Amazon Bedrock: Para processamento de linguagem natural, utilizado para interpretar as preferências do usuário e fornecer as recomendações apropriadas.
Arquitetura da Solução
A aplicação é composta por várias etapas no AWS Step Functions, onde cada estado representa uma fase do fluxo de interação com o usuário:

Identificação do Usuário: Determina a localização e preferências.
Identificação da Necessidade: Coleta informações sobre o objetivo do usuário (ocasião ou preferência).
Escolha de Opção: O usuário seleciona entre "faça você mesmo", "restaurante" ou "delivery".
Caminhos Diferenciados: Cada escolha leva a um fluxo específico para fornecer as informações adequadas.
Finalização: A interação é concluída com uma resposta personalizada.
Como Executar
Crie uma stack de AWS Step Functions: Use a definição de fluxo JSON fornecida no arquivo step_function_definition.json.
Configure o Amazon Bedrock: Verifique se o modelo escolhido está habilitado para sua conta e região.
Suba o fluxo no Step Functions: Teste as interações com diferentes entradas para validar as recomendações.
Estrutura do Repositório
step_function_definition.json: Definição do fluxo do Step Functions.
README.md: Documentação sobre o projeto.
arquivos-exemplos/: Exemplos de entrada e saída para testes do Step Functions.
Contribuindo
Contribuições são bem-vindas! Sinta-se à vontade para abrir issues e pull requests para melhorias.
