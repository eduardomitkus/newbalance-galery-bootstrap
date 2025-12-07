# Guia de Otimização de Imagens

## Tamanhos Recomendados

Para os cards da galeria, use imagens com:
- **Largura:** 800px a 1200px (suficiente para boa qualidade)
- **Formato:** JPEG com qualidade 75-80%
- **Peso ideal:** 100KB a 300KB por imagem

## Ferramentas Online (Mais Fácil)

### 1. TinyPNG / TinyJPG
- Site: https://tinypng.com
- Comprime JPEG e PNG automaticamente
- Mantém boa qualidade visual
- Reduz 60-80% do tamanho

### 2. Squoosh (Google)
- Site: https://squoosh.app
- Permite ajustar qualidade em tempo real
- Suporta WebP
- Interface visual para comparar antes/depois

### 3. ImageOptim (Mac) / FileOptimizer (Windows)
- Aplicativos desktop
- Comprimem múltiplas imagens de uma vez

## Processo Recomendado

1. **Baixe as imagens** das camisas dos clubes
2. **Redimensione** para 1000px de largura (mantém proporção)
3. **Comprima** usando TinyPNG ou Squoosh
4. **Salve** na pasta `images/` com os nomes:
   - `liverpool-2013-2014.jpg`
   - `porto-2015-2016.jpg`
   - `sevilla-2015-2016.jpg`

## Exemplo de Tamanhos

| Imagem Original | Após Redimensionar | Após Comprimir | Redução |
|----------------|-------------------|----------------|---------|
| 5 MB (4000px)  | 800KB (1000px)    | 150KB          | 97%     |
| 3 MB (3000px)  | 600KB (1000px)    | 120KB          | 96%     |

## Dica Extra

Se quiser usar WebP (formato mais moderno e leve):
- Use Squoosh para converter
- Adicione fallback no HTML:
```html
<picture>
  <source srcset="images/liverpool.webp" type="image/webp">
  <img src="images/liverpool.jpg" alt="Liverpool">
</picture>
```

Mas para este projeto, JPEG comprimido já é suficiente!
