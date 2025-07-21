# Podcast Menager

### DESCRIÇÃO
Um app ao estilo Netflix, aonde possa centralizar diferentes episodios de podcast separados por categoria

### DOMINIO
Podcast feitos em video

### FEATURES
- Listar os episodios podcast em sessoes de categorias
    - [saude, fitness, mentalidade, humor]
- filtrar episodios por nome de podcast

## COMO

### FEATURE:
Listar os episodios podcast em sessoes de categorias

### como vou implementar:
Vou retornar em uma api rest (json) o nome do podcast, nome do episodio, imagem de capa, link e categoria

```js
[
{
    podcastName: "flow",
    episode: "CBUM - Flow #319",
    videoId: "pQSuQmUfS30",
    cover: "https://i.ytimg.com/vi/pQSuQmUfS30/maxresdefault.jpg",
    link: "https://www.youtube.com/watch?v=pQSuQmUfS30",
    categories: ["saude", "esporte","bodybuilder"],
},
]
```