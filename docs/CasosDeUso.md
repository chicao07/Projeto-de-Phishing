# Casos de Uso

- ID: UC-001
- Nome: Detectar URLs
- Versão: 1.0
- Autores: Francisco dos Santos Dutra, Vinicius Andrade Silva Lima
- Data: 15/06/2026

Descrição:
  - O sistema de detecção de URLs tem como finalidade receber uma URL fornecida pelo usuário e analisá-la, classificando-a quanto ao seu nível de risco. O valor entregue por este caso de uso está em garantir maior segurança ao usuário, alertando-o sobre potenciais ameaças associadas ao acesso à URL informada.

Ator
  - Qualquer usuário do sistema, incluindo Clientes, Colaboradores e Parceiros de negócios que necessitem verificar a segurança de URLs antes de acessá-las.

Pré-condição:
  - O usuário deve possuir uma URL a ser verificada e submetê-la ao sistema para análise.

Pós-condição:
  - Após a análise, o sistema retornará o resultado da classificação da URL, que poderá ser: Segura, Suspeita ou Perigosa.

Fluxo Principal
  - O usuário obtém a URL a ser verificada.
  - O usuário digita a URL no campo do formulário.
  - O usuário envia a URL ao sistema.
  - O sistema analisa a URL recebida.
  - O sistema classifica a URL com base em critérios de pontuação.
  - O sistema compila um relatório com os possíveis problemas identificados na URL.
  - O sistema retorna o relatório de problemas ao usuário.
  - O sistema retorna a classificação final da URL ao usuário.

Fluxos de Exceção
  FE1 — URL inválida:
    - O usuário informa uma URL com formato inválido.
    - O sistema exibe a mensagem: "URL inválida."
  FE2 — Campo em branco:
    - O usuário tenta submeter o formulário sem preencher o campo de URL.
    - O sistema exibe a mensagem: "Campo obrigatório."



Regras de Negócio: 
  - RN01: O campo de URL é de preenchimento obrigatório.
  - RN02: URLs com formato inválido não serão aceitas pelo sistema.
  - RN03: Somente uma URL pode ser submetida por requisição.