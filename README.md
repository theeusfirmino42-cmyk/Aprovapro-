# AprovaPro — protótipo mobile/PWA

## Abrir localmente
Extraia o ZIP e abra `index.html` no navegador para testar a interface.

## Testar instalação PWA
A instalação e o modo offline exigem servir os arquivos por HTTPS ou `localhost` (não funcionam abrindo o HTML diretamente como `file://`).
Uma opção local é executar, na pasta do projeto:
```bash
python -m http.server 8000
```
Depois abra `http://localhost:8000` no navegador. Em hospedagem, publique em um domínio HTTPS. No Android, use o menu do navegador e escolha **Instalar app** ou **Adicionar à tela inicial** quando disponível.

## O que está incluído
- Layout responsivo com navegação lateral no desktop e menu inferior no celular.
- Manifesto PWA, ícone e service worker para cache básico/offline.
- Marcação das tarefas do dia com persistência local no navegador.
- Cadastro de linhas no caderno de erros durante a sessão.
- Seleção/listagem de PDFs na sessão.
- Telas demonstrativas de cronograma, questões, revisões e assistente IA.

## Limitações importantes
Este é um protótipo front-end. Indicadores e cronograma são dados de demonstração; o caderno de erros e os PDFs ainda não são sincronizados em nuvem. Não há login, banco de dados, questões reais, notificações push nem integração real com IA. Para produção, implementar API e banco de dados, autenticação, armazenamento seguro e integração de IA no servidor. Nunca colocar chaves secretas da IA no JavaScript do navegador.
