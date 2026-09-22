# PRE-KNOWN METER · Ernandes

Ferramenta interativa de diagnóstico prévio para aulas, cursos e eventos.

## O que já existe

- Estúdio para criar, editar, duplicar, ordenar e excluir perguntas.
- Código de sala e QR Code para participantes.
- Modo professor e modo participante.
- Resultados ao vivo.
- Persistência das sessões e dos resultados no `localStorage` do navegador do professor.
- Exportação de resultados em CSV e sessão completa em JSON.
- Importação de sessões JSON.
- Biblioteca local com múltiplas sessões.
- Tipos de pergunta: nuvem de palavras, múltipla escolha, múltiplas escolhas, escala 0–10, estrelas, resposta aberta, número, ranking, clique no mapa, matriz Likert e plano XY.
- Mapa com OpenStreetMap/Leaflet.

## Arquitetura

O GitHub hospeda apenas o aplicativo estático. Configurações e resultados persistem localmente no navegador. Para comunicação ao vivo entre dispositivos, o aplicativo usa um tópico temporário do `ntfy.sh` derivado do código da sala. O relay transporta mensagens; ele não é o banco de dados da aplicação.

## Uso

Abra `index.html`, escolha **Sou o professor**, monte a sessão e clique em **Ao vivo**. Conecte a sala, projete o QR Code e transmita a pergunta atual. Participantes podem entrar pelo QR Code ou pelo código exibido.

> Não use a ferramenta para coletar dados pessoais sensíveis. O código da sala funciona como identificador do canal temporário.
