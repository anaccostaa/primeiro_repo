# 🐾 Patinhas Petshop
> Site institucional para pequeno negócio local — construído com HTML, CSS e JavaScript

🔗 **[Ver site no ar](https://anaccostaa.github.io/primeiro_repo/)**

---

## Sobre o projeto

O **Patinhas Petshop** é um site institucional desenvolvido para um pequeno negócio fictício de serviços para pets localizado em São João del Rei, MG. O projeto foi criado como solução prática para pequenos negócios que desejam ter presença online sem necessidade de contratar programadores.

---

## Tecnologias utilizadas

| Tecnologia | Uso |
|---|---|
| HTML5 semântico | Estrutura das páginas |
| CSS3 com variáveis | Estilização, animações e responsividade |
| JavaScript vanilla | Interatividade do formulário |
| GitHub Pages | Publicação gratuita com link público |
| Google Maps Embed | Integração do mapa no footer |
| Google Fonts API | Fontes Playfair Display e Inter |

---

## Páginas

| Página | Descrição |
|---|---|
| `index.html` | Página inicial com hero, serviços, relatos e footer |
| `banho_tosa.html` | Página de reserva com tabela de preços e formulário |
| `style.css` | Todos os estilos do site |
| `assets/` | Imagens dos pets e logo |

---

## Funcionalidades

- Header fixo com efeito de vidro fosco
- Hero com animação de entrada (fadeUp)
- Seção de serviços em grid com hover animado
- Relatos de clientes com fotos, nome, raça e depoimentos
- Tabela de preços com card de destaque
- Formulário de agendamento com validação em JavaScript
- Mensagem de confirmação dinâmica após envio
- Google Maps integrado no footer
- Layout 100% responsivo para celular, tablet e desktop

---

## Padrões web aplicados

### HTML semântico
```html
<header>, <nav>, <main>, <section>, <article>, <figure>, <footer>
```

### CSS Variables
```css
:root {
  --marrom: #5C3D2E;
  --laranja: #E8773A;
  --creme: #FAF6F0;
}
```

### Animações CSS
```css
@keyframes fadeUp {
  from { opacity: 0; transform: translateY(24px); }
  to   { opacity: 1; transform: translateY(0); }
}
```

### Responsividade
```css
@media (max-width: 768px) {
  .hero { grid-template-columns: 1fr; }
  .servicos-grid { grid-template-columns: repeat(2, 1fr); }
  .footer-grid { grid-template-columns: 1fr; }
}
```

### JavaScript — Formulário dinâmico
```javascript
form.addEventListener('submit', function(e) {
  e.preventDefault();
  if (!form.checkValidity()) { form.reportValidity(); return; }
  form.style.display = 'none';
  confirmacao.style.display = 'block';
  confirmacao.scrollIntoView({ behavior: 'smooth' });
});
```

---

## Acessibilidade

- `lang="pt-BR"` no HTML para leitores de tela
- Atributo `alt` descritivo em todas as imagens
- `<label>` conectado a cada campo do formulário
- `aria-label` nas estrelinhas de avaliação
- `aria-live="polite"` na mensagem de confirmação
- `title` no iframe do Google Maps
- Foco visível com `:focus-visible` para navegação por teclado

---

## Como rodar localmente

1. Clone o repositório:
```bash
git clone https://github.com/anaccostaa/primeiro_repo.git
```

2. Abra a pasta no VSCode

3. Abra o `index.html` no navegador

Não precisa de servidor ou instalação de dependências!

---

## Estrutura de arquivos

```
primeiro_repo/
│
├── index.html          — Página inicial
├── banho_tosa.html     — Página de reserva
├── style.css           — Estilos globais
├── README.md           — Este arquivo
└── assets/
    ├── logo_semfundo.png
    ├── Shitzu_tosado.jfif
    ├── yorkie_tosado.jfif
    └── poodle_tosado.jfif
```

---

*Projeto desenvolvido para a disciplina Padrões Web para No Code e Low Code — UniFECAF 2025.*
