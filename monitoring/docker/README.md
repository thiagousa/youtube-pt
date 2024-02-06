# Pilha de Monitoramento com Prometheus, AlertManager, Grafana, Node Exporter, MailHog e NGINX 🚀

![Pré-visualização do Projeto](https://github.com/thiagousa/youtube/blob/main/monitoring/docker/screenshot/docker-design.png)

Bem-vindo ao projeto Pilha de Monitoramento, uma solução robusta e abrangente para monitoramento e gerenciamento da sua infraestrutura. Este projeto combina poderosas ferramentas de código aberto para ajudá-lo a continuar aprendendo sobre a infraestrutura de monitoramento.

## O que está incluído? 🧐

Este projeto oferece uma configuração pronta para uso de uma pilha de monitoramento que inclui:

- **Prometheus**: Uma das principais ferramentas de código aberto para monitoramento e alerta, projetada para confiabilidade e escalabilidade.

- **AlertManager**: Gerencia alertas enviados por várias aplicações, deduplica, agrupa, roteia e entrega-os aos destinatários corretos.

- **Grafana**: Uma plataforma de código aberto para monitoramento e observabilidade, completa com painéis personalizáveis e opções de visualização poderosas.

- **Node Exporter**: Um exportador do Prometheus que coleta métricas de hardware e do sistema operacional, essencial para o monitoramento do sistema.

- **MailHog**: Uma ferramenta de teste de e-mail para desenvolvedores, permitindo configurar a entrega SMTP e visualizar mensagens convenientemente.

- **Gerenciador de Proxy NGINX**: Simplifica o proxy reverso para sites com SSL gratuito, sem a complexidade da configuração do Nginx ou Letsencrypt.

## Primeiros Passos 🚀

Siga as instruções detalhadas de configuração na [documentação do projeto](https://github.com/thiagousa/youtube-pt/tree/main/monitoring/docker) para colocar sua pilha de monitoramento para funcionar rapidamente. Com apenas alguns passos simples, você terá acesso a um ambiente de monitoramento totalmente funcional.

## Funcionalidades e Benefícios 🌟

- **Configuração Fácil**: O projeto inclui arquivos de configuração bem definidos para cada componente, tornando a personalização simples.

- **Visualização Poderosa**: O Grafana permite que você crie painéis deslumbrantes e visualize dados em tempo real, ajudando a obter insights sobre sua infraestrutura.

- **Alertas e Notificações**: O AlertManager garante que você seja prontamente notificado sobre qualquer problema, permitindo tomar medidas proativas.

- **Escalável e Confiável**: O Prometheus é projetado, em sua essência, para confiabilidade e escalabilidade, tornando-o adequado para ambientes de pequena e grande escala.

- **Desenvolvimento Local**: O projeto é perfeito para desenvolvimento local, permitindo testar e otimizar sua configuração de monitoramento.

## Como Contribuir 🤝

Contribuições para este projeto são bem-vindas! Seja para corrigir um bug, melhorar a documentação ou adicionar novos recursos, confira nossas [Diretrizes de Contribuição](../../CONTRIBUTING.md) para começar.

## Licença 📜

Este projeto está licenciado sob a [Licença MIT](../../LICENSE), então você está livre para usá-lo em seus próprios projetos.

## Comece Hoje Mesmo! 🚀

Pronto para assumir o controle do monitoramento da sua infraestrutura? Comece com este projeto de Pilha de Monitoramento e mantenha seus sistemas funcionando sem problemas!

[![Monitoramento](https://github.com/thiagousa/youtube/blob/main/monitoring/docker/screenshot/monitoramento.png)](https://www.youtube.com/watch?v=eVi-ec7n_7cD)

[Assista ao Vídeo](https://www.youtube.com/watch?v=eVi-ec7n_7cD)

Sinta-se à vontade para personalizar e expandir esta descrição conforme necessário para o seu projeto no GitHub.

## Requisitos

Para configurar seu ambiente efetivamente para uso do Docker, juntamente com o Git, também é importante ter um editor de código. Aqui está uma lista atualizada de pré-requisitos:

1. **Docker Desktop**: Esta aplicação é essencial para executar aplicações em contêineres. Certifique-se de que o Docker Desktop esteja instalado e em execução no seu sistema. Você pode baixá-lo do [site oficial do Docker](https://www.docker.com/products/docker-desktop).

2. **Git**: Um sistema de controle de versão crucial para o gerenciamento de código, especialmente ao colaborar em equipe. Ajuda a rastrear alterações no código-fonte durante o desenvolvimento de software. Baixe o Git do [site oficial do Git](https://git-scm.com/downloads).

3. **Editor de Código (como o Visual Studio Code)**: Um editor de código é necessário para escrever e editar seu código. O Visual Studio Code (VS Code) é uma escolha popular devido à sua ampla gama de recursos, incluindo suporte para Docker e Git. Você pode baixar o VS Code do [site oficial do Visual Studio Code](https://code.visualstudio.com/). No entanto, você pode escolher qualquer outro editor de código com o qual se sinta confortável.

Com essas ferramentas instaladas, você terá uma configuração robusta para gerenciar contêineres Docker, manter seu código-fonte e editar seu código de forma eficaz.

### Linux ou MacOS 🏠 Edite Seu Arquivo Hosts

Adicione as seguintes entradas ao seu arquivo `/etc/hosts`:

```plaintext
127.0.0.1 nginx.acme.net
127.0.0.1 grafana.acme.net
127.0.0.1 prometheus.acme.net
127.0.0.1 alertmanager.acme.net
127.0.0.1 nodeexport.acme.net
127.0.0.1 mailhog.acme.net
127.0.0.1 services.acme.net
```

### Windows 🏠 Edite Seu Arquivo Hosts

1. **Abra o Bloco de Notas como Administrador**: 😎 Para exercer seu poder e editar o arquivo host do Windows, comece clicando com o botão direito do mouse no aplicativo Bloco de Notas no menu Iniciar. Escolha "Executar como administrador" porque você está no controle!

2. **Abra o Arquivo Hosts**: 📂 No Bloco de Notas, navegue até a sagrada pasta `C:\Windows\System32\drivers\etc`. Você não encontrará o arquivo host imediatamente porque ele é um pouco ninja. Para desmascará-lo, altere o tipo de arquivo para "Todos os Arquivos (*.*)."

3. **Edite o Arquivo Hosts**: 🖋️ Selecione o arquivo `hosts` e clique em "Abrir". Esta é a sua tela!

4. **Adicione Entradas de Host**: ✍️ Agora, vamos adicionar um pouco de magia. Adicione as entradas de host com a finesse de um maestro. Por exemplo:

   ```
   127.0.0.1 nginx.acme.net
   127.0.0.1 grafana.acme.net
   127.0.0.1 prometheus.acme.net
   127.0.0.1 alertmanager.acme.net
   127.0.0.1 nodeexport.acme.net
   127.0.0.1 mailhog.acme.net
   127.0.0.1 services.acme.net
   ```

   Coloque essas linhas no final do arquivo hosts, como a cereja do bolo!

5. **Salve as Alterações**: 📁 Após adicionar as encantadoras entradas de host, vamos selar o feitiço com um clique. Escolha "Arquivo" e depois "Salvar" no Bloco de Notas.

6. **Feche o Bloco de Notas**: 🚪 Você realizou sua mágica! Agora você pode fechar elegantemente o Bloco de Notas.

## Clonando o Projeto

Para começar com o projeto Pilha de Monitoramento, siga estes passos para clonar o repositório Git para sua máquina local:

1. **Abra um Terminal ou Prompt de Comando**: Inicie o aplicativo de terminal no seu computador.

2. **Clone o Repositório**: Execute o seguinte comando para clonar o repositório Git:

   ```shell
   git clone https://github.com/thiagousa/youtube.git
   ```

   Este comando criará um novo diretório chamado `youtube` em sua localização atual e clonará o projeto para dentro dele.

3. **Mude de Diretório**: Entre no diretório do projeto executando:

   ```shell
   cd youtube/monitoring/docker
   ```

Agora você clonou com sucesso o projeto Pilha de Monitoramento para sua máquina local e pode prosseguir com a configuração e exec

ução da pilha de monitoramento conforme descrito no restante deste readme.

### 🐳 Execute o Docker Compose

Navegue até o diretório do projeto e execute o seguinte comando para iniciar os serviços:

```bash
docker compose up -d
```

### 🔗 Acesse Todos os Serviços

Visite [Todos os Serviços](http://services.acme.net) para acessar os vários componentes da pilha de monitoramento.

![Captura de Tela](/monitoring/docker/screenshot/services.png)

## 📚 Descrição dos Serviços

### Prometheus 📈

[Prometheus](http://prometheus.acme.net) é sua ferramenta confiável de coleta e armazenamento de métricas. Armazena dados com carimbos de data/hora e rótulos opcionais, permitindo monitorar e analisar seus sistemas de forma eficaz.
![Captura de Tela](/monitoring/docker/screenshot/prometheus.png)

#### Arquivos de Configuração

- `alert_rules.yaml` para definir regras de alerta.
- `prometheus.yaml` para configuração do servidor Prometheus.

### AlertManager 🚨

[AlertManager](http://alertmanager.acme.net/#/alerts) lida com alertas enviados por aplicações cliente, deduplica, agrupa, roteia e entrega-os ao receptor correto. Também cuida do silenciamento e inibição de alertas.

![Captura de Tela](/monitoring/docker/screenshot/alertmanager.png)

### Grafana 📊

[Grafana](http://grafana.acme.net/) é sua solução de código aberto para análise e monitoramento. Use-a para visualizar seus dados de várias fontes.

![Captura de Tela](/monitoring/docker/screenshot/grafana.png)

#### Fonte de Dados

Configure o Prometheus como uma fonte de dados:

```yaml
datasources:
  - name: 'prometheus'
    type: 'prometheus'
    access: 'proxy'
    url: 'http://prometheus:9090'
```

Faça login com as seguintes credenciais:

- Usuário: admin
- Senha: s0W#Pg562^YA

### Node Exporter 🖥️

[Node Exporter](http://nodeexport.acme.net/) é um exportador do Prometheus para métricas de hardware e do sistema operacional expostas por kernels *NIX.

![Captura de Tela](/monitoring/docker/screenshot/nodeexport.png)

### MailHog 📧

[MailHog](http://mailhog.acme.net/) é uma ferramenta de teste de e-mail para desenvolvedores, perfeita para configurar a entrega SMTP para suas aplicações.

![Captura de Tela](/monitoring/docker/screenshot/mailhog.png)

### Gerenciador de Proxy Nginx 🌐

[Gerenciador de Proxy Nginx](http://nginx.acme.net/) simplifica o proxy reverso para sites e fornece SSL gratuito, tudo sem o incômodo da configuração do Nginx ou Letsencrypt.

![Captura de Tela](/monitoring/docker/screenshot/nginx.png)

Faça login com as seguintes credenciais:

- Usuário: acme@acme.net
- Senha: s0W#Pg562^YA

### Consulta Prometheus 📊

[Consulta Prometheus](http://prometheus.acme.net/) é onde você pode experimentar várias consultas e explorar seus dados.

![Captura de Tela](/monitoring/docker/screenshot/prometheus.png)

### ❌ Parando o Node Exporter para Receber o Alerta no Mailhog

Se precisar parar o Node Exporter, use este comando:

```bash
docker rm --force foobar-exporter
```

### 🧹 Deletando Todas as Aplicações

Para limpar todos os contêineres e redes em execução associados ao projeto, execute:

```bash
docker compose down
```

## Apoie Meu Trabalho

Criar vídeos e recursos de alta qualidade gratuitamente para todos é um desafio. Seu apoio me permite investir mais na criação de conteúdo, melhorando a qualidade geral. Tornar-se um membro oferece um apoio significativo e vem com vantagens legais como forma de agradecimento.

Lembre-se, ***o apoio é opcional***. Independentemente de você escolher se tornar um membro ou não, você terá acesso total a todos os meus vídeos e recursos.

Apoie aqui: [https://www.patreon.com/thi

agodsantos](https://www.patreon.com/thiagodsantos) ou [https://www.buymeacoffee.com/thiagodsantos](https://www.buymeacoffee.com/thiagodsantos)
