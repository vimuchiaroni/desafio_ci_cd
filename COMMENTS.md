# Ferramentas escolhidas

- ci/cd - Jenkins
- monitoring e estatisticas - Graphite - prometheus
- infraestrutura - Vagrant + Docker


# Motivos

Utilizar o Jenkins para realizar a esteira de deployment devido a minha familiaridade com a ferramenta e os diversos plugins disponiveis(GIT, Docker, k8s etc.).
Os passos básicos necessários para o deploy da api são: 
- "Conteinerizar" a api;
- Baixar o código fonte disponibiizado no git;
- fazer o build da imagem docker;
- fazer o push da imagem para um repositório central;
- Parar as instancias atuais da aplicação(se existirem);
- fazer o depoy da nova versão da api;
- realizar um teste primário de acesso a url;
- Um serviço do graphite para exibir estatisticas da api.


