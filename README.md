# ReputationChecker
Jupyter Notebook para avaliação de Reputação de Domínios e IPs com Agentes de IA

# Análise de Reputação de IP/Domínio com Agentes Gemini

Este projeto utiliza a SDK do Google Gemini para criar um sistema de três agentes que trabalham em conjunto para analisar a reputação de um endereço IP ou domínio fornecido pelo usuário.

## Como funciona

O sistema é composto por três agentes:

1.  **Agente Buscador:** Este agente utiliza a ferramenta de busca do Google para encontrar as notícias e informações mais recentes sobre o IP ou domínio fornecido.
2.  **Agente Investigador:** Recebe as informações do Agente Buscador e as aprofunda usando a ferramenta de busca do Google, identificando os pontos mais relevantes para uma análise de reputação.
3.  **Agente Avaliador:** Utiliza as informações processadas pelos agentes anteriores, e se necessário consulta sites de reputação, para avaliar se o IP ou domínio pode ser considerado malicioso ou não, e gera um resumo justificando a avaliação.

## Pré-requisitos

Para rodar este notebook, você precisará:

*   Uma conta Google Cloud.
*   Uma chave de API do Google Gemini.
*   Instalar as bibliotecas necessárias (já incluídas no notebook).

## Configuração

1.  **Obtenha sua chave de API do Google Gemini:** Siga as instruções na documentação do Google AI para obter sua chave de API.
2.  **Configure a chave de API no Colab:** No Google Colab, vá em "Secrets" (ícone de chave) e adicione uma nova chave com o nome `GOOGLE_API_KEY` e o valor da sua chave de API.
3.  Execute as células do notebook.

## Uso

1.  Execute todas as células do notebook no Google Colab.
2.  Quando solicitado, digite o endereço IP ou domínio que você deseja avaliar.
3.  O sistema irá executar os três agentes e exibir os resultados de cada etapa, finalizando com a avaliação de reputação.

## Estrutura do Código

O notebook está organizado nas seguintes seções:

*   Instalação de bibliotecas.
*   Configuração da API Key e cliente Gemini.
*   Definição dos agentes (Buscador, Investigador, Avaliador).
*   Função auxiliar para chamar os agentes via Runner.
*   Função auxiliar para formatar a saída em Markdown.
*   Fluxo principal do sistema, interagindo com o usuário e executando os agentes em sequência.

## Contribuindo

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou pull requests.

## Licença

Este projeto está licenciado sob a MIT.
