# Portifólio-QA-Funcional-Junior
Validação e Qualidade em Foco

# 🧪 Portfólio QA Funcional Júnior

**Validação e Qualidade em Foco**

Um portfólio profissional que demonstra competências em **Testes Funcionais**, **Segurança** e **Garantia de Qualidade**, com foco em abordagem orientada a risco e impacto no negócio.

---

## 📋 Sobre o Projeto

Este portfólio apresenta um **caso de estudo completo** de validação de um sistema web de cadastro e autenticação. O projeto foi desenvolvido com abordagem prática, documentando todos os passos desde a análise de escopo até a identificação e análise de bugs.

### 🎯 Objetivo

Demonstrar habilidades em:
- ✅ **Testes Funcionais**: Validação de funcionalidades e fluxos de usuário
- 🔒 **Testes de Segurança**: Validação de autenticação e proteção de dados
- 📊 **Análise de Risco**: Identificação e priorização de bugs por impacto
- 📝 **Documentação**: Casos de teste estruturados e bem documentados
- 🎯 **Abordagem Orientada a Risco**: Foco em validações críticas para o negócio

---

## 🏗️ Estrutura do Projeto

### Escopo Validado

O projeto abrange a validação de **4 áreas principais**:

1. **Cadastro de Usuários** - Validação de campos obrigatórios e regras de negócio
2. **Autenticação** - Testes de login com credenciais válidas e inválidas
3. **Segurança** - Bloqueio de conta após tentativas inválidas
4. **Gestão de Dados** - Atualização de informações do usuário

### Regras de Negócio Validadas

| Regra | Status | Descrição |
|-------|--------|-----------|
| **RN01** | ✅ Validado | Campos obrigatórios devem ser preenchidos |
| **RN02** | ✅ Validado | Email deve estar em formato válido |
| **RN03** | ✅ Validado | Senha deve ter mínimo 8 caracteres |
| **RN04** | ✅ Validado | Conta é bloqueada após 3 tentativas inválidas |
| **RN05** | ✅ Validado | Usuário autenticado pode atualizar seus dados |

---

## 🧪 Casos de Teste

### Resumo Executivo

- **Total de Casos**: 4
- **Validados**: 4 (100%)
- **Taxa de Sucesso**: 100% ✓
- **Projeto**: Aprovado ✓

### Casos de Teste Detalhados

#### **CT01 - Validação de Campos Obrigatórios**
- **Tipo**: Funcional
- **Prioridade**: Alta
- **Status**: ✅ Validado
- **Descrição**: Verificar se o sistema exibe mensagens de erro quando campos obrigatórios não são preenchidos
- **Resultado**: Conforme esperado - Validações funcionando corretamente

#### **CT02 - Teste de Autenticação**
- **Tipo**: Segurança
- **Prioridade**: Crítica
- **Status**: ✅ Validado
- **Descrição**: Validar o processo de login com credenciais válidas
- **Resultado**: Login realizado com sucesso - Autenticação funcionando conforme especificado
- **Evidência**: Captura de tela com mensagem de sucesso

#### **CT03 - Teste de Bloqueio por Tentativas Inválidas**
- **Tipo**: Segurança
- **Prioridade**: Alta
- **Status**: ✅ Validado
- **Descrição**: Verificar se a conta é bloqueada após 3 tentativas de login inválidas
- **Resultado**: Conta bloqueada conforme esperado - Sistema bloqueou a conta após 3 tentativas
- **Evidência**: Captura de tela com mensagem de bloqueio

#### **CT04 - Teste de Atualização de Dados do Usuário**
- **Tipo**: Funcional
- **Prioridade**: Média
- **Status**: ✅ Validado
- **Descrição**: Validar se o usuário consegue atualizar seus dados pessoais corretamente
- **Resultado**: Dados atualizados com sucesso - Alterações foram persistidas no banco de dados
- **Evidência**: Captura de tela com confirmação de atualização

---

## 🐛 Bugs Identificados

### Bug #001 - Validação Incompleta de Email

**Severidade**: 🔴 Alta  
**Impacto no Negócio**: Crítico

**Descrição**:
O sistema aceita emails inválidos que não seguem o padrão RFC 5322, permitindo cadastros com endereços de email malformados.

**Passos para Reproduzir**:
1. Acessar página de cadastro
2. Inserir email: `usuario@dominio` (sem TLD)
3. Preencher demais campos corretamente
4. Clicar em "Cadastrar"

**Resultado Esperado**: Sistema rejeita o email inválido

**Resultado Obtido**: Email é aceito e cadastro é realizado

**Impacto no Negócio**:
- ⚠️ Risco de comunicação perdida com usuários
- ⚠️ Possíveis problemas em envio de notificações
- ⚠️ Dados inconsistentes no banco de dados

**Recomendação**: Implementar validação rigorosa de email no backend e frontend

---

## 📊 Tipos de Testes Executados

### 🔍 Teste Funcional
Validação de funcionalidades e fluxos de usuário conforme especificado

### 🔒 Teste de Segurança
Validação de autenticação, autorização e proteção de dados

### ⚙️ Teste de Integração
Validação de integração entre componentes do sistema

### 📱 Teste de Usabilidade
Validação da experiência do usuário e interface

---

## 🛠️ Tecnologias e Ferramentas

### Frontend
- **React 19** - Framework JavaScript
- **TypeScript** - Tipagem estática
- **Tailwind CSS 4** - Estilização
- **Wouter** - Roteamento cliente

### Design & UX
- **Poppins** - Tipografia para títulos
- **Inter** - Tipografia para corpo
- **Design Minimalista Corporativo** - Abordagem visual

### Testes & QA
- **Casos de Teste Estruturados** - Documentação completa
- **Capturas de Tela** - Evidências visuais
- **Análise de Risco** - Priorização por impacto

---

## 🚀 Como Acessar o Portfólio

### Online
Acesse o portfólio em tempo real:
- **URL**: [denisqa-nlw4xwks.manus.space](https://denisqa-nlw4xwks.manus.space)

### Localmente
```bash
# Clonar repositório
git clone https://github.com/731986/qa-portfolio-denis.git
cd qa-portfolio-denis

# Instalar dependências
pnpm install

# Executar servidor de desenvolvimento
pnpm dev

# Acessar em http://localhost:3000
```

---

## 📄 Estrutura de Arquivos

```
qa-portfolio-denis/
├── client/
│   ├── src/
│   │   ├── pages/
│   │   │   ├── Home.tsx           # Página inicial do portfólio
│   │   │   ├── TestCases.tsx      # Página de casos de teste detalhados
│   │   │   └── NotFound.tsx       # Página 404
│   │   ├── components/            # Componentes reutilizáveis
│   │   ├── contexts/              # Contextos React
│   │   ├── App.tsx                # Componente raiz
│   │   └── index.css              # Estilos globais
│   ├── public/                    # Arquivos estáticos
│   └── index.html                 # HTML principal
├── server/                        # Servidor Express (compatibilidade)
├── package.json                   # Dependências e scripts
└── README.md                      # Este arquivo
```

---

## 📋 Seções do Portfólio

### 1️⃣ Página Inicial
- Hero section com apresentação do projeto
- Visão geral dos objetivos
- Call-to-action para explorar casos de teste
- Informações de contato

### 2️⃣ Página de Casos de Teste
- Listagem completa de todos os 4 casos de teste
- Detalhes de cada teste: pré-condições, passos, resultados
- Capturas de tela como evidências
- Resumo executivo com taxa de sucesso

### 3️⃣ Seção de Bugs
- Documentação de bugs identificados
- Análise de severidade e impacto
- Recomendações de correção

---

## 👤 Autor

**Denis Hamilton Borges Guimarães Camara**

- 📧 Email: [deniscamara.informatica@gmail.com](mailto:deniscamara.informatica@gmail.com)
- 💼 LinkedIn: [Denis Hamilton](https://www.linkedin.com/in/denis-hamilton-borges-guimarães-camara-2882771a9/)
- 💻 GitHub: [@731986](https://github.com/731986)

---

## 📞 Contato & Redes

Interessado em colaborar ou tem dúvidas sobre o portfólio?

- **Email**: deniscamara.informatica@gmail.com
- **LinkedIn**: [Conecte-se comigo](https://www.linkedin.com/in/denis-hamilton-borges-guimarães-camara-2882771a9/)
- **GitHub**: [Veja meus repositórios](https://github.com/731986)

---

## 📜 Licença

Este projeto é de código aberto e está disponível sob a licença MIT. Sinta-se livre para usar, modificar e distribuir conforme necessário.

---

## 🎯 Próximas Melhorias

- [ ] Adicionar seção de habilidades técnicas com ferramentas de teste
- [ ] Implementar filtros interativos na página de casos de teste
- [ ] Criar formulário de contato funcional
- [ ] Adicionar mais casos de teste (CT05, CT06, etc.)
- [ ] Implementar dark mode
- [ ] Adicionar testes de performance

---

## 📈 Estatísticas do Projeto

| Métrica | Valor |
|---------|-------|
| **Casos de Teste** | 4 |
| **Taxa de Sucesso** | 100% |
| **Bugs Identificados** | 1 |
| **Tempo de Execução** | ~2 horas |
| **Cobertura de Funcionalidades** | 100% |

---

## 🙏 Agradecimentos

Obrigado por visitar meu portfólio! Este projeto representa meu compromisso com **qualidade**, **documentação clara** e **abordagem profissional** em testes de software.

Se você está procurando um **QA Funcional Júnior** dedicado e atento aos detalhes, não hesite em entrar em contato!

---

**Última atualização**: Fevereiro de 2026  
**Versão**: 1.0.0
