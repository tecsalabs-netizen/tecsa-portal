# Tecsa Portal - Sistema de Acesso aos Exames

Portal de acesso com autenticação para download de documentos/exames de usuários.

## 📁 Estrutura do Projeto

```
tecsa-portal/
├── index.html                      # Página de login
├── download_007311940.html         # Página de download - Usuário 1
├── download_007311941.html         # Página de download - Usuário 2
├── images/                         # Pasta de imagens
│   ├── bg-login.jpg               # Imagem de fundo (substituir)
│   ├── tecsa.jpg                  # Logo Tecsa (substituir)
│   └── ssl-site-seguro.png        # Selo SSL (substituir)
├── documento_007311940.pdf        # PDF Usuário 1 (adicionar)
├── documento_007311941.pdf        # PDF Usuário 2 (adicionar)
└── README.md                      # Este arquivo
```

## 🔐 Credenciais de Login

| Usuário | Senha | Redirecionamento |
|---------|-------|------------------|
| 007311940 | 36534830 | download_007311940.html |
| 007311941 | 24078104 | download_007311941.html |

## 🎨 Design e Tecnologias Utilizadas

- **Bootstrap 3.3.5** - Framework CSS responsivo
- **Font Awesome 4.4.0** - Ícones
- **Ionicons** - Ícones adicionais
- **iCheck** - Checkbox customizado
- **Google Fonts** - Fonte Montserrat (700, 400)
- **Cores principais:**
  - Teal primário: `#095a53`
  - Teal hover: `#00acd6`
  - Verde: `#a0c32e`

## ⚙️ Funcionalidades

✅ Autenticação com 2 usuários hardcoded  
✅ Validação de credenciais em JavaScript  
✅ Redirecionamento automático para página de download  
✅ Mensagem de erro em vermelho: "Usuário ou senha inválidos."  
✅ Erro desaparece ao digitar ou trocar abas  
✅ Layout responsivo com Bootstrap  
✅ 3 abas visuais (Tutor, Veterinário, Clínica)  
✅ Design consistente em todas as páginas  
✅ Footer com informações de copyright e SSL  

## 📝 Como Adicionar Imagens

1. Acesse a pasta `/images/`
2. Substitua os arquivos placeholder pelos arquivos reais:
   - **bg-login.jpg** - Imagem de fundo (recomendado: 1920x1080px ou maior)
   - **tecsa.jpg** - Logo da Tecsa (altura: 53px)
   - **ssl-site-seguro.png** - Selo SSL seguro (altura: 25px)

### Recomendações de Dimensões

- **bg-login.jpg**: 1920x1080px (16:9), JPG ou PNG
- **tecsa.jpg**: 200x53px (qualidade alta)
- **ssl-site-seguro.png**: 100x25px (PNG com fundo transparente)

## 📄 Como Adicionar PDFs

1. Acesse a raiz do projeto
2. Adicione os arquivos PDF:
   - **documento_007311940.pdf** - Documento do usuário 1
   - **documento_007311941.pdf** - Documento do usuário 2

Os PDFs serão baixados ao clicar no botão "Baixar Documento" na página de download.

## 🚀 Como Usar

1. Clone ou acesse o repositório
2. Abra `index.html` em um navegador
3. Faça login com uma das credenciais acima
4. Será redirecionado para a página de download correspondente
5. Clique em "Baixar Documento" para fazer download do PDF

## 🔒 Segurança

⚠️ **Importante**: As credenciais estão armazenadas em JavaScript (código fonte). Para um ambiente de produção, implemente:
- Autenticação no backend
- Hash de senhas
- Tokens JWT ou Sessões
- HTTPS obrigatório
- CORS adequado

## 📱 Responsividade

O portal é responsivo e funciona em:
- Desktop (1920px e acima)
- Tablet (768px a 1024px)
- Mobile (320px a 767px)

## 🐛 Troubleshooting

### Imagens não carregam
- Verifique se os arquivos estão em `/images/`
- Nomes dos arquivos devem estar corretos e em minúsculas
- Use caminhos relativos: `images/arquivo.jpg`

### PDFs não fazem download
- Verifique se os arquivos PDF estão na raiz do projeto
- Nomes devem corresponder aos links (documento_007311940.pdf, etc)
- Se hospedado em servidor, configure CORS corretamente

### Erro ao fazer login
- Verifique a capitulação do usuário/senha (sensível a maiúsculas)
- Remova espaços em branco antes/depois
- Abra o console (F12) para verificar se há erros JavaScript

## 📧 Suporte

Para dúvidas ou problemas, entre em contato com o administrador do sistema.

---

**Versão**: 1.0  
**Último update**: 2026  
**Desenvolvido por**: SOFTEASY
