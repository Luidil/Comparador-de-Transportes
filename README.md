# Comparador de Transportes em Salvador

Este projeto é um comparador de transportes que ajuda os usuários a determinar a melhor opção de transporte em Salvador, considerando custo, tempo e distância.

## Como Hospedar no Netlify

Siga estes passos para hospedar seu site no Netlify:

### Passo 1: Criar uma conta no Netlify
1. Acesse [https://app.netlify.com/](https://app.netlify.com/)
2. Clique em "Sign up" e crie uma conta (pode usar GitHub, Google ou email)

### Passo 2: Preparar os arquivos
1. Crie uma pasta para seu projeto
2. Dentro dela, crie um arquivo chamado `index.html`
3. Copie e cole todo o código HTML fornecido neste arquivo

### Passo 3: Fazer upload dos arquivos
1. No painel do Netlify, clique em "Add new site" > "Deploy manually"
2. Arraste e solte a pasta do projeto na área indicada
3. Aguarde o processo de deploy

### Passo 4: Acessar seu site
1. Após o deploy, o Netlify fornecerá uma URL (ex: `nomedoseu-site.netlify.app`)
2. Acesse esta URL para ver seu site funcionando

## Solução para Erro 404

Se você encontrar erro 404 no Netlify, siga estas soluções:

1. **Verifique o nome do arquivo principal**:
   - Ele deve se chamar exatamente `index.html` (com "i" minúsculo)
   - Não use nomes como `Index.html` ou `INDEX.HTML`

2. **Verifique a estrutura de arquivos**:
   - O arquivo `index.html` deve estar na raiz da pasta que você fez upload
   - Não coloque dentro de subpastas

3. **Limpe o cache do Netlify**:
   - Vá para "Site settings" > "Build & deploy" > "Deploy settings"
   - Em "Build settings", clique em "Clear build cache"

4. **Forçar novo deploy**:
   - Vá para "Deploys"
   - Clique em "Trigger deploy" > "Deploy site"

5. **Verifique o console de erros**:
   - No painel do Netlify, vá para "Deploys"
   - Clique no deploy mais recente
   - Verifique se há erros no log

## Recursos

- **OpenStreetMap**: Mapa gratuito e sem necessidade de chave API
- **OSRM**: Serviço de roteamento gratuito
- **Nominatim**: Geocodificação de endereços

## Personalização

Você pode personalizar os parâmetros de custo editando os valores iniciais no código:

```javascript
// Exemplo de personalização
document.getElementById('fuel-price').value = 6.20; // Novo preço da gasolina
document.getElementById('bus-fare').value = 4.50;   // Nova tarifa de ônibus