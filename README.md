# Ísis
Aplicação web de suporte emocional, psicológico e de proteção para mulheres em situação de violência. O objetivo é reunir em um só lugar ferramentas de emergência, acolhimento, informação e reconstrução de vida, de forma segura e acolhedora.

##Como principais funcionalidades: \
Botão de pânico - Pedido de ajuda rápido, com envio de localização para contatos de confiança e serviços de emergência. Também oferece atalho para o **180** (Central de Atendimento à Mulher, 24h, gratuita e sigilosa).\
Diário digital - Registro diário de sentimentos e humor (feliz, bem, neutra, triste, irritada), histórico de registros e **cofre digital** para fotos, áudios e documentos.\
Chat de conversa - Atendimento psicológico, orientação jurídica e chat popular entre usuárias.\
Redes de apoio - Mapa para localizar hospitais, delegacias e advogados próximos.\
Informações que protegem - Conteúdo sobre tipos de violência, leis e direitos, e como denunciar.\

## Tecnologias
*React
*Vite
*TypeScript
*FireBase
*Socket.IO
*Maps JavaScript API
*Places API (New)

##Como rodar o Projeto
Baixe o arquivo e extraia. \
Abra no terminal e rode os comandos:
npm install
npm run dev

## Como rodar o Chat
Abra a raiz do projeto no terminal e rode:
npm install

cd backend
npm install

Confira se o arquivo .env.local da raiz contém VITE_SOCKET_URL=http://localhost:3001, que é o endereço do servidor de chat. Se alterar esse arquivo, reinicie o Vite, pois ele só lê as variáveis ao iniciar.\

Em seguida, abra dois terminais. No primeiro, entre em backend e rode npm run dev; deve aparecer a mensagem "Servidor rodando na porta 3001". No segundo, rode npm run dev na raiz para subir o frontend, que abre em http://localhost:5173.\

Para testar, entre com uma conta numa janela normal e com outra conta numa janela anônima, já que o Firebase guarda o login por navegador. Nas duas, acesse Chat e depois Chat popular, e envie uma mensagem: ela deve aparecer nas duas telas quase instantaneamente, e o terminal do backend registrará a entrada de cada pessoa na sala. Use contas diferentes, porque com a mesma conta todas as mensagens aparecem como se fossem suas.
