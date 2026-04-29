Este projeto demonstra uma integração completa de captura de dados (Web-to-Lead), validação de regras de negócio via código (Apex) e automação de processos (Flow).

🛠️ Arquitetura do Projeto
O fluxo de dados segue a seguinte hierarquia:

Front-end: Página estática hospedada no GitHub Pages utilizando Tailwind CSS.

Integração: Captura via protocolo POST (Web-to-Lead) diretamente para o endpoint da Salesforce API.

Camada de Validação (Back-end): Uma Trigger Apex intercepta o registro antes da inserção para validar se o telefone possui o formato brasileiro de 11 dígitos.

Camada de Automação: Um Record-Triggered Flow processa o Lead e, caso o setor seja "Technology", realiza o roteamento automático para uma fila de atendimento específica.
