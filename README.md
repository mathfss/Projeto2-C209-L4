# Edição de Vídeo com MoviePy

Este projeto utiliza a biblioteca [MoviePy](https://zulko.github.io/moviepy/) para realizar diversas edições em um vídeo, incluindo manipulação de imagem e áudio. Ele foi implementado em um notebook Python (`.ipynb`) para facilitar a visualização e execução do código.

## Funcionalidades

1. **Inversão de imagem no eixo vertical a cada 20 segundos**
   - O vídeo é dividido em segmentos de 20 segundos, e os segmentos ímpares têm suas imagens invertidas no eixo vertical.

2. **Redução gradativa de volume**
   - O volume do áudio diminui gradativamente nos últimos 30 segundos, chegando a zero nos últimos 10 segundos.

3. **Corte e reposicionamento de trecho**
   - Após o primeiro minuto (60 segundos), o vídeo corta um trecho de 20 segundos (entre 60 e 80 segundos).
   - O trecho cortado é removido do vídeo original e adicionado ao final do vídeo.

4. **Exportação final**
   - O vídeo editado é exportado no formato MP4, com compressão de vídeo e áudio otimizados.

## Requisitos

Certifique-se de ter o Python instalado na versão 3.7 ou superior e as seguintes bibliotecas:

- `moviepy`
- `numpy`
- `matplotlib`

Você pode instalar as dependências executando:
```bash
pip install moviepy numpy matplotlib
```

## Uso

1. Clone este repositório:
   ```bash
   git clone https://github.com/seu_usuario/seu_repositorio.git
   cd seu_repositorio
   ```

2. Coloque o vídeo original na pasta do projeto com o nome `video_inicial.mp4`. Você pode alterar este nome diretamente no notebook, se necessário.

3. Abra o notebook (`.ipynb`) e execute os blocos de código na ordem indicada. Cada bloco realiza uma etapa específica do processo de edição.

4. Após a execução, o vídeo editado será salvo como `video_final.mp4` na pasta do projeto.

## Estrutura do Código

- **Bloco 1**: Importação das bibliotecas necessárias.
- **Bloco 2**: Carregamento do vídeo original.
- **Bloco 3**: Aplicação de inversão de imagem no eixo vertical a cada 20 segundos.
- **Bloco 4**: Redução gradativa do volume do áudio.
- **Bloco 5**: Corte e reposicionamento de um trecho do vídeo.
- **Bloco 6**: Exportação do vídeo final.

## Observações

- Certifique-se de que o vídeo original esteja no mesmo diretório que o notebook.
- O tempo total do vídeo original deve ser superior a 80 segundos para que todas as edições sejam aplicáveis.
- O vídeo final será exportado com compressão de áudio e vídeo usando os codecs `libx264` e `aac`.
