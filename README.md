# Meu Treino - App de Academia

Um aplicativo React para gerenciar treinos de academia com interface moderna e funcionalidades completas.

## Funcionalidades

- ✅ Criar e gerenciar treinos personalizados
- ✅ Adicionar exercícios com séries e repetições
- ✅ Executar treinos com controle de progresso
- ✅ Marcar séries como concluídas
- ✅ Registrar cargas utilizadas
- ✅ Histórico de treinos finalizados
- ✅ Modo escuro/claro
- ✅ Armazenamento local (localStorage)
- ✅ Interface responsiva

## Tecnologias Utilizadas

- React 18
- Tailwind CSS
- Lucide React (ícones)
- LocalStorage para persistência

## Como Executar Localmente

1. Instale as dependências:
```bash
npm install
```

2. Execute o projeto:
```bash
npm start
```

3. Abra [http://localhost:3000](http://localhost:3000) no seu navegador.

## Deploy na Cloudflare Pages

### Opção 1: Deploy Automático (Recomendado)

1. **Faça push do código para o GitHub**:
```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/SEU_USUARIO/gym-app.git
git push -u origin main
```

2. **Acesse o Cloudflare Dashboard**:
   - Vá para [dash.cloudflare.com](https://dash.cloudflare.com)
   - Clique em "Pages" no menu lateral
   - Clique em "Create a project"

3. **Conecte com o GitHub**:
   - Selecione "Connect to Git"
   - Autorize o Cloudflare a acessar seu GitHub
   - Selecione o repositório `gym-app`

4. **Configure o Build**:
   - **Framework preset**: Create React App
   - **Build command**: `npm run build`
   - **Build output directory**: `build`
   - **Root directory**: `/` (deixe vazio)

5. **Clique em "Save and Deploy"**

### Opção 2: Deploy Manual

1. **Crie o build de produção**:
```bash
npm run build
```

2. **Faça upload da pasta `build`**:
   - Vá para [dash.cloudflare.com](https://dash.cloudflare.com)
   - Clique em "Pages" → "Create a project"
   - Selecione "Direct Upload"
   - Arraste a pasta `build` para o upload

### Configurações Importantes

O arquivo `_redirects` já está configurado para lidar com as rotas do React SPA.

## Como Usar

1. **Criar um Treino**: Clique em "Novo Treino" e adicione exercícios
2. **Iniciar Treino**: Clique em "Iniciar Treino" em qualquer treino criado
3. **Executar**: Marque as séries como concluídas e registre as cargas
4. **Finalizar**: Clique em "Finalizar Treino" quando terminar
5. **Histórico**: Visualize todos os treinos finalizados

## Estrutura do Projeto

```
src/
├── components/
│   └── GymApp.js          # Componente principal
├── App.js                 # App wrapper
├── index.js              # Entry point
└── index.css             # Estilos globais
```

## Scripts Disponíveis

- `npm start` - Executa o projeto em modo desenvolvimento
- `npm build` - Gera build de produção
- `npm test` - Executa os testes
- `npm eject` - Ejecta do Create React App (irreversível)

## Vantagens do Deploy na Cloudflare Pages

- ⚡ **Performance**: CDN global para carregamento rápido
- 🆓 **Gratuito**: Plano gratuito generoso
- 🔄 **Deploy Automático**: Integração com GitHub
- 🛡️ **Segurança**: Proteção DDoS incluída
- 📱 **PWA Ready**: Suporte a Progressive Web Apps 