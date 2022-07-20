# Log
## 2022-07-19
Ok, após andar nas couves durante demasiado tempo, 
2 problemas na aplicação do código da aula no dataset das RM.
Para o caso de ajudar alguém, 
isto foi o que identifiquei e possíveis soluções para começar a 
gerar imagens sintéticas:

1) O número de canais está hardcoded para 1. 
O número de canais das imagens do dataset é 3. Soluções:
  - Mudar o 1 para 3
  - Implementar código para inferir o número de canais
  - Usar apenas 1 dos canais
  - Converter para preto e branco (e.g. adicionar uma transformação na cadeia -> transformers.Grayscale())

2) Estas redes não se dão bem com um batch size pequeno, 
nomeadamente de 1. Eu estava a ter problemas com isto, e 
indiquei ao dataloader para ignorar o último batch se for não 
regular (adicionar argumento drop_last=True).

Considerations about batch size
 - https://stackoverflow.com/questions/66133492/pytorch-training-with-batches-of-different-lenghts
