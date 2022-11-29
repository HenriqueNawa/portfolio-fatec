#### Sobre o projeto


Projeto em parceria com a UOL, o projeto tem como base o monitoramento de websites e por meio de inteligência artificial prever quando um sistema irá cair para atuação preventiva, a fim de mitigar o problema de indisponibilidade.

#### Empresa parceira - UOL
A UOL é uma empresa brasileira de conteúdo, serviços e produtos de Internet, foi fundado em abril de 1996 por Luis Frias. De acordo com a Comscore, ela ocupa a terceira posição entre aqueles que operam propriedades multiplataforma na Internet do Brasil atrás do Google e Meta. Ainda de acordo com a Comscore, a UOL é o maior portal do Brasil com mais de 108 milhões de visitantes únicos por mês e 7,4 bilhões de páginas visitadas mensalmente.

#### Lista de Requisitos

Requisitos Funcionais
- Criação de página de formulário 
- Listagem de usuários cadastrados
- Prever indisponibilidade de sites

Requisitos Não Funcionais 
- Utilização de Vue.js para desenvolvimento do frontend
- Utilização de Java e Spring para desenvolvimento do backend
- Tempo de resposta de cadastro abaixo de 300ms
- Tempo de resposta de consulta abaixo de 100ms

#### Tecnologias Utilizadas
- Prometheus - utilizado para colher métricas
- Grafana - Visualizar as métricas geradas pelo Prometheus
- Locust - ferramenta para executar carga em aplicações
- Vue.js, HTML, CSS - Criação do frontend para página de formulário, login e listagem 
- Java, Spring, Mysql - Backend 
- Docker - para facilitar a execução das ferramentas de monitoramento
- Python, Pandas, Sklearn, Matplot - Utilizado para a previsão de indisponibilidade de websites utilizando Time Series e Análise de Sobrevivência 

#### Contribuições Pessoais
Neste projeto, atuei no desenvolvimento backend utilizando a arquitetura MVC com as tecnologias Java e Spring e a conexão com o Banco de Dados feita com Mysql.
#### Hard Skills
- Análise de requisitos - sei fazer com ajuda
- Desenvolvimento backend padrão MVC - sei fazer com ajuda
- Gerenciamento do Banco de Dados - sei fazer com autonomia
- Documentação do projeto - sei fazer com ajuda

#### Soft Skills
No decorrer do projeto, pude me desenvolver na parte de gerenciamento de tempo para que minhas entregas fossem realizadas no prazo, e na comunicação com a equipe para que as documentações estivesse coerente com as implementações descritas.

#### Demonstração do Monitoramento
Abaixo é possível observar que a aplicação está sendo alvejava pelo Prometheus, como também realiza consultas do estado atual da aplicação.

<p align="center">
  <img alt="prom" src="https://github.com/Oraculum-Fatec/sistema-cadastro-backend/blob/main/assets/prometheus_show.gif">
</p>

Temos também, uma breve demonstração da configuração do Grafana e dos dados exibidos a partir do Dashboard importado.

<p align="center">
  <img alt="graf" src="https://github.com/Oraculum-Fatec/sistema-cadastro-backend/blob/main/assets/grafana_show.gif">
</p>

### Métricas e Extração de Dados
Para analisar o estado atual da aplicação, é necessário focalizar as principais métricas capazes de indicar o funcionamento do sistema. Nesta situação, por ora, foram selecionadas as seguinte métricas:
  - Contagem por minuto de todos os HTTP Request GET; 
  - Contagem por minuto de todos os HTTP Request POST; 
  - Tempo de Resposta, em segundo, de todos os HTTP Request GET;
  - Tempo de Resposta, em segundo, de todos os HTTP Request POST;
  - Porcentagem atual de uso da CPU pela aplicação; 
  - Uso atual de Memória pela aplicação em bytes.

O Grafana possibilita a extração de dados dessas métricas específicas como um arquivo do tipo .csv. O arquivo será usado futuramente para o desenvolvimento da inteligência artificial capaz de prever indisponibildades do sistema.

Segue abaixo as métricas selecionadas destacadas em um painel do Grafana, as regras de alertamento do Prometheus e a apresentação destes dados.

<p align="center">
  <img alt="data" src="https://github.com/Oraculum-Fatec/sistema-cadastro-backend/blob/main/assets/getting_data_show.gif">
</p>


#### Github do projeto - [Oraculum](https://github.com/Oraculum-Fatec)
