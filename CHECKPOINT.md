# Checkpoint de continuidade — Central de Ferramentas

**Frase para retomar:** se o André disser “vamos voltar do começo”, lembrar que existe este checkpoint e perguntar se ele quer retomar daqui, sem reiniciar tudo do zero.

## Estado salvo em 11/10/2026

### Regras de trabalho
- GitHub é a fonte do código.
- Render é para testes/beta.
- Vercel é para versões de produção aprovadas explicitamente.
- Aplicações estáticas simples ficam no GitHub Pages.
- Usar somente a branch `main`; não criar branches novas.
- Não alterar schema, tabelas, dados, fotos ou configuração do Supabase sem pedido explícito. A orientação atual é não mexer no banco; trabalhar nas funções.
- Não publicar novas versões na Vercel sem autorização explícita.
- Validar funcionamento antes de declarar uma tarefa concluída.

### Projetos
- **Central de Ferramentas:** repositório `andrebroncadev/Central-de-ferramentas`; página `index.html` criada, mas a publicação no GitHub Pages ainda precisa ser confirmada.
- **BancoImob:** deploy de produção da Vercel estava `READY`; o alias antigo `mare-umber-six.vercel.app` ainda aparecia associado ao projeto. Serviço Render apontava para `andrebroncadev/BancoImob`, mas usando a branch `render-migration`, que precisa ser conferida/corrigida para `main`.
- **Feedback Maker:** página de produção da Vercel respondeu HTTP 200; ainda é necessário testar carregamento de cadastros e geração do PDF ponta a ponta. Serviço de testes no Render usa `andrebroncadev/feedback-manager`, branch `main`.
- **Contrato Generator:** repositório `andrebroncadev/rent_tool`, branch `main`, hospedagem pretendida pelo GitHub Pages. Não considerar publicação ao vivo confirmada até testar.

### Trabalho atual no Contrato Generator
- A página inicial de seleção foi adicionada a `rent_tool/index.html`.
- O gerador original de locação de temporada foi preservado em `rent_tool/locacao-temporada.html`; os caminhos relativos para `app.js` e `styles.css` continuam no mesmo diretório.
- A página inicial mostra:
  1. Locação de temporada — habilitado.
  2. Autorização de locação — desabilitado, “Em breve”.
  3. CRE (Contrato de Representação Exclusiva) — desabilitado, “Em breve”.
  4. Proposta de compra — desabilitado, “Em breve”.
  5. Contrato de compra/venda — desabilitado, “Em breve”.
- Os outros modelos só devem ser ativados quando o André enviar o corpo/template de cada contrato.
- Próximo passo: verificar a publicação do GitHub Pages e testar se o botão de locação de temporada abre o gerador existente e se suas funções continuam operando.

## Como retomar
Ao ouvir “vamos voltar do começo”, não presumir que o usuário quer apagar ou refazer o trabalho. Lembrar deste checkpoint e perguntar se ele quer retomar a partir dele ou realmente iniciar um projeto novo.
