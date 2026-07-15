# SAVEdesk 🏭💻

> Solução Web Intranet para Gestão de Chamados de TI de Baixa Complexidade.

![Status do Projeto](https://img.shields.io/badge/Status-Protótipo%20Funcional-green)
![License](https://img.shields.io/badge/License-Apache%202.0-blue)
![Stack](https://img.shields.io/badge/Stack-HTML5%20|%20CSS3%20|%20JS-orange)

## 📌 Sobre o Projeto

Este projeto foi desenvolvido como Trabalho de Conclusão de Curso (TCC), em resposta a uma demanda real da **OMPI do Brasil** através do SENAI.

O objetivo é otimizar o fluxo de chamados internos de TI de baixa complexidade (troca de toner, acesso à internet, reset de senhas), que anteriormente não possuíam controle métrico, gerando gargalos na alocação da equipe técnica.

A solução é um sistema **Web Lightweight** que opera sem necessidade de aquisição de novas licenças de software, focada na usabilidade em ambiente fabril (chão de fábrica).

## 🚀 Funcionalidades Principais

* **Interface do Solicitante (Fábrica):** Design simplificado para abertura e acompanhamento de chamados.
* **Dashboard Kanban (Técnicos):** Gestão visual interativa para a equipe de TI (Pendente, Em Andamento, Concluído) e triagem de prioridades.
* **Painel Administrativo:** Visão gerencial com gráficos em tempo real, gestão de utilizadores e exportação de relatórios (XLSX).
* **Acessibilidade Nativa:** Integração com a *Web Speech API*, permitindo digitação por voz (Speech-to-Text) e leitura de mensagens em voz alta (Text-to-Speech).
* **Métricas de Tempo:** Registro automático de timestamps para cálculo de SLA e KPIs de atendimento.
* **Zero Deploy:** Funciona diretamente no navegador, compatível com a infraestrutura legada da planta.
* **Responsividade:** Interface adaptável para desktops, tablets industriais e smartphones.

## 🛠 Tecnologias Utilizadas

O projeto segue a arquitetura Vanilla Web para garantir leveza e facilidade de manutenção interna:
* **Frontend:** HTML5 (Semântico), CSS3 (Flexbox/Grid/Variáveis Nativas).
* **Lógica e Interatividade:** JavaScript (ES6+).
* **Persistência de Dados (Protótipo):** LocalStorage e SessionStorage API.
* **Gráficos e Relatórios:** Chart.js e ExcelJS.
* **Persistência (Produção Proposta):** SQL Server / MySQL (Arquitetura mapeada).

## 📂 Estrutura do Projeto

Abaixo está a estrutura atualizada dos arquivos do sistema:

```text
├── index.html                   # Landing Page Institucional e Portal de Login Unificado
├── user.html                    # Painel do Solicitante (Abertura rápida e acompanhamento)
├── dashboard_ti.html            # Painel Kanban Técnico (Tratamento, triagem e resolução)
├── dashboard_administrador.html # Painel Admin (Gráficos Chart.js, relatórios CSV/Excel)
├── Logo.svg                     # Identidade Visual / Logotipo da empresa
├── LICENSE                      # Licença Apache 2.0
└── README.md                    # Documentação do projeto
```
Nota: Os dados são salvos no LocalStorage do seu navegador. Para limpar os dados e reiniciar os testes, utilize o botão "⚠️ Limpar Dados (Dev)" disponível no Dashboard Técnico.

🔮 Melhorias Futuras
Para a implantação final na OMPI, o roadmap inclui:

Substituição do LocalStorage por uma API REST (Node.js ou PHP).

Conexão com Banco de Dados SQL Relacional para persistência a longo prazo.

Implementação de autenticação via LDAP/Active Directory da empresa.  

Geração automática de relatórios gerenciais em PDF.  

📄 Licença  
Este projeto está licenciado sob a Licença Apache 2.0 - veja o arquivo LICENSE para detalhes.  

👨‍💻 Autores  
**Maiderson Junio de Souza Oliveira - Desenvolvedor Full Stack**

**Lorena Santos Figueredo - Analista de QA** 

**Raissa Ellen de Moraes - Engenheira de Software** 

**Matheus Henrique Teixeira Munis - Especialista em UX/UI e Designer**  

**Erick Gonçalves Amaral - Arquiteto de Banco de Dados**  

**Gizele Telheiro dos Santos - Analista de Negócios**

Projeto desenvolvido para o curso de Informática para Internet - SENAI.
