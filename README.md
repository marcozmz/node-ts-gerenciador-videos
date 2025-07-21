# Gerenciador de Vídeos

## Descrição

O **Gerenciador de Vídeos** é uma aplicação inspirada na interface da Netflix, criada para organizar e exibir vídeos em diversas categorias temáticas. O objetivo é centralizar conteúdos audiovisuais, proporcionando uma navegação simples, organizada e agradável.

## Funcionalidades

- **Listagem de vídeos por categorias:** Os vídeos são agrupados em categorias como tecnologia, entretenimento, esportes, saúde, entre outros, permitindo explorar conteúdos de forma segmentada.
- **Filtro por nome de canal:** Permite buscar vídeos pelo nome do canal de origem, facilitando o acesso ao conteúdo desejado.

## Endpoints

### Listar vídeos por categorias

- **Endpoint:** `GET /list`
- **Descrição:** Retorna uma lista de vídeos organizados por categorias.
- **Exemplo de resposta:**

```json
[
  {
    "channelName": "TechWorld",
    "title": "Revolução da IA - Episódio 1",
    "videoId": "abc123",
    "cover": "https://i.ytimg.com/vi/abc123/maxresdefault.jpg",
    "link": "https://www.youtube.com/watch?v=abc123",
    "categories": ["tecnologia", "inteligência artificial"]
  },
  {
    "channelName": "VidaAtiva",
    "title": "Treino Funcional em Casa",
    "videoId": "xyz789",
    "cover": "https://i.ytimg.com/vi/xyz789/maxresdefault.jpg",
    "link": "https://www.youtube.com/watch?v=xyz789",
    "categories": ["saúde", "fitness"]
  }
]
```
### Filtrar vídeos por nome de canal

- **Endpoint:** `GET /video?channelName={nome}`
- **Descrição:** Retorna uma lista de vídeos com base no nome do canal fornecido.
- **Exemplo de requisição:** `GET /video?channelName=TechWorld`

## Tecnologias Utilizadas

- **TypeScript:** Linguagem usada para garantir tipagem estática e segurança no desenvolvimento.
- **Tsup:** Empacotador leve e rápido para projetos TypeScript.
- **Tsx:** Execução rápida de arquivos TypeScript no modo de desenvolvimento.
- **Node.js:** Ambiente para execução de código JavaScript no servidor.
- **@types/node:** Tipagens auxiliares para desenvolvimento com Node.js em TypeScript.

## Como Utilizar

1. Clone este repositório.
2. Instale as dependências com `npm install`.
3. Execute o servidor com `npm run start:dev`.
4. Utilize os endpoints disponíveis para listar ou filtrar vídeos.

## Contribuição

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou enviar pull requests com melhorias, correções ou novas funcionalidades.

## Licença

Este projeto está licenciado sob a Licença MIT.
