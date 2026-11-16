# Combina? — Protótipo acadêmico (PWA)

Versão mobile-first compartilhável das telas **Explorar** e **Perfil**, baseadas nas versões aprovadas do Combina? Design System 1.0.

## O que funciona
- Buscar e filtrar 10 locais de Porto Alegre por categoria e nome
- Fotografias reais *ilustrativas* (do Unsplash, não necessariamente dos estabelecimentos) com imagem alternativa se falhar
- Cartões compactos com fotos de 104 × 104 px à esquerda
- Favoritar estabelecimentos e vê-los na seção **Salvos**
- Perfil fictício com Top 5, XP, avaliações recentes/mais engajadas e métricas demonstrativas
- Notificações demonstrativas; engrenagem com edição de nome, usuário, cidade, bio e interesses
- Alternar **Day** / **After Dark**
- Barra inferior com Explorar, Mapa, +, Salvos e Perfil
- Layout responsivo, PWA instalável sob HTTPS, preferências locais via localStorage

**Limites:** o Mapa e o editor de publicação não possuem backend. Não existe autenticação, persistência compartilhada, dados reais de usuários nem avaliações reais. Cada visitante tem seus próprios dados locais. As fotos dependem da Internet, salvo os ícones alternativos.

## Como publicar sem pagar (GitHub + Vercel)
1. Crie uma conta gratuita em https://github.com e um repositório, por exemplo `combina-prototipo`.
2. Envie **todos os arquivos desta pasta**, mantendo `index.html` e `vercel.json` na raiz. Pela interface do GitHub: **Add file → Upload files → Commit changes**. O repositório pode ser privado; verifique as opções de importação na Vercel.
3. Entre em https://vercel.com/new, faça login com GitHub e importe o repositório.
4. Em **Framework Preset** escolha **Other** (ou deixe a detecção de projeto estático), **Root Directory** `./`, e sem comando de build ou diretório de saída personalizado. Clique **Deploy**.
5. Quando o deploy terminar, compartilhe a URL `.vercel.app` exibida na Vercel. Em cada novo commit na branch principal, a Vercel publica uma atualização.

Vercel Hobby é gratuito para uso pessoal e não comercial, sujeito a limites e políticas. Não é preciso comprar domínio.

## Testar localmente
Na pasta do projeto, execute `python -m http.server 8000` e abra `http://localhost:8000` no navegador. PWA instalável requer HTTPS, exceto no localhost.

## Créditos e direitos das imagens
As fotografias vêm de `images.unsplash.com`, usadas apenas como referências genéricas de comida e ambientes; **não** são fotos verificadas dos estabelecimentos. Antes de lançar um produto real, confirme direitos/licenças e substitua-as por imagens autorizadas de cada local. Consulte https://unsplash.com/license. Fontes da interface: Google Fonts (Plus Jakarta Sans, DM Sans, Space Grotesk), sujeitas às respectivas licenças abertas.

## Identidade
Design system fornecido: #DFFF33, #111111, #F8F3EA, #EEDFC6, #6B2E8A, #C96A4A, #F4A300. Modo noturno: #101019, #20152C, #352342, #CBBED6.
