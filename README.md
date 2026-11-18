# Teste isolado de Luau decompilado

Este repositório é somente para **depuração** do arquivo decompilado MoonSec V3. Não faz parte do Bugnana Hub.

## Arquivos
- `ffff_clean_corrigido.lua`: primeira versão recuperada, preservada como referência.
- `ffff_clean_teste.lua`: versão de teste, com seis strings de status quebradas corrigidas.

## Verificação realizada (18/11/2026)
- Compilador: `luau-compile.exe`, sem executar o código no Roblox.
- A primeira versão falhava com 6 mensagens `Malformed string` (linhas aproximadamente 7751, 8276, 11679, 12260, 12904 e 15175).
- Na versão de teste, essas mensagens não aparecem mais.
- A compilação ainda falha perto da linha 6293 com `Out of registers ... exceeded limit 255`. Há uma chamada gerada pelo decompilador com muitos parâmetros/variáveis; precisa ser reconstruída com cuidado.
- Portanto, **não há confirmação de que o script funcione**. Não executar como se estivesse corrigido.

Aviso: o repositório é público. O source foi colocado aqui para teste e inspeção estática.
