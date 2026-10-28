# MBNet — lista de licenças (checagem online)

Este repositório é **público de propósito**: os MBNet instalados nos clientes leem daqui, quando o
computador tem internet, o arquivo **`status.mbs`** com as licenças bloqueadas.

- O arquivo é **assinado** com a mesma chave privada das licenças (fica só com o fornecedor).
  Ninguém consegue criar ou alterar a lista sem ela; um arquivo adulterado é ignorado.
- Cada lista tem um número crescente: um MBNet nunca aceita uma lista mais antiga que a última recebida.
- Não há dados de clientes aqui: só os IDs das licenças bloqueadas e uma mensagem opcional.

## Como publicar

1. Abra o **Gerador de Licenças** › aba **Bloqueio online**.
2. Coloque os IDs das licenças a bloquear (um por linha) e, se quiser, uma mensagem.
3. Clique em **Gerar status.mbs** e salve o arquivo.
4. Neste repositório: **Add file › Upload files**, envie o `status.mbs` (substituindo o anterior) e
   clique em **Commit changes**.

Para desbloquear, gere uma lista nova sem o ID e publique de novo.
Os MBNet conferem a cada 6 horas (e 1 minuto depois que o serviço inicia).
